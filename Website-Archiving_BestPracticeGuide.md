# The Internet does forget - Guidelines for the archiving of scientific websites
Authors: Andreas Frech (LMU) and Yves Vincent Grossmann (MPDL)

Version 1.0 - 18/01/2024

This text has been machine-translated from German to English and slightly edited for readability and accuracy.

## Introduction
### Description of the problem
Contrary to the frequently quoted phrase "The Internet forgets nothing!" and the equally frequently cautioned "right to be forgotten", information often disappears quietly and unnoticed, but steadily from the Internet. These phenomena are referred to as "content drift" (changes of web content under the same address), "link rot" (decay of website links) or "reference rot" (decay of citations of web content). They affect the entire spectrum of the internet, from individual websites and publications to social media providers. While it is true that social media posts in particular remain relevant over a medium-term period, long-term availability is anything but guaranteed, even for major market players. In March 2019, it was announced that the social media platform ["MySpace"](https://de.wikipedia.org/wiki/Myspace#Geschichte ) lost around 50 million photos, videos and audio files uploaded between 2003 and 2016 due to a failed server move. 490,000 mp3s were recovered by the Internet Archive in April 2019, but the majority of the data remained lost. In the 2000s, MySpace was the central hub for musicians and music lovers alike on the internet and the disappearance of both data and the platform itself was long as unthinkable as other major contemporary platforms that have since faltered. Every single website on the Internet requires hardware components such as web servers, storage media and network infrastructure, as well as suitable operating systems, database and web server software. Programming languages, scripts and style sheets are also used to display the content. Each of these components is subject to a technological ageing process and requires extensive care and maintenance. Many of these software components are combined in user-friendly content management systems such as WordPress, which are themselves subject to these ageing processes and require maintenance. The result is the paradox of (apparent) abundance on the one hand and scarcity, i.e. the rapid loss of sources, on the other (Roy Rosenzweig[^9]). When creating a new website, it is therefore important to bear the importance of data archiving in mind from the outset. This enables the long-term preservation of the information published on the site. 
### Aim of the document
Web designers usually build a website with user-friendliness, performance and search engine optimisation in mind. However, it is also becoming increasingly important to design for long-term accessibility and complete long-term archiving, which has an impact on structure, content, functionality and front-end presentation. So how should a website be structured if it is to provide relevant information, either online or in a web archive, for as long as possible - i.e. with a time horizon of more than 10 years, as recommended by the DFG's [Standards for Safeguarding Good Scientific Practice](https://wissenschaftliche-integritaet.de/kodex/archivierung/ )? And what should be considered before web publication?
### Target groups
> **Project managers**
> The guide is primarily intended to support the conceptualisation of projects so that the project content can be kept available online for as long as possible.
>> Important chapters "First steps", "Information models", "File formats and databases", "Graphical representations", "Machine readability", "Website archiving in the guidelines for good scientific practice", "Legal issues", "Data protection", "Checklist for website archiving"

> **Technical staff, web designers**
> The handout is intended to provide developers and web designers with information on which technical parameters and design decisions have an influence on the long-term availability and archivability of a website.
>> Important chapters "Technical", "File formats and databases" "Graphical representations", "Machine readability"

> **Institutions**
> The handout can be used to develop internal standards and guidelines to keep your own websites available in the long term. It can also be helpful when communicating with archiving infrastructure organisations. This also applies to the awarding of contracts, where it can be used to derive requirements.
### First steps and key questions
Here are some points you should consider:
* Define clear objectives for your website and consider what should be communicated and how. What information must, should or can be obtained?
* The simpler the structure of the website, the easier and more secure it is to ensure long-term availability.
* Is the focus of the website on content or presentation and user experience?
* Dynamically generated content is often difficult or impossible to maintain in the long term.
* Organise your data on the website systematically and use clear metadata for better searchability.
* Use a content versioning system to keep track of changes and developments on your website.
* Ensure access controls and data protection measures are in place to protect sensitive data.
* Implement regular backup routines to ensure the security of your data.
* Consider storing important data, such as databases behind a website, on independent archiving platforms that specialise in long-term data protection.
* Regularly monitor the technological ageing of your website's systems and adapt your archiving methods accordingly.
* Choose a reliable web hosting provider and make sure you have sufficient storage space to cope with future data volumes.
* Structure your data in advance for possible data migration if a change of hosting provider is required or the website is permanently transferred to others.
* Consider working with organisations that specialise in the long-term archiving of data.
* Document in detail how your data is archived and managed to make it easier for future generations to use the information.
* Educate your team and stakeholders on the importance of data archiving and sensitise them to best practice.

By taking these steps into account when creating your website, you will ensure that your digital information and cultural heritage are preserved for the future and provide long-term value.

## Information models
Use clear and consistent information models to define the structure and organisation of your website and ensure that the information models are flexible enough to allow for future changes and enhancements. The choice of information model for the presentation of data on a website has a direct influence on digital data archiving; this should also be taken into account if different information models are used on individual web pages of a website. Each of these information models has its own significant properties that must be maintained so that the information is preserved and remains useful in the long term.
### Essential questions
> Which information models exist?
> What are the critical aspects of archiving?

Here are some examples of different information models and how they affect the archiving of digital content:

**Hierarchical information model**
Hierarchical models structure information in a tree structure with main categories and subcategories. As in a web shop, for example, products can be organised into categories and subcategories. The hierarchy could be: Electronics (main category) → Smartphones (subcategory) → Android (subcategory).
 > When archiving, it is important to maintain the hierarchy and structure. Both the main categories and the subcategories should be clearly recognisable. Metadata describing the relationships between the categories is helpful.

**Network information model**
The network model enables non-linear navigation where users can jump from one point to another. Wikipedia is an example where articles are linked together. Users can navigate from one article to the next via internal links.
> Archiving requires the capture of hyperlinks and references to preserve the navigation and links of the website. It is important that users can move seamlessly between linked content.

**Tabular information model**
Tabular structures organise information in columns and rows. In a price comparison portal, products can be displayed in rows and their properties in columns.
> Archiving requires the maintenance of the table structure to ensure that information is displayed in the same columns and rows as on the website.

**Layer-based information model:**
Layer-based models allow interactive navigation through different layers of information, with each layer representing specific aspects of the information, breaking down complex information into clearly understandable layers and allowing for a comprehensible presentation. An example is an interactive infographic where users click on different parts of the graphic to view detailed information. The way in which information is presented is often the main focus here.
> Archiving must preserve interactivity and navigation between layers to recreate the original user experience. This requires careful recording of interactions.

**List-based information model**
Lists provide information in a clear, linear structure. A FAQ section on a website is an example of a list-based presentation.
> When archiving, it is important to maintain the order and list style. The information should be restored in the same orderly sequence.

**Map-based information model**
Map models are used for geographical information and locations. Examples include map services where users click on locations to view more details.
> The archiving of map-based models requires the retention of the geographical context, coordinates and interactive map functions.

**Time-based information model**
Time-based models emphasise the chronological sequence of information. Examples are timelines, time series databases or Gantt charts, where the temporal dimension is an essential aspect of the data to be organised and is important for understanding processes, developments and trends.
> Archiving must preserve the chronological order and temporal relationships of the information. Restoring events and updates is important.

Archiving these models requires careful planning and documentation to preserve the original structure and functionality of the website. Depending on the model, specific requirements and relationships must be taken into account.
## Technical
### Basics
When archiving and using web archives, it must be clear that in most cases the archived website is only an approximation of the original site. If not all areas of a website can be archived, for example due to inaccessible areas, embedded content, dynamically generated content, etc., "blind spots"[^8] can arise for the evaluation and use of the archive. To counteract these "blind spots", orientation and compliance with technical standards is recommended. This can improve overall access, archiving and finding of content.

### Essential questions
> Which web standards can be relevant for website archiving?
> Which technical aspects should be taken into account when building a website?
> What metadata should the website be labelled with?

#### Overview of website archiving
Website archiving means preserving the content, structure, functionality and front-end presentation(s) of a website using different approaches or web archiving tools and presenting them again later. There are different types, which are used differently depending on the requirements and objectives. The most common types are

**1. Static archiving**

***HTML download***
Static HTML snapshots of the website are created and saved.

***Screenshot based***
Screenshots of the website are created at different times to document the visual changes over time. As these are only images of the website, it is not possible to search or interact with them. Dynamically generated content or content designed for user interaction can currently often only be documented with screenshots or screencasts and additional text or audio descriptions.

**2. dynamic archiving**

***Crawling and scraping***
Web crawlers actively search the Internet or specific websites, follow links and extract content from websites. The archived websites are often saved as WARC files and often do not have the full functionality of the original website.

**3. Archiving projects and organisations:**
There are organisations that specialise in archiving web content, such as the Wayback Machine from the Internet Archive Foundation.

**4. content management systems (CMS)**
Some content management systems offer content versioning features that enable some form of archiving. The sustainability and format of the archive are not standardised and must be checked against the archive requirements.

### W3C standards
The World Wide Web Consortium (W3C) has developed a number of standards, compliance with which can ensure long-term availability. These standards ensure a better structure and consistency of websites, which in turn facilitates archiving. 

Relevant [W3C standards](https://www.w3.org/standards/):

1. **[HTML (Hypertext Markup Language)](https://html.spec.whatwg.org/multipage/)**
HTML is the basic building block of the web and is standardised by the W3C. The use of current HTML versions, such as HTML5, ensures a clear and standardised structure of websites, which simplifies archiving.

2. **[CSS (Cascading Style Sheets)](https://www.w3.org/Style/CSS/)**
CSS is another W3C standard and is used to design the visual appearance of websites. The separation of content (HTML) and presentation (CSS) makes it easier to capture the actual content during archiving.

3. **[XML (Extensible Markup Language)](https://www.w3.org/XML/)** 
XML is a standard for structuring data, which can also be helpful when archiving structured information on websites.

4. **[Web Annotations](https://www.w3.org/TR/annotation-model/)**
This W3C standard enables comments, annotations and metadata to be added to web content. This can be helpful for the documentation and interpretation of archived content.

5. **[Web Components](https://www.w3.org/TR/?filter-tr-name=&tags%5B%5D=browser)**
Web Components are a collection of W3C standards that facilitate the creation of reusable web components. This can rationalise the maintenance of web archives.

6. **[Linked Data](https://www.w3.org/TR/?tags[0]=data)**
Linked data principles promote the networking of data on the web. In archiving, this networking can help to better understand relationships between different web content.

7. **[Character encoding](https://www.w3.org/International/questions/qa-what-is-encoding.de)**
For correct display of content and indexing in search engines, the character encoding, i.e. the unique assignment of letters, numbers, special characters and symbols, must be clearly specified. Content should be encoded in UTF-8 as standard.

These W3C standards help to ensure the structure and consistency of web content, which in turn simplifies the recording and archiving of websites. The use of these standards supports long-term archiving and facilitates the later reconstruction of web content.

### Robots
Certain types of instructions in the ```robots.txt``` file may be good for search engine crawlers, but they can prevent archiving crawlers from capturing important web page content that is critical for accurate web page recovery. For example, instructing crawlers to avoid certain directories such as CSS and JavaScript on a web page might not make much difference to search engine crawlers, but they would make a big difference to the quality of the archived record.

### Sitemaps, links and navigation
A web crawler can only capture web pages that are known to it. It works by following links, which means that it can ultimately only archive pages that are accessible via links. It follows that a user using an archived website can only navigate by following links, as server-side functions such as searching in the archive do not work. Therefore, avoid relying solely on JavaScript or other techniques that could obfuscate links to navigate to a particular page and consider creating[^12] a comprehensive sitemap to ensure that the crawler does not miss anything and can easily search and navigate the web archive later. This makes it easier to capture and later access your website and its content. 
A sitemap is a structured list or file that contains information about the organisation, hierarchy and content of a website. A special type of sitemap is an XML sitemap, which is created primarily for search engines and is formatted in XML. It contains information about all relevant URLs on the website, including metadata such as the time of the last update, the frequency of changes and the priority of the pages. It is primarily intended for search engines and makes it easier for them to crawl and index the website efficiently, but is just as useful for archiving crawlers.

#### Stable URLs and redirection
To ensure continuity and accessibility of website recordings in web archives, it is crucial to maintain stable URLs and use redirects when necessary. The stability of a URL over time makes it possible to create a seamless series of website snapshots. If a URL is changed and no redirect to the new address is set up, the likelihood that the new URL will be saved in the next archiving crawl decreases. This effectively separates access to the archived web page before the URL change from access after the change. Web archiving tools are sensitive to URL stability, which also means that URLs with session IDs can be separated from previous captures of the same resource.

### Metadata
Improving metadata enhances the readability of content for search engines, its findability and chronological categorisation in web archives. The timestamps associated with archived content in a web archive indicate when the crawler visited the page, but not necessarily when it was published or updated. Specifying the publish date or last update via the HTTP Last-Modified response header and/or the text in the document then helps users to better understand the temporal context of the content. Timestamps are also valuable in legal proceedings as they prove when the content may have been published or updated.
The use of page-related titles and description elements ```<META>``` facilitates the curation of web pages by web archives, and improves the presentation of search result summaries.

### Web page test for archive readiness
On the [ArchiveReady.com](https://archiveready.com/) page, the archivability of the website can be tested using HTML validity, page structure, Robots.txt, linking and sitemap, among other things. The tests in ArchiveReady.com are by no means exhaustive, but provide an initial overview and good indications of the weak points of the tested website with regard to web archiving.

## File formats and databases
Although a website is perceived as a single unit, it consists of a large number of files and file types. The long-term maintenance of a website therefore also means the long-term maintenance of this diversity of types. Open standards and formats are therefore preferable to proprietary formats when building a website. Regardless of the openness of the standard, general distribution, familiarity and documentation also play a role.

### Essential questions
> Which file formats are used for the website?
> How sustainable are the file formats used?
> How is the data migration process organised?

### Sustainable file formats

The sustainability factors of the US Library of Congress are recommended for the assessment of file formats.[^7] This recommends seven factors for the assessment of file formats: 

**1. disclosure**
This concerns the extent to which complete specifications and tools for validating technical completeness exist and whether they are (freely) accessible.

**2. adoption by users**
This refers to how widespread the format is. This also includes its use as a so-called master format, i.e. for provision to end users, but also as a transport format between technical applications.

**3. transparency**
This refers to the openness of the digital representation for direct analysis; for example, readability with a pure text editor.

**4. self-documentation**
The documenting objects contain basic descriptive, technical and other administrative metadata.

**External dependencies**
Degree of dependency of a particular format on a particular hardware. This also goes hand in hand with the question of anticipated complexity in dealing with future dependencies.

**6. impact of patents**
Extent to which patents adversely affect the ability of archiving facilities to maintain certain content in a format.

**7. technical protection mechanisms**
Implementation of mechanisms such as encryption that prevent the preservation of content by a trusted repository.

### File formats
The choice of file formats for archiving is a key factor in the success (or failure) of digital archiving. In particular, it has been shown that in-house developments harbour a high risk of failure with regard to long-term availability. In contrast, it makes more sense to orientate oneself on existing standards. A standard is better than no standard.

At the same time, it is recommended that the file formats and the associated software and hardware are designed to be as open as possible and as closed as necessary. Non-proprietary formats are generally preserved in the long term thanks to the open source concept. And where this is not the case, at least the code, documentation etc. can be viewed and utilised for your own technical archiving concept.

Nevertheless, it makes sense to consider community-specific aspects of your own scientific field when choosing file formats. The handling of file formats can therefore not be generalised. It is therefore advisable to consider your own specialised community as a target group. The technical conventions of a website should also be taken into account.

When searching for specific file formats for archiving, two contact points are particularly recommended. The Library of Congress in Washington offers a comprehensive overview of [long-lived file formats](https://www.loc.gov/preservation/digital/formats/index.html). The [section on qualitative and functional factors in the archiving of websites](https://www.loc.gov/preservation/digital/formats/content/webarch_quality.shtml) is particularly recommended. The Swiss Coordination Office for the Permanent Archiving of Electronic Records (KOST) offers a comprehensive [catalogue of archival file formats](https://kost-ceco.ch/cms/kad_main_de.html). The [Overview of standards and guidelines in digital archiving](https://kost-ceco.ch/cms/standards_de.html) is particularly suitable for an initial orientation in this topic.

> **Excursus archive format**
> In addition to file formats suitable for archiving, there are also special file formats for archiving web applications. A quasi-standard for archiving websites is [Web ARChive (.warc file)](https://iipc.github.io/warc-specifications/specifications/warc-format/warc-1.1/).[^3] The WARC format offers a standardised way of saving different types of resources, such as HTML, images, stylesheets and other files, enriched with special metadata in a single archive. It is the standard format used by many archive crawlers and archive service providers.
### Data migration
The point of data transfer is one of the critical moments in the archiving of websites. It marks the transition from working mode to archive mode. The content editing phase is now complete. In archive mode, practically no more content editing or revision takes place. This point in data migration is generally more of a procedural challenge than a technical one. This is because users have to say goodbye to the fact that their "own" website is no longer under their (content) control. However, this is offset by the advantage of long-term archiving and thus the availability of information and form.

The form of data migration depends heavily on the structure and technical circumstances of the website. For websites that contain many PDF files, for example, different migration strategies must be developed than for project websites that consist mainly of html elements. This also shows that archive-friendly platforms offer a long-term advantage as a basis. Widely used content management systems such as Wordpress already offer archiving functions and extensive documentation. Open source systems also offer the advantage that there are usually communities with others who may have already found answers to such questions or are looking for them together. This can significantly simplify the migration of data for the archiving of websites.

## Graphical representations
The reproduction of graphical elements of a website in an archived state is associated with numerous challenges. The problems usually increase exponentially with the complexity of the visual elements. The simpler the technical elements of a website are, the easier it is to archive in terms of form and content.

### Essential questions
> Are external extensions used?
> What significance do graphic elements have for the website?
> What meaningful information do graphic elements convey? And how can they be preserved in the long term with low technical complexity?

### Reduction of external extensions

Technical elements such as extensions, plugins, external libraries, online databases etc. increase the complexity of the application. For archiving, their use means that pure bitstream preservation is not sufficient in most cases, e.g. to preserve the graphical representations of interactive maps. The interaction of the technical systems makes it necessary for the functionalities of the interfaces to be preserved.

In order to reduce such dependencies in maintenance, it is advisable to use dynamic and embedded external elements as sparingly as possible. By dispensing with plugins and individual extensions, path dependencies are avoided so that archiving is less complex and also more stable in the long term.

### Reproduction of the visual impression

The visual representation of web pages is usually an essential piece of information that needs to be reproduced as completely as possible during archiving. At the same time, browsers are constantly being further developed as interpreting software for websites. In the long term, this leads to problems with the display of e.g. images, graphic elements such as menu bands, which are essential for the original impression of a website.
In order to preserve the visual impression of html-based pages, KOST recommends the [PDF/A-2 for Hypertext](https://kost-ceco.ch/cms/pdf-a-2-fuer-hypertext.html) format, for example. This allows html files and their graphical interpretation to be reproduced. With PDF representation, the graphic design is retained at the time of archiving. In view of the constant further development of browser technologies, this is an aspect that should not be underestimated for the long-term archiving of scientific websites.


### Strategic planning for "Look&Feel"
When planning your own website, it is therefore particularly advisable to be clear about the requirements and wishes for the graphical presentation. The more complex the design of the website, the more difficult it usually is to archive the website. It makes sense to address this conflict of objectives at an early stage in order to establish explicit guidelines and measures. In this way, your own requirements and the technical possibilities can be harmonised.
If this decision is postponed and only made shortly before archiving, it is usually too late. Ultimately, this can also mean that the website is not archived after all and is therefore irrevocably deleted.

## Machine readability
Artificial intelligence (AI) is in the spotlight thanks to the impressive capabilities of current language models. Intelligent chatbots impressively illustrate the current state of research and development in the field of text analysis and text generation. However, the success of AI solutions depends not only on having suitable algorithms for the respective application area, but also on having the best possible texts and data to train these language models. If texts are to be extracted from a corpus of archived websites for a research project, the design of the websites plays an important role. A website can be structured in such a way that text extraction can be carried out particularly efficiently and accurately.

### Essential questions
> Why is machine readability important?
> What aspects need to be considered in web design?

Implementing the following practices will help text extraction tools and search engines to better understand and interpret the content of your website:

**1. Semantic HTML structure**
Use a clear, semantic HTML structure. This means using heading tags (h1, h2, h3, etc.) for headings, paragraph tags (p) for paragraphs and lists for lists. This makes it easier to identify and extract text elements.

**2. Meaningful classes and IDs**
Use CSS classes and IDs to identify text elements, especially if they have a special meaning. This makes it easier to extract text from specific sections of the website.

**3. Avoid complex layouts**
Overly complex layouts, especially those generated primarily by CSS and JavaScript, can make text extraction difficult. Endeavour to use a simple and understandable layout.

**4. Structured metadata**
Add metadata such as author information, creation, publication and modification dates, and categories. This information can be helpful in extracting and understanding the context.

**5. Alternative texts for media**
If you use images or other media, provide them with alternative text (alt text) to describe their content. This is important to understand the text content of these elements.

**6. Clear separation of content**
Separate the main text content from secondary information such as navigation elements, adverts and so on. This can be achieved using HTML tags and CSS.

**7. Use microdata and structured data**
Use structured data markup such as Schema.org to label important information on the website. Search engines and text extraction tools can use these markers to better understand the content.

**8. Valid HTML and CSS** 
Make sure your HTML and CSS are up to standard. Errors in the code can affect text extraction.


## Web page archiving in the guidelines for good scientific practice
The long-term archiving of websites in a scientific context takes place within different normative frameworks.

### Essential question
> Do the guidelines in the DFG Code also apply to your own project website?
> Is there an institutional regulation for archiving project websites?
> Are there community-specific standards for website archiving?

### Website archiving in the DFG Code

The [DFG "Guidelines for Safeguarding Good Scientific Practice"](https://www.dfg.de/download/pdf/foerderung/rechtliche_rahmenbedingungen/gute_wissenschaftliche_praxis/kodex_gwp.pdf) are fundamental in the German context. According to these guidelines, scientists are obliged to preserve the underlying, central materials of their research for an appropriate period of time.[^1] This can also include project websites. The period usually refers to ten years after the end of the project. However, depending on the case and relevance, this period can also be (voluntarily) extended.

### Institutional regulations on website archiving

At the same time, every German scientific institution has its own set of rules for good scientific practice (GWP).[^2] These internal rules may also clearly regulate the availability of research results beyond the end of the project.
At the same time, it is important to note that the partners may be subject to different institutional regulations in co-operation projects. Such problems can be resolved through early clarification, ideally in the cooperation agreement or joint third-party funding application.

### Subject-specific perspective on website archiving

Subject-specific regulations can also affect the archiving of research-related websites. For example, the [DFG review boards can publish subject-specific recommendations for handling research data](https://www.dfg.de/foerderung/grundlagen_rahmenbedingungen/forschungsdaten/empfehlungen/index.html), which also formulate recommendations for website archiving. The subject-specific context of the research project must therefore always be taken into account when making an archiving decision. 

## Legal issues[^13]
Legal issues often affect the archiving of research-related websites. Based on the question of authorship, the options for dealing with the website to be archived develop. These can be decisions such as licensing, time limits or transfer of ownership.

### Essential questions
> What is the ownership structure of the website?
> Who owns the publication and exploitation rights?
> Does the website have a licence?
> How is the transfer of the website to the archiving institution regulated? Is there a deposit contract?

### Clarification of ownership rights
One of the central legal questions when archiving websites is the right of ownership: Who owns the website? Especially in a scientific context, this question often cannot be answered in a generalised way. On the one hand, a project website is usually created as part of an employment relationship. However, the employer is entitled to publication and exploitation rights. On the other hand, the author is generally entitled to the right of publication. Similarly, freedom of research exists in the Federal Republic of Germany according to [GG Art. 5 Para. 3](https://www.gesetze-im-internet.de/gg/art_5.html). Clarification of this situation depends on the details of the employment relationship and the respective contractual agreements.[^4] When outsourcing websites, it must of course also be clarified how the work of development companies and hosting service providers is reproduced when archiving. (Contractual) agreements should also be made in advance for the transfer of data and code from the service provider to the archiving institution.

At the same time, a decision must be made as to how the website is to be categorised. Is it predominantly textual in nature and can it therefore be categorised as a scientific publication? Or do aspects of databases including architectures, nesting and links predominate? In such a case, the website could also be considered a database work according to [UrHrG § 4](https://www.gesetze-im-internet.de/urhg/__4.html).[^5] Here, too, a decision can only be made on the basis of a specific example. If in doubt, please consult experts from your own institution.

### Licence and licensing options

The owner can provide the website with a licence. If possible, this should be done. This legal act makes explicit which usage options are granted by the owner. As with software in general, the compatibility of licences must also be taken into account in the case of websites if external objects are reused. Depending on the context, website content and technical platform must be treated as different legal entities when archiving. In case of doubt, the legal experts at your own institution can provide advice and support.

Common addresses such as https://choosealicense.com, https://opensource.org/licenses/ etc. can provide support in the search for licences. For code components, it is always advisable to select software-specific licences. They contain a disclaimer for faulty code, which data-specific or CC licences do not.

### Accessibility
The use of websites can be subject to barriers. This can be a particular challenge for people with a disability. For this reason, a website must be designed to be accessible. This is derived from EU Directive 2016/2102 on the accessibility of websites and mobile applications of public sector bodies.[^10] This was transposed into national law in 2019 in Regulation BITV 2.0.[^11] This also applies to public universities and research institutions. This applicable law must therefore be observed when designing a website.

The [Web Content Accessibility Guidelines (WCAG 2)](https://www.w3.org/WAI/standards-guidelines/wcag/) of the W3C are a useful standard for concrete implementation. With [WAI-ARIA](https://www.w3.org/TR/wai-aria/), for example, there are concrete specifications that are relevant for websites and their accessible use. At the same time, there are also many digital tools that help to assess the accessibility of a website. Examples of this include the [WCAG Contrast Checker](https://contrastchecker.com/), the [Web Accessibility Evaluation Tool](https://wave.webaim.org/) or the [BITV Test](https://www.bitvtest.de).

### Deposit of the website

The depositum (from the Latin for "deposited") of a scientific website should contain all the files, information etc. necessary for its maintenance. The act of depositing means that the website can no longer be edited by the owner. The archive mode is "read only". As far as possible, the full rights of use to the website should also be transferred to the archiving institution.

In any case, it makes sense to conclude a deposit agreement between the website owner and the archiving institution. This creates legal certainty for both parties and sets a clear framework for the service and expectations for archiving. However, a clear legal categorisation with regard to ownership rights is necessary for such a contract. This is the only way to clarify who is authorised to conclude a legally binding deposit contract. Such an agreement can also contain restrictions on use or issues relating to usage rights. These could be, for example, access restrictions or embargo periods. 

For the archiving of a website, the transfer of ownership rights may be advisable under certain circumstances. The background to this is that the preserving institution can also take curatorial measures such as updating the database and rectifying security gaps. Depending on the agreed preservation scenario and relevance, such an approach may make sense.

An archiving right on the part of libraries, interpreted as a right to redundant storage and, if necessary, transformation into other file formats, may also be covered by [UrhG § 60e para. 1-3](https://www.gesetze-im-internet.de/urhg/__60e.html) under certain circumstances. This path should be discussed together to see whether such a path offers additional opportunities.

## Data protection
Data protection aspects can also affect the long-term archiving of websites. It therefore makes sense to think about data protection as early as possible. Data protection should be taken into account as early as the design decision for a website structure and its technical solution, also with a view to long-term preservation[^6].

### Essential questions
> Has personal or sensitive data been published on the website?
> Is website user data available?

### Data protection when archiving websites

Data protection can take effect in two directions on a scientific website. On the one hand, it can relate to the content of the project page. This may be the case for research projects with personal data, for example. In this case, the page should also not be publicly available or only available to a limited extent before the archive phase. The archive solution must also reflect this fact.

On the other hand, the technical and procedural data of the users must also be considered with regard to data protection. For example, there may be user accounts for publishing and editing with additional personal information or even local passwords. If this information is not absolutely necessary for the use of the archived website, consideration should be given to not transferring it to the archived state. One possibility could be, for example, a technical separation of the project website and user information during operation.

If in doubt, it makes sense to contact the local data protection officer. They can provide advice on further measures and their effectiveness.

## Use cases
### End of project
In many areas, the conception and launch of projects and associated websites can draw on a tried-and-tested toolbox. However, little thought is given to how a project ends when the funding comes to an end and what happens to the resulting websites. References are an essential part of scientific discourse and this depends on information being permanently available for analysis, replication, verification and citation.
The main thing to consider here is what should primarily be preserved: The website content, the possibly separately stored research results or the user experience? Can the individual presentation layers be archived separately and reassembled in a meaningful way? In addition, before archiving, the site should be checked for any personal information that may still exist and should not be archived.

### Retirement
Websites set up by individual scientists over a longer period of time often have a somewhat longer time horizon than project websites. Over the years, these develop into important contact points within the scientific community. When the operator of the website retires, however, the website should continue to be maintained. To make this possible, it is often possible for an institutional operator to take over the hosting - ideally. In an off-boarding process, the modalities of the transfer of ownership must then be clarified, such as the transfer of passwords and admin access or the transfer to other servers. It is also possible to set up a decommissioned mirror and the possible need to set up redirects so that citations and links can still be resolved. The less complex a site is structured, the easier it is to keep it online in the long term.

### Data visualisation. Maps, diagrams, interactive graphics
Today, data must not only be collected, processed and analysed, but also appropriately visualised in order to be able to make statements about it. This often leads to very complex interactive representations in which text and visualisation may even adapt to the reading progress. Data visualisation is therefore a powerful tool for presenting numerical facts. However, it should be noted that complex interactive maps are difficult to maintain in the long term - the more different software components are required for visualisation, the less likely this is the case. If the result of a visualisation is a graphic, it should be created in an established format (see [File format](#File formats) and [Representations](#Representations))

## Examples

### MPDL: Journal for Nature Research
discontinued after own service as website due to low interest; website was taken completely offline and the corresponding PDF files of the journal volumes published as dataset: https://doi.org/10.17617/3.GRUJYR. The former domain https://zfn.mpdl.mpg.de now redirects directly to the dataset.
The solution for website archiving was therefore to retain the content in a different format in the long term but to no longer present the original website. The content in PDF file format took precedence over the form.

## Checklist for website design
- [ ] Definition of the communication goals
- [ ] Definition of information models to be used
- [ ] Conceptualisation of the logical website structure
- [ ] Definition of the technology used
The diversity must remain manageable in the long term
- [ ] Definition of the file formats used
Use open and widespread formats wherever possible
- [ ] Define web design guidelines ("look & feel")
Design decisions and graphic elements have a direct influence on the long-term archivability of the website
- [ ] Identify a web hosting provider
- [ ] Definition of a data management plan (or at least a backup routine)
- [ ] Conception of a versioning concept
Guarantees scientific citation and prevents "content drift"
- [ ] Data protection: Check technical concept
- [ ] Data protection: Check design concept
## Checklist for website archiving
- [ ] Identification of a suitable web archive or infrastructure provider
- [ ] Identification of properties of a website worth preserving 
Possible significant properties: Content (database content, text, etc.), presentation (graphics, map displays, etc.), structure (e.g. chronological sequence) or user experience (animations, design, look & feel)
- [ ] Categorisation: What information must, should or can be retained
- [ ] Metadata labelling of the content
A search may not be available to a web archive
- [ ] Clarification of property rights
- [ ] Clarification of copyrights
- [ ] Removal of copyrighted content
- [ ] Checking for data protection-relevant content
- [ ] Setting up access control and/or removal of privacy-sensitive content
- [ ] Create end-of-project release of the website
- [ ] Independent archiving of databases in research data repositories
- [ ] Deposit agreement with archiving institution
- [ ] Transfer data and software to archiving institution
- [ ] Documentation of archived content
- [ ] Documentation of the methods used
- [ ] Publicising the archiving

## Further information
### Literature
* Federal Ministry of Education and Research: "Urheberrecht in der Wissenschaft Ein Überblick für Forschung, Lehre und Bibliotheken", 2023, 2nd edition, https://www.bmbf.de/SharedDocs/Publikationen/de/bmbf/1/31518_Urheberrecht_in_der_Wissenschaft.pdf?__blob=publicationFile&v=6.
* Dave Bunten and Gregory P. Way: "Long-Term Software Gardening Strategies for Cultivating Scientific Development Ecosystems", 17 August 2023, https://bssw.io/blog_posts/long-term-software-gardening-strategies-for-cultivating-scientific-development-ecosystems.
* Digital Preservation Coalition (2023): Digital Preservation Documentation: A Guide, http://doi.org/10.7207/documentation-23.
* Bastian Gillner, Martin Hoppenheit and Franziska Klein: "Webarchivierung im Landesarchiv NRW", in: Archivpflege in Westfalen-Lippe 96 (2022), pp. 47-51, https://www.lwl-archivamt.de/media/filer_public/5b/d9/5bd9b059-6a16-4b3f-a6d4-d589343b05ab/47-51_gillner_hoppenheit_klein.pdf.
* European Archives Group of the European Union (EAG): Archiving by Design Whitepaper, 25/05/2023, https://commission.europa.eu/system/files/2023-06/Whitepaper%20AbD_en.pdf
* Michelle Lindlar: "Evaluation & Prioritisation of Digital Objects Worthy of Archiving in Practice", nestor Practitioners' Day 2020, https://www.langzeitarchivierung.de/Webs/nestor/SharedDocs/Downloads/DE/praesentationen/2020praktikertagLindlar.pdf?__blob=publicationFile&v=1.
* Mark C. Miller: "Discontinuing a Research Software Project", 04.12.2023, https://bssw.io/items/discontinuing-a-research-software-project.
* Laura Niebling: Scientific Websites -- Past, Present and Future of Science on the Internet, 2020, https://mediastudies.hypotheses.org/1363.
* Stapelfeldt, Kirsta et al: "Strategies for Preserving Digital Scholarship," The Code4Lib Journal 53 (2022), https://journal.code4lib.org/articles/16370.
* Andreas Weber and Claudia Piesche: "Datenspeicherung, -kuration und Langzeitverfügbarkeit", in: Markus Putnings, Heike Neuroth and Janna Neumann (eds.): Praxishandbuch Forschungsdatenmanagement, 2021, https://doi.org/10.1515/9783110657807-019, pp. 327-356.
* Konstanze Weimer and Astrid Schoger: "Das Dateiformat WARC für die Webarchivierung", 2021, https://files.dnb.de/nestor/kurzartikel/thema_15-WARC.pdf.

### Links
* German National Library: https://www.dnb.de/DE/Professionell/Sammeln/Sammlung_Websites/sammlung_websites_node.html
* GitHub Web Archiving Community https://github.com/ArchiveBox/ArchiveBox/wiki/Web-Archiving-Community
* Nestor: https://www.langzeitarchivierung.de
* nestor wiki: Introduction to LTA, https://wiki.dnb.de/x/ObmkBQ
* nestor-Wiki: Web Archiving, https://wiki.dnb.de/x/-rSkBQ
* Library of Congress, Creating Preservable Websites, https://www.loc.gov/programs/web-archiving/for-site-owners/creating-preservable-websites/

## Endnotes
[^1]: DFG, Guidelines for Safeguarding
good scientific practice, 2019, Guideline 17, p. 22 or https://wissenschaftliche-integritaet.de/kodex/archivierung/.
[^2]: See, for example, [Ludwig-Maximilians-Universität München](https://cms-cdn.lmu.de/media/lmu/downloads/die-lmu/beauftragte/richtlinien-der-lmu-muenchen-zur-selbstkontrolle-in-der-wissenschaft.pdf) and the [Max Planck Society](https://www.mpg.de/197494/rulesScientificPractice.pdf).
[^3]: Andreas Weber and Claudia Piesche: "Datenspeicherung, -kuration und Langzeitverfügbarkeit", in: Markus Putnings, Heike Neuroth and Janna Neumann (eds.): Praxishandbuch Forschungsdatenmanagement, 2021, https://doi.org/10.1515/9783110657807-019, p. 349. See also https://kost-ceco.ch/cms/warc.html.
[^4]:BMBF: "Urheberrecht in der Wissenschaft Ein Überblick für Forschung, Lehre und Bibliotheken", 2023, https://www.bmbf.de/SharedDocs/Publikationen/de/bmbf/1/31518_Urheberrecht_in_der_Wissenschaft.pdf?__blob=publicationFile&v=6, p. 43.
[^5]:BMBF: "Urheberrecht in der Wissenschaft Ein Überblick für Forschung, Lehre und Bibliotheken", 2023, https://www.bmbf.de/SharedDocs/Publikationen/de/bmbf/1/31518_Urheberrecht_in_der_Wissenschaft.pdf?__blob=publicationFile&v=6, p. 33. The database owner right [UrhG § 87 para. 2](https://www.gesetze-im-internet.de/urhg/__87a.html) is also still an option. However, this right to protect investments in databases probably rarely applies in academic contexts.
[^6]:Matthias Bäcker and Sebastian Golla: Handreichung Datenschutz, published by the German Council for Social and Economic Data, RatSWD Output 8 (6), 2nd completely revised edition, Berlin 2020, https://doi.org/10.17620/02671.50, p. 31.
[^7]: https://www.loc.gov/preservation/digital/formats/intro/format_eval_rel.shtml#factors
[^8]:Donig, S., Eckl, M., Gassner, S., & Rehbein, M. (2023). Web archive analytics: Blind spots and silences in distant readings of the archived web. Digital Scholarship in the Humanities, 1-16. https://doi.org/10.1093/llc/fqad014.
[^9]:The American Historical Review, Volume 108, Issue 3, June 2003, Pages 735-762, https://doi.org/10.1086/ahr/108.3.735.
[^10]: Directive 2016/2102 of the European Parliament and of the Council of 26 October 2016 on the accessibility of the websites and mobile applications of public sector bodies, https://eur-lex.europa.eu/legal-content/DE/TXT/PDF/?uri=CELEX:32016L2102.
[^11]: Ordinance on the creation of barrier-free information technology in accordance with the Disability Equality Act (Barrier-free Information Technology Ordinance -- BITV 2.0), https://www.gesetze-im-internet.de/bitv_2_0/BJNR184300011.html. Section 2 (2.2) of the BITV 2.0 ordinance contains an exception for "*archives that neither contain content that is required for active administrative procedures nor have been updated or revised* after 23 September 2019".
[^12]: An illustrative example of the concept of a sitemap is given in the article Rockwell, G., Day, S., Yu, J., Engel, M.: Burying Dead Projects: Depositing the Globalisation Compendium. In: Digital Humanities Quarterly, Vol. 8 Number 2, 2014, http://digitalhumanities.org
[^13]: Please note that this text does not constitute legal advice but merely provides information on the subject matter without providing conclusive certainty. For legal advice, please contact your respective legal department.
