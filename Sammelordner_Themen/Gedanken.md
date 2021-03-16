# Using graph tools as an alternative exploratory tool for clinical data

## Abstract {.page_break_before}

Researchers are often used to find their data in many distributed tables in the form of rows and columns. In relational databases, for instance, the information is linked across multiple tables by unique identifiers and the relationship between data values is only implicitly apparent. By modeling relationships between data types- or values, graph databases have been used successfully in recent years to represent complex, inhomogeneous data. Furthermore, the exploration of the underlying data structure and the data itself is intuitively possible with graph databases. Neo4j as an example of a graph database system can be adapted in many ways with the help of interactive tools to provide a new way of data exploration and analysis. In the present work, we examine the benefit of graph databases as an exploratory and analytic tool for clinical data. In collaboration with domain experts in Obstetrics and Fetal Medicine, we demonstrate how this resource can improve the efficiency and comprehensiveness of hypothesis generation.

## Introduction {.page_break_before}
### Background
Comprehensive data collections are indispensable for answering complex scientific questions. In health and medical research, the collection of electronic patient records together with multi-omics data (genomics, epigenomics, transcriptomics, proteomics, metabolomics, interactomics, pharmacogenomics, diseasomics) results in heterogeneous databases that can offer enormous potential for science due to the interconnections. By using data-mining methods based on machine learning methods and/or methods from artificial intelligence, statistical relationships in the data can be identified in a short period of time and new knowledge can be provided [Literature Sylvia]. These methods are suitable especially in difficult manageable heterogeneous data sets for a non-hypothesis-driven approach. At the same time, when it comes to specific questions, there is often a desire for a hypothesis-driven approach in which a targeted search is made for connections in the data which are not known yet.
With the currently dominant form of data storage in the form of relational databases with multiple tables connected via primary- and foreign keys connections, exploration and analysis are not always possible without further ado [].

Graph databases have proven that they can store and visualize complex connections between data elements, especially with heterogeneous data sets, and also show an advantage in terms of their general performance compared to currently prevailing database systems such as relational databases. Furthermore, graph database systems such as Neo4j provide extensive data interaction tools that can easily be expanded and thereby turn graphical databases into a storage-, exploration- and analysis tool for the entire data analysis process. In the present work, we demonstrate the use of graphic tools for exploration, analysis and visualization based on a publicly accessible database and compare it with procedures for relational data structures, especially for hypothesis-driven investigations. For this purpose, the relational data structure was transformed into a graphic structure and made explorable and analyzable using the tools provided by Neo4j.
### Objective and Requirements
Our objective of this work is to show the possibilities of a hypothesis-driven approach with Neo4j and the tools related to Neo4j in comparison to relational databases. All data used in this project has been imported into the Neo4j v1.3.8 graph database and a PostgreSQL Database. We are going to repeat some published results based on a graph database.

To perform data exploration we use Data explorer a tool made by yworks, which facilitates the exploration of the underlying data schema and the  exploration of relationships between specific Data types. 

With the present work we want to take a first step towards a data warehouse system based on a graph database and demonstrate the first integration of a clinical data set. We use Neo4j as a graph management system and integrate a relational data structure into a graph database model. We then use existing visualization interfaces based on Neo4j that can facilitate exploration.


## State ot the art
Aktuellen Datenanalyseprozess genauer skizzieren (von Rohdaten über Machine learning zu Schlussfolgerung). Einfluss des Wissenschaftlers und des Domainexperten anhand relationaler DBs. Nachteil, Datenstruktur muss vor der Exploration schon bekannt sein. Graphische Interaktionsmöglichkeiten durch neo4j als zusätzliche Interaktionsmöglichkeit darstellen

### Related Work
Data Warehouse Systeme zeigen den 
Reactome ect. darstellen. [Reactome graph database: Efficient access to complex pathway data](brain://Oc7_RTSOglu1Y7o1XiC1_w/ReactomeGraphDatabaseEfficientAccessToComplexPathwayData)
KC als Option. 

### Short commings
Verknüpfung zu Patientendaten als wichtige Unterscheidung einer reinen Strukturvisualisierung wie REACTOME. Abfragen der Patientendaten über mehrere Zugänge je nach ergänzter Strukturontologie z.B. SNOMED CT
Tableau und Limitationen eingehen. Man kommt nur mit Tableau nicht weiter. 

## Concept
Wege zum Umformen einer relationalen Datenbank in graphische DB am Beispiel der PRINCE Studie beschrieben. Alternative Wege dieser Umformung darstellen. Beispiel aus Paper mit MIMIC-III patient database [Can Neo4j Replace PostgreSQL in Healthcare?](brain://dHnZxITsAEy3yGTtdVz8KQ/CanNeo4jReplacePostgreSQLInHealthcare) Begründung für den einfachen mechanismus erklären. Aktuell gibt es noch kein sinnvolles Patientenmodell für Patientendaten (siehe : )[](brain://mkyTjg4g5lyRkczP6T2EtA/GraphRepresentationOfPatientDataASystematicLiteratureReview)Kritische Punkte beschreiben.

## Implementation
### Solution / Result

Datenbankmodell und relationaler Vergleich hierzu.
Überblick zur gesamten Datenstruktur und den Relationen hieraus. 
Bilder zur Darstellung des Neo4j- Interfaces.
Bilder zur Darstellung des Data Explorers von yWorks
Bilder zur Darstellung spezieller Explorationsmöglichkeiten z.B: k-Means Clustering, Shortest Path, Centrality
	
### System in Use

Potentiellen Nutzen und den aktuellen Aufbau beschreiben. 
	  
## Lesson learned
Intensiver Gebrauch des Workflows muss noch getestet werden. Weitere Interaktionsmöglichkeiten mit den Daten müssen herausgearbeitet werden.

## Conclusion
Neo4j kann neue Möglichkeiten in der Exploration von klinischen Daten liefern nicht nur auf Strukturebene, auch auf Rohdatenebene. Ergänzende Transformationen notwendig um die SQL ähnliche Berechnungen zu ergänzen. Mapping tool für die Abbildung auf Ontologien sinnvoll. Muss anhand größerer Datenbestände überprüft werden. Vielleicht als Konzeption für Data Warehouse, oder für klinische Anwendungen ähnlich den Knowlege  Connector
Declarations
References 






























# Formatierung

--- 
This manuscript is a template (aka "rootstock") for [Manubot](https://manubot.org/ "Manubot"), a tool for writing scholarly manuscripts.
Use this template as a starting point for your manuscript.

The rest of this document is a full list of formatting elements/features supported by Manubot.
Compare the input (`.md` files in the `/content` directory) to the output you see below.

## Basic formatting

**Bold** __text__

[Semi-bold text]{.semibold}

[Centered text]{.center}

[Right-aligned text]{.right}

*Italic* _text_

Combined *italics and __bold__*

~~Strikethrough~~

1. Ordered list item
2. Ordered list item
    a. Sub-item
    b. Sub-item
        i. Sub-sub-item
3. Ordered list item
    a. Sub-item

- List item
- List item
- List item

subscript: H~2~O is a liquid

superscript: 2^10^ is 1024.

[unicode superscripts](https://www.google.com/search?q=superscript+generator)⁰¹²³⁴⁵⁶⁷⁸⁹

[unicode subscripts](https://www.google.com/search?q=superscript+generator)₀₁₂₃₄₅₆₇₈₉

A long paragraph of text.
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

Putting each sentence on its own line has numerous benefits with regard to [editing](https://asciidoctor.org/docs/asciidoc-recommended-practices/#one-sentence-per-line) and [version control](https://rhodesmill.org/brandon/2012/one-sentence-per-line/).

Line break without starting a new paragraph by putting  
two spaces at end of line.

## Document organization

Document section headings:

# Heading 1

## Heading 2

### Heading 3

#### Heading 4

##### Heading 5

###### Heading 6

### A heading centered on its own printed page{.center .page_center}

<!-- an arbitrary comment. visible in input, but not visible in output. -->

Horizontal rule:

---

`Heading 1`'s are recommended to be reserved for the title of the manuscript.

`Heading 2`'s are recommended for broad sections such as *Abstract*, *Methods*, *Conclusion*, etc.

`Heading 3`'s and `Heading 4`'s are recommended for sub-sections.

## Links

Bare URL link: <https://manubot.org>

[Long link with lots of words and stuff and junk and bleep and blah and stuff and other stuff and more stuff yeah](https://manubot.org)

[Link with text](https://manubot.org)

[Link with hover text](https://manubot.org "Manubot Homepage")

[Link by reference][manubot homepage]

[Manubot Homepage]: https://manubot.org

## Citations

Citation by DOI [@doi:10.7554/eLife.32822].

Citation by PubMed Central ID [@pmc:PMC6103790].

Citation by PubMed ID [@pubmed:30718888].

Citation by Wikidata ID [@wikidata:Q56458321].

Citation by ISBN [@isbn:9780262517638].

Citation by URL [@https://greenelab.github.io/meta-review/].

Citation by alias [@deep-review].

Multiple citations can be put inside the same set of brackets [@doi:10.7554/eLife.32822; @deep-review; @isbn:9780262517638].
Manubot plugins provide easier, more convenient visualization of and navigation between citations [@doi:10.1371/journal.pcbi.1007128; @pubmed:30718888; @pmc:PMC6103790; @deep-review].

Citation tags (i.e. aliases) can be defined in their own paragraphs using Markdown's reference link syntax:

[@deep-review]: doi:10.1098/rsif.2017.0387

## Referencing figures, tables, equations

Figure @fig:square-image

Figure @fig:wide-image

Figure @fig:tall-image

Figure @fig:vector-image

Table @tbl:bowling-scores

Equation @eq:regular-equation

Equation @eq:long-equation

## Quotes and code

> Quoted text

> Quoted block of text
>
> Two roads diverged in a wood, and I—  
> I took the one less traveled by,  
> And that has made all the difference.

Code `in the middle` of normal text, aka `inline code`.

Code block with Python syntax highlighting:

```python
from manubot.cite.doi import expand_short_doi

def test_expand_short_doi():
    doi = expand_short_doi("10/c3bp")
    # a string too long to fit within page:
    assert doi == "10.25313/2524-2695-2018-3-vliyanie-enhansera-copia-i-insulyatora-gypsy-na-sintez-ernk-modifikatsii-hromatina-i-svyazyvanie-insulyatornyh-belkov-vtransfetsirovannyh-geneticheskih-konstruktsiyah"
```

Code block with no syntax highlighting:

```
Exporting HTML manuscript
Exporting DOCX manuscript
Exporting PDF manuscript
```

## Figures

![
**A square image at actual size and with a bottom caption.**
Loaded from the latest version of image on GitHub.
](https://github.com/manubot/resources/raw/15493970f8882fce22bef829619d3fb37a613ba5/test/square.png "Square image"){#fig:square-image}

![
**An image too wide to fit within page at full size.**
Loaded from a specific (hashed) version of the image on GitHub.
](https://github.com/manubot/resources/raw/15493970f8882fce22bef829619d3fb37a613ba5/test/wide.png "Wide image"){#fig:wide-image}

![
**A tall image with a specified height.**
Loaded from a specific (hashed) version of the image on GitHub.
](https://github.com/manubot/resources/raw/15493970f8882fce22bef829619d3fb37a613ba5/test/tall.png "Tall image"){#fig:tall-image height=3in}

![
**A vector `.svg` image loaded from GitHub.**
The parameter `sanitize=true` is necessary to properly load SVGs hosted via GitHub URLs.
White background specified to serve as a backdrop for transparent sections of the image.
](https://raw.githubusercontent.com/manubot/resources/main/test/vector.svg?sanitize=true "Vector image"){#fig:vector-image height=2.5in .white}

## Tables

| *Bowling Scores* | Jane          | John          | Alice         | Bob           |
|:-----------------|:-------------:|:-------------:|:-------------:|:-------------:|
| Game 1 | 150 | 187 | 210 | 105 |
| Game 2 |  98 | 202 | 197 | 102 |
| Game 3 | 123 | 180 | 238 | 134 |

Table: A table with a top caption and specified relative column widths.
{#tbl:bowling-scores}

|         | Digits 1-33                        | Digits 34-66                      | Digits 67-99                      | Ref.                                                        |
|:--------|:-----------------------------------|:----------------------------------|:----------------------------------|:------------------------------------------------------------|
| pi      | 3.14159265358979323846264338327950 | 288419716939937510582097494459230 | 781640628620899862803482534211706 | [`piday.org`](https://www.piday.org/million/)               |
| e       | 2.71828182845904523536028747135266 | 249775724709369995957496696762772 | 407663035354759457138217852516642 | [`nasa.gov`](https://apod.nasa.gov/htmltest/gifcity/e.2mil) |

Table: A table too wide to fit within page.
{#tbl:constant-digits}

|          | **Colors** <!-- $colspan="2" --> |                      |
|:--------:|:--------------------------------:|:--------------------:|
| **Size** | **Text Color**                   | **Background Color** |
| big      | blue                             | orange               |
| small    | black                            | white                |

Table: A table with merged cells using the `attributes` plugin.
{#tbl: merged-cells}

## Equations

A LaTeX equation:

$$\int_0^\infty e^{-x^2} dx=\frac{\sqrt{\pi}}{2}$$ {#eq:regular-equation}

An equation too long to fit within page:

$$x = a + b + c + d + e + f + g + h + i + j + k + l + m + n + o + p + q + r + s + t + u + v + w + x + y + z + 1 + 2 + 3 + 4 + 5 + 6 + 7 + 8 + 9$$ {#eq:long-equation}

## Special

<i class="fas fa-exclamation-triangle"></i> [WARNING]{.semibold} _The following features are only supported and intended for `.html` and `.pdf` exports._
_Journals are not likely to support them, and they may not display correctly when converted to other formats such as `.docx`._

[Link styled as a button](https://manubot.org "Manubot Homepage"){.button}

Adding arbitrary HTML attributes to an element using Pandoc's attribute syntax:

::: {#some_id_1 .some_class style="background: #ad1457; color: white; margin-left: 40px;" title="a paragraph of text" data-color="white" disabled="true"}
Manubot Manubot Manubot Manubot Manubot.
Manubot Manubot Manubot Manubot.
Manubot Manubot Manubot.
Manubot Manubot.
Manubot.
:::

Adding arbitrary HTML attributes to an element with the Manubot `attributes` plugin (more flexible than Pandoc's method in terms of which elements you can add attributes to):

Manubot Manubot Manubot Manubot Manubot.
Manubot Manubot Manubot Manubot.
Manubot Manubot Manubot.
Manubot Manubot.
Manubot.
<!-- $id="element_id" class="some_class" $style="color: #ad1457; margin-left: 40px;" $disabled="true" $title="a paragraph of text" $data-color="red" -->

Available background colors for text, images, code, banners, etc:  

`white`{.white}
`lightgrey`{.lightgrey}
`grey`{.grey}
`darkgrey`{.darkgrey}
`black`{.black}
`lightred`{.lightred}
`lightyellow`{.lightyellow}
`lightgreen`{.lightgreen}
`lightblue`{.lightblue}
`lightpurple`{.lightpurple}
`red`{.red}
`orange`{.orange}
`yellow`{.yellow}
`green`{.green}
`blue`{.blue}
`purple`{.purple}

Using the [Font Awesome](https://fontawesome.com/) icon set:

<!-- include the Font Awesome library, per: https://fontawesome.com/start -->
<link rel="stylesheet" href="https://use.fontawesome.com/releases/v5.7.2/css/all.css">

<i class="fas fa-check"></i> <i class="fas fa-question"></i> <i class="fas fa-star"></i> <i class="fas fa-bell"></i> <i class="fas fa-times-circle"></i> <i class="fas fa-ellipsis-h"></i>

[
<i class="fas fa-scroll fa-lg"></i> **Light Grey Banner**<br>
useful for *general information* - [manubot.org](https://manubot.org/)
]{.banner .lightgrey}

[
<i class="fas fa-info-circle fa-lg"></i> **Blue Banner**<br>
useful for *important information* - [manubot.org](https://manubot.org/)
]{.banner .lightblue}

[
<i class="fas fa-ban fa-lg"></i> **Light Red Banner**<br>
useful for *warnings* - [manubot.org](https://manubot.org/)
]{.banner .lightred}
