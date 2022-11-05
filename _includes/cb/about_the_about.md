{% assign imagesample = site.data[site.metadata] | where_exp: 'item','item.format contains "image"' | first %}
{% capture imagesampleid %}{{imagesample.objectid | default: "https://www.lib.uidaho.edu/collectionbuilder/demo-objects/mg101_b6_photographs_01.jpg"}}{% endcapture %}
{% assign pdfsample = site.data[site.metadata] | where_exp: 'item','item.format contains "pdf"' | first %}
{% capture pdfsampleid %}{{pdfsample.objectid | default: "https://digital.lib.uidaho.edu/utils/getfile/collection/ui_ep/id/21768/filename/uiext21768.pdf"}}{% endcapture %}
{% assign videosample = site.data[site.metadata] | where_exp: 'item','item.format contains "video"' | first %}
{% capture videosampleid %}{{videosample.objectid | default: "https://cdil.lib.uidaho.edu/storying-extinction/objects/trailcams/videos/ballcreek-cedarrub-birdonpath.mp4"}}{% endcapture %}
{% assign audiosample = site.data[site.metadata] | where_exp: 'item','item.format contains "audio"' | first %}
{% capture audiosampleid %}{{audiosample.objectid | default: "https://www.lib.uidaho.edu/digital/mp3s/Clouds.mp3"}}{% endcapture %}

## About Books of Hours

Books, in a common sense, are pages placed inside of a cardboard or paper cover. However, it can also be said that a famous dress or suit is just threads that have been stitched together. A book, just like other objects, always has a story to tell. Their texts can reveal what trends have come and gone in societies over time, and can illustrate changes in what is considered culturally “acceptable” at a given moment. Plates within their binding reveal the status of who owned them. Scribblings in the margins tell us what a previous reader thought. And the wear or preservation of a volume illustrates how high or low it was held in esteem by its last custodian. Books, in this way, are like mini-archaeological digs. They tell stories about those who have come before us when those people can no longer tell us themselves. Sometimes, the details they reveal can be very intimate. Other times, however, a work can illuminate less personal but no less important evolutions within a group of people. That is very true when it comes to “books of hours.”

Books of hours “were the most popular books of the late Middle Ages”, and “survive in significantly greater numbers than any other genre of manuscript” (Clemens/Graham, 2007,       p. 208). They were a means by which lay men and women could “participate for themselves in the daily round of prayer and worship that typified the lives of monks and priests” (Clemens/Graham, 2007, p. 208). There were two main factors which led to a growth in the popularity of books of hours as a text. The first was a desire among the laity, during a period of increasing secularization within their world, to imitate the clergy (Wieck, 1988, p. 27). The second was “the cult of the Virgin,” referring to an increase in the reverence in which Mary, the mother of Jesus, was held during that time (Wieck, 1988, p.27). The “Hours of the Virgin,” a devotion which had previously been added to the breviary, was extracted from that text and made the central feature of the book of hours (Wieck, 1988, p. 27).

The production of books of hours, like the books themselves, was unique and             non-uniform. Plain manuscripts without illustrations were likely available at bookstores in larger settlements, while “lavish versions with texts and pictures selected for a particular owner were commissioned (often at great expense) from the very best artists of the day” (Hindman, 2020). The books were usually written in Latin (the liturgical language of the Roman Catholic Church at the time), and buyers had many choices as to how they wanted their book constructed, such as “support (paper or parchment), color of ink, number and size of pictures…how much blue and gold leaf…borders…and type of binding” (Hindman, 2020). Although books of hours were produced in several European countries, France led the production of them during the entirety of their popularity. As the thirteenth century was ending, “illuminators in Paris and northern France, heirs to the spare but refined Court Style of St. Louis, applied themselves to the decoration of Books of Hours, then just coming into fashion” (Wieck, 1988, p. 28).

The “hours” referenced in the name “book of hours” are in fact “the hours of the monastic divine office, the times of day at which monks gathered in church to pray” (Clemens/Graham, 2007, p. 208). “There were eight of these hours: matins, for which monks rose from their beds at about two a.m., and which was immediately followed by lauds; prime, marking the first hour of the day, around six am; terce, sext, and none, respectively marking the third, sixth, and ninth hours (nine a.m., noon, and three p.m.) vespers, marking the onset of evening; and compline, which brought the day to a close” (Clemens/Graham, 2007, p. 208).

After these lessons would come two prayers addressed to the Virgin Mary. They were known by their opening words: Obsecro te (I beseech thee) and O intemerata (O Spotless one) (Clemens/Graham, 2007, p. 212). Both are “Impassioned prayers that seek to secure the Virgin’s intercession on behalf of the one praying. Obsecro te “movingly commemorates the joys that Mary experienced in bringing Christ into the world and her sorrow at the Crucifixion; the prayer then petitions for her assistance in all that devotee does and requests that she may reveal herself to the devotee at the moment of death” (Clemens/Graham, 2007, p. 212). The other prayer, O intemerata, invokes “the Virgin and St. John, the disciple whom Jesus loved, who, with Mary, witnessed the crucifixion. The prayer requests Mary and John to watch over the devotee throughout life and to intercede on his or her behalf before God, ‘because you can immediately obtain whatever you want from God” (Clemens/Graham, 2007, p. 212).

### Central Feature of the Collection

The medieval text shown below is the first page of Ricketts 135, a book of hours in the possession of the Lilly Library at Indiana University Bloomington. It was digitized at the request of the author of this project. 

#### Ricketts 135 Page 1

{% include feature/image.html objectid="1-0" width="50" %}

#### Include a PDF

- PDF -- > `{% raw %}{% include feature/pdf.html objectid="demo_002"  width="50" %}{% endraw %}`

{% include feature/pdf.html objectid=pdfsampleid width="50" %}

#### Include a Video

- Video: `{% raw %}{% include feature/video.html objectid="demo_004" %}{% endraw %}`

{% include feature/video.html objectid=videosampleid width="75" %}

#### Include an Audio File

- Audio: `{% raw %}{% include feature/audio.html objectid="demo_003" %}{% endraw %}`

{% include feature/audio.html objectid=audiosampleid  %}

### Include Bootstrap Features

The template also provides includes to make it easier to add [Bootstrap](https://getbootstrap.com/) components to your Markdown writing.
These features allow you to better organize and highlight your content.

#### Include a Card

- Card -- > `{% raw %}{% include feature/card.html header="This is a Card" text="The card features an image from the collection as a cap" objectid="demo004" width="25" centered=true %}{% endraw %}`

{% include feature/card.html header="This is a Card" text="The card features an image from the collection as a cap" objectid="demo_001" width="25" centered=true %}

#### Include a Button 

- Buttons -- > `{% raw %}{% include feature/button.html text="Button Link to Somewhere" link="https://collectionbuilder.github.io/" color="success" %}{% endraw %}`

{% include feature/button.html text="Button Link to Somewhere" link="https://collectionbuilder.github.io/" color="success" centered=true %}
  
#### Include an Alert

- Alerts -- > `{% raw %}{% include feature/alert.html text="this is an *alert* that 'warns' a user" color="warning" align="center" %}{% endraw %}`

{% include feature/alert.html text="This is an *alert* that 'warns' a user with centrally aligned text." color="warning" align="center"  %}

#### Include a Modal

- Modals -- > `{% raw %}{% include feature/modal.html button="This is a modal using a 'primary' colored button to invite clicking" title="when clicked:" text="A Modal will pop out a box with some more information" color="primary"  %}{% endraw %}`

{% include feature/modal.html button="This is a modal using a 'primary' colored button to invite clicking" title="When clicked:" text="A Modal will pop out a box with some more information" color="primary"  %} 
