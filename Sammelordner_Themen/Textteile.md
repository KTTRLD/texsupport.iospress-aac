# Introduction
Umfangreiche Datensammlungen sind für die Beantwortung komplexer wissenschaftlicher Fragestellungen unverzichtbar. In der Gesundheits- und Medizinforschung entstehen aus der Sammlung elektronischer Patientenaktien zusammen mit multi-omics Daten (genomics, epigenomics, transcriptomics, proteomics, metabolomics, interactomics, pharmacogenomics, diseasomics) heterogene Datenbestände die durch die Verknüpfungen untereinander enormes Potential für die Wissenschaft bieten können. Durch die Anwendung von Data-Mining-Methoden, basierend auf maschinellen Lernmethoden und/ oder Methoden aus der künstlichen Intelligenz, können statistische Zusammenhänge in den Datenbeständen in kurzer Zeit identifizieren werden und neue Erkenntnisse liefern [Literatur Sylvia]. Diese Methoden eigenen sich vor allem bei schwer überschaubaren heterogenen Datenbeständen für einen nicht-hypothesengetriebenen Ansatz. Zugleich besteht bei spezifischen Fragestellungen oft auch der Wunsch nach einem hypothesengetriebenen Ansatz, bei dem gezielt nach Zusammenhängen in den Daten gesucht werden soll. Hier ist, bei der derzeit vorherrschenden Speicherung der Daten in Form von relationalen Datenbanken mit multiplen, über primary - und foreignkeys, zusammenhängende Tabellen, eine Exploration und Analyse nicht immer ohne weiteres möglich []. Graphische Datenbanken haben beweisen, dass sie gerade bei heterogenen Datensätzen zum einen komplexe Verbindungen zwischen Datenelementen speichern und visualisieren können und zum anderen im Vergleich zu aktuell Relationalen Datenbanken auch einen Vorteil bezüglich ihrer allgemeinen Performance zeigen. [literatur] Ferner liefern graphische Datenbanksysteme wie Neo4j umfangreiche Dateninteraktionswerkzeuge, die leicht erweitert werden können und dadurch graphische Datenbanken zu einem Speicher, Explorations- und Analysewerkzeug für den gesamten Datenanalyseprozess werden lassen. In der vorliegenden Arbeit möchten wir anhand einer öffentlich zugänglichen Datenbasis den Nutzen von graphischen Tools für die Exploration, Analyse und Visualisierung untersuchen und mit Vorgehen bei relationalen Datenstrukturen vorallem bei hypothesengetriebnen Untersuchung vergleichen. Hierfür wurde ein Transformation der relational vorliegenden Datenstruktur in eine graphische Struktur vorgenommen und mittels der von Neo4j bereitgestellten Tools explorierbar und analysierbar gemacht. 

Hypothesengetriebene Analysen, zeichnen sich häufig durch die Notwendigkeit aus 


Methoden und Tools um Hpothesengenerierung und Entscheidungsfindung aus komplexen heterogenen Daten zu erleichtern werden immer wichtiger. Dabei wurde Data Visualisierung und Visuelle Analyse als eine Möglichkeit angesehen die

Visualisierungs und Visuelle Anlysetools sind schwer zu evaluieren

%%%%%%%%%%%%%%%%%%%% 1.2. Objective and Requirements %%%%%%%%%%%%%%%%%%%%%%%%%%%%%%55555


We test the use of already established tools based on the Neo4j ecosystem on a hypothesis-driven investigation to allow users to easily examine the data and the underlying data structure in compersion to currently used relational databases. 



We developed such a system based on graph based tool that allows users to easily examine available data and to extract required subsets of the data. therfore we .

In the present work, our objectiv is to use graph database tools for exploration, analysiation and visualization of a publicly accessible database and compare it with procedures for relational data structures, especially for hypothesis-driven investigations. 

A key demand on this approach is to give the user the abbility to of the underlying data structure and 

Our objective of this work is to show the possibilities of a hypothesis-driven approach with Neo4j and the tools related to Neo4j in comparison to relational databases. All data used in this project has been imported into the Neo4j v1.3.8 graph database and a PostgreSQL Database. We are going to repeat some published results based on a graph database.

To perform data exploration we use Data explorer a tool made by yworks, which facilitates the exploration of the underlying data schema and the  exploration of relationships between specific Data types. 


####################### MIMIC %%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%5

The Medical Information Mart for Intensive Care (MIMIC) is a large database (DB)
containing data of patients who were treated at intensive care units of the Beth Israel Deaconess Medical Center (Boston, Massachusetts, USA). The full database underwent an automatic de-identification to protect patients’ privacy. As full anonymity cannot be guaranteed, researchers who want to use the data have to pass an online course and accept a data use agreement before they are granted access by the curators [1].
However, there is no further restriction on the usage, which makes the database a
valuable source for reproducible data-driven studies in the biomedical domain.
The third version MIMIC III comprises clinical measurements, administrative
information, laboratory test results, (pharmacological) therapy descriptions, and
caregiver notes related to more than 40 000 patients [1]. During the generation process between 2001 and 2012, (electronic) medical records and accounting documents as well as free texts were compiled into this database. file:///C:/Users/k538d/Downloads/SHTI-267-SHTI190817.pdf