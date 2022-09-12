# Building/Creating Plant Humanities Lab and Juncture
Flora, frameworks, academic fields
A Framework for Flora and Fledgling Fields??

## Introduction

In botany, a rhizome is a horizontal subterranean root system capable of sending out both shoots and roots, serving to both ground the plant and allow for its continuous regeneration and growth. Picked up by philosophers Gilles Deleuze and Felix Guattari in the late 20th century[^ref1], the rhizome became a model for a networked mode of non-hierarchical, heterogeneous, multiplicitous thought and communication.[^ref2] Rhizomatic thinking, destabilizing what Guattari and Deluze considered a traditional “tree” model of Western thought in which all leaves stem from a definitive and authoritative core, would allow for connections to be made in nonlinear fashions, without center and free from hegemony. While the rhizome might seem abstract as a concept, its use as a metaphor stems directly from its botanical, physical structure.

The rhizome might also be a fitting way to describe the ways in which the Plant Humanities Lab by JSTOR Labs creates a uniquely connective and generative learning experience with plants. The Plant Humanities Lab is both a resource for learning about plants through a collection of “plant narratives,” or visual essays crafted by scholars that connect the histories of plants with further sources, as well as a tool for researching plants using numerous primary sources, databases, and scholarship. Using linked open data to create relationships across various dimensions such as plants’ cultural histories, genealogies, and geographies, the Plant Humanities Lab supports interdisciplinary study of plants from the various perspectives of the arts, sciences, and humanities, to explore their extraordinary significance to human culture. Furthermore, the Plant Humanities Lab’s powering infrastructure, Juncture[^ref3] – a free, open-source framework for converting simple text files into an engaging visual essay – allows for this web to be extended even further by enabling users to craft multifaceted, multi-media essays of their own. 

With funding from the Mellon Foundation in 2018, the Plant Humanities Lab began as a project to design, develop, and build a prototype of a digital tool for the emerging field of Plant Humanities – a new and interdisciplinary field exploring and communicating the unparalleled significance of plants to human culture. This project not only resulted in the creation of an innovative digital tool, but also, in so doing, supported the further rootedness of the field itself by illustrating the value of visualizing the complex relationships between plants and humankind. Humans rely on plants for our most fundamental individual and social needs: from food, medicine, and construction to our encounters with them in art and literature. Although we often think of plants as rooted in place, their global travels over the millennia offer fascinating pathways into the past and illuminate some of the most burning issues of today, including legacies of colonial violence and displacement. Climate change, habitat loss, and accelerated species extinctions add to the urgency of researching plant–human interactions and acknowledging the importance of plants in our environment. The plant narratives currently available in the Plant Humanities Lab speak to this thicket of interrelated concerns, and open onto future work to draw connections across plants, people and places.

In this paper, we will first describe the process of creating the Plant Humanities Lab in collaboration with Dumbarton Oaks, including efforts to improve search capabilities and support visual essay creation; then, we will take a deeper dive into the Plant Humanities Lab’s functionality and learning experiential qualities by highlighting one visual essay on the site; and finally, we will share reflections on participating in the further establishment of Plant Humanities as a discrete field of study, as well as future directions for leveraging linked open data for and across additional disciplines. 

## About JSTOR Labs 

JSTOR Labs works with partner publishers, libraries and labs to expand access to knowledge by creating tools for researchers, teachers and students that are useful, innovative, and spark curiosity and imagination. The team employs an agile, iterative, and user-focused approach that is inspired by the “design thinking” and “lean startup” communities. This approach has been used by the Labs team previously to create innovative tools like Text Analyzer, which helps users to text mine a document in order to discover relevant scholarly writings, and to explore complex problem areas as in the Reimagining the Monograph project, which sought to unlock some of the value lost in the transition from longform scholarship to fully digital by investigating and prototyping alternate ways of presenting scholarly argument. 

JSTOR is a digital library with a mission to expand access to historical and educational materials, and provides access to more than 19 million academic journal articles, books, and primary sources in 83 disciplines. In 2021, JSTOR received 304 million unique visitors from 240 countries, attesting to the broad reach and relevance of this database across the globe. JSTOR Labs, often in partnership with libraries and archives, explores and develops new ways to discover, interact with and utilize this vast and varied collection for teaching and learning.  

JSTOR and JSTOR Labs are part of the nonprofit organization ITHAKA, whose mission is to advance, preserve and increase access to knowledge, and to improve teaching and learning through the use of digital technologies. This vision implicitly hinges upon expanding this access of diverse populations and communities of learners. JSTOR Labs’s work is one part of an organization-wide program aimed at supporting the needs of incarcerated learners. In addition to efforts to increase incarcerated students’ access to academic resources, this program includes original research conducted by Ithaka S+R, ITHAKA’s research and strategic advisory group, to help guide programs and policies toward better academic outcomes for incarcerated individuals, and the American Prison Newspapers: 1880-2020 project, which seeks to deepen public understanding of mass incarceration through digitization of hundreds of newspapers published in US prisons over the past 200 years.

## About Dumbarton Oaks

Dumbarton Oaks is a Harvard University research institute, library, museum, and garden located in Washington, DC. The institution is the legacy of Robert and Mildred Bliss, collectors of art and patrons of learning in the humanities. Dumbarton Oaks’ mission is, first, to maintain what we have been entrusted by the Blisses to preserve. Second, to support the pursuit of the humanities as a whole, with particular focus on the disciplines of Byzantine, Pre-Columbian, and Garden and Landscape Studies. Third, to honor the intention of the donors by achieving the greatest mutual advantage between Harvard and Dumbarton Oaks. Fourth, to serve the larger public through the museum, garden, and our music program. 

The Plant Humanities Lab has had a lasting impact on Dumbarton Oaks’ intellectual focus. Following the conclusion of this project, Dumbarton Oaks has continued the interdisciplinary summer program that was created; plants and their social worlds have influenced Dumbarton Oaks’ collecting and public programs; and our core areas of study are ever more welcoming of research projects and fellowship applications focused on plant humanities. Dumbarton Oaks continues to fund and run the Plant Humanities Summer Program, a unique synthesis of interdisciplinary approaches to plants and a great feeder of talent. Dumbarton Oaks also hopes to continue creating collaborations with faculty at diverse institutions to continue testing the adoption of the Plant Humanities Lab in the classroom; and to help develop education and public outreach projects related to the Plant Humanities Lab. 

## Creating the Plant Humanities Lab: Collaboration with Dumbarton Oaks

In 2017, JSTOR Labs and Dumbarton Oaks held a day-long workshop to foster exchange about expanding the availability of primary sources online and increasing their usefulness to researchers and students, with a focus on the social and historical contexts of botany and horticulture. Informed by user research conducted prior to the meeting, we discussed how individuals currently discover and use botanical primary sources, brainstormed and sketched possible new approaches to meet their needs, and considered what current and future approaches and source materials held the greatest promise for enhancing the value of this content for a broader array of research communities. 

With support from a Mellon Foundation grant in 2018, the Labs team and Dumbarton Oak faculty began building some of the ideas generated with a grant structured to support two distinct strands of research and development. 

Dumbarton Oaks, seeking to build a community of practice around the emerging field of plant humanities, brought scholars together to curate content that would seed the visual essays and database of the Plant Humanities Lab. Dumbarton Oaks also developed the Plant Humanities Summer Program to fund scholars with an interest in plants from the perspectives of botany, botanical exploration, the history of science and medicine, environmental studies, art history, literature, and the history of the book and botanical illustration. Dumbarton Oaks provided their subject area and collection expertise to the collaborative project, guiding the selection of plants for the Plant Humanities Lab based on what might be interesting (i.e. not an overly-studied plant, but with a rich story to tell and material to support that story) but also with an eye toward highlighting the the different kinds of relationships and uses humanity has with plants, e.g. agriculture, medicine, industry, etc. 

JSTOR Labs, reciprocally, took on the project of developing the digital tool and infrastructure that would bring the collective team’s shared goal of supporting research, discovery and scholarship on these rich topics to fruition. The tool would need to enable two mutually beneficial but discrete functions and purposes: 1) to foreground specific, careful collection of content, hand curated by experts, and 2) to utilize the scale and machine processing that a digital tool allows. These twin pressures helped to shape and power what ultimately emerged as the two complementary halves of the Plant Humanities Lab: respectively, the visual essays and linked open data-enabled plants database, which together allow for both deep dives into specific plant histories, as well as broader, more far-flung exploration. Both of these functions are readily available to explore on the landing page of the Plant Humanities Lab site, the database accessible via the search bar and plant narratives currently featured on the site appear as clickable thumbnails which lead to each visual essay. Furthermore, the database is links back to visual essays which feature that particular plant (fig–), seamlessly connecting these two functions of and spaces that comprise the Plant Humanities Lab.  

Over the course of ___/beginning in June 2019, the Labs team worked to create the Plant Humanities Lab, prototyping x versions and conducting user testing…just notes not prose yet but we had user research in June/July 2019 in person at DO, then August 2019, then April 2021. 
 

What resulted from this collaboration with Dumbarton Oaks was not only a useful tool – but a turning of a new leaf for possibilities in scholarly publishing and research, all driven by a team of academics, technology experts, and libraries working together to discover a new way to create and share academic knowledge. 

## Show and Tell: Supporting Visual Essay Creation

The Plant Humanities Lab project set out to enable telling the stories of plants not only easier, but also more visually and intellectually compelling, through supporting visual essay creation. JSTOR Labs worked to expand the technical capabilities of the visual essay, seeing it as an ideal medium to support the writing of complex narratives; visual essays are uniquely able to draw on a plethora of sources with a coherence and cohesiveness on the digital page that traditional scholarly publishing does not yet support. Whereas in a traditional academic article, much of the scholarly and source material would be ancillary, visual essays in the Plant Humanities Lab feature sources side by side, as interwoven and interactive elements with value in their own right. This presentation of material allows for seamless triangulation between sources and types of sources, ultimately providing a richer experience with those materials than in traditionally static print contexts. High resolution images from library collections can be zoomed into, making it possible to get an up-close look at a 16th century watercolor illustration of cacao in a manuscript, for example, next to definitions of terms and context about this type of herbal manuscript (fig.-), while still situated within the essay’s framing text. The viewer/reader might pause their reading of a given essay in the Lab to more deeply explore numerous resources, presented in parallel on the screen– perhaps to compare an illustration of a plant specimen with a color photograph of it using a feature that overlays these images (fig.--), or to follow a migration path on a map, to view a botanist discussing xyz in a video (fig.--), or to examine key events on an interactive timeline (fig.--).

The visual essay format thus also lays bare the construction of scholarly knowledge, directly showing the viewer/reader the diversity of sources utilized by the author in building their narrative and helping the reader to understand how they have arrived at an understanding of a plant’s history. Showing sources while simultaneously telling a story of the plant in prose creates a unique and empowering encounter with scholarship by enabling a demystification of the scholarly writing process as the reader/viewer is placed at the center of their own experience of processing and exploring dimensions of a given plant narrative.

In a rapidly changing digital environment in which countless needling and/or enticing things compete for our attention – you may have received a pop-up notification from your inbox, or strayed to another, more alluring browser tab by this point in the essay – harnessing our capacities to take in new information while also adapting to new norms of viewer/readership that exist within an context of myriad distractions and multi-layered, hybrid experiences has become paramount to supporting learning. The Plant Humanities Lab optimizes for an increasingly multimedia mode of attention and nascent forms of digital publishing that may follow, allowing for multiple forms of engagement that are nonetheless anchored by the throughline of the text. 

Developing the features of the Plant Humanities Lab that make such a rich multimedia experience with scholarship possible proved technically challenging on two main fronts: 1) the endeavor to create a full library of tools (such as the aforementioned maps, zoomable images, and videos) for authors to use, 2) balancing the need for ease of use and relevance of tools for authors crafting their visual essay, with the need to create an engaging, exploratory experience for the reader/viewer. 

### Building the library of tools 

How did we start approaching this? Were there existing models that we looked to? What worked and what didn’t? 

### Making Plant Humanities Lab usable and useful for authors and learners

How did we start approaching this? Were there existing models that we looked to? What worked and what didn’t? 










## A Closer Look at a Plant Narrative

### Cacao: Indigenous Network to Global Commodity

In “Cacao: Indigenous Network to Global Commodity,” Plant Humanities scholar Rebecca Friedel takes us on a botanical and visual journey – specifically, cacao’s journey across the globe beginning in the 16th century as European colonists extracted the plant from Mesoamerica and transported it to Europe. The visual essay format allows the reader/viewer to explore this complex history through numerous overlapping primary and secondary sources such as botanical illustrations, artworks, maps, and definitions of terms drawn from Wikidata sources. 

“Cacao: Indigenous Network to Global Commodity,” is an exemplar of the visual essay as a medium supported by the Plant Humanities Lab. The Cacao visual essay grounds its viewer/reader’s understanding of the plant’s origins, features and delicious uses (chocolate, of course!) with the help of multiple, overlapping primary sources. “Cacao” illustrates the uniquely horizontal, rhizomatic orientation of visual essays as they are enabled by the Plant Humanities Lab, mirroring this narrative’s focus on historical networks in a format that itself allows for networking across diverse sources and places. The essay text occupes the left half of the page, while the right half features the primary sources that the author has connected to specific areas of the text, marked by an icon in the upper right hand corner of each segmented paragraph. This feature serves as a tether between the text and the image, even as one may take a deeper dive into the image on the right panel. 

Not only does the “Cacao” essay feature illustrations hailing from academic library collections and artworks which serve to expand the viewer/reader’s knowledge of the representation of Cacao throughout human history, but also there are visuals that stem from the sciences, such as a diagram showing the stages of the Milpa cycle, a Mesoamerican agricultural process which was used to cultivate Cacao. No matter the viewer/reader’s particular subject of study, this highly multidisciplinary essay provides an entry point to diving deeper into one’s area of interest. Moreover, the page is dynamic, shifting the resources that it provides the viewer/reader as they scroll the length of the essay. For example, the passage on cacao’s global movement is paired with a map which zooms out as the reader/viewer moves through the text, zooming out to reveal the global route of Cacao by 1580. This animation not only establishes basic facts about the means by which Cacao was brought to England, but also lends the passage a greater sense of scale and momentum.

Although many of the featured illustrations in this essay hail from academic library collections and artworks which serve to expand the viewer/reader’s knowledge of the representation of Cacao throughout human history, additional visuals stemming from botanical sciences and agricultural resources, such as a diagram describing the stages of the Milpa cycle, a Mesoamerican agricultural process which was used to cultivate Cacao, appear alongside the text. No matter the viewer/reader’s particular subject of study, this highly multidisciplinary essay provides an entry point to diving deeper into one’s area of interest. 

This visual essay’s use of illustration, animation, and contextual information come together as a rich learning experience made possible by linked open data to connect these disparate sources and media. In addition to its many dynamic augmentations to a more traditional print essay, however, a list of references appears at the conclusion of the visual essay, with links to digital versions wherever possible. These references both promote further engagement toward a deeper dive into informing literature and serve to represent the ongoing conversation that is academic work, across authors, place and time. From the outset, the page makes its participation across a network of sources and scholarship visible: in the top right of the essay screen prompts a “cite this essay” button, allowing for easy reference to the essay in the reader/viewer’s future work, as well as a friendly – and useful – “more resources” button which opens onto Cacao’s record in the database, complete with its taxonomy and connections to further resources to support research, such as relevant articles in the JSTOR Database. 

## Improving Search Capabilities

What were the primary technical challenges to overcome? How were they overcome? 

These narratives are deeply integrated with linked open data; references throughout are tied to Wikidata QIDs, and data from the project's own knowledge graph appear as well. Over the course of the grant, JSTOR:
Developed and supported a self-hosted version of the Wikibase knowledge graph enabling federated semantic search with information contained in Wikidata,
Defined and implemented a user interface allowing users to easily associate essay text with Wikidata entities, including people, locations and taxon elements, 
Conducted five formal usability assessments on the evolving application, in addition to regular informal design and usability reviews.  In addition, we conducted an expert review of the site’s accessibility and made all adjustments needed to ensure WCAG 2.1 compliance. 



## Reflections 

The role of digital tools in establishing a field

Grant-funding Discovery Work (pairing engineering & R&D with academic work)

Value of teaching digital skills 



Recommendations & Next Steps
Make Juncture easier to use
Make Juncture mobile/friendly
Etc.
Build more usage / adoption / training.
Develop / genericize LOD search

Our work on the Plant Humanities Lab validated the potential for linked open data as a means of integrating and connecting diverse multimedia primary and secondary source content. We saw first hand the potential for digital humanities-based tools to support multidisciplinary project-based learning, helping students to gain digital skills that will help them in the marketplace while providing an engaging and empowering learning experience.

# References
[ref1]:  A Thousand Plateaus
[ref2]:  https://lucian.uchicago.edu/blogs/mediatheory/keywords/rhizome/ 
[ref3]:  https://juncture-digital.org

