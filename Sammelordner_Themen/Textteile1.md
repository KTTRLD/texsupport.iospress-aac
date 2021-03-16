#################################################################Gedanken######################################

Researchers are often used to find their data in many distributed tables in the form of rows and columns. In relational databases, for instance, the information is linked across multiple tables by unique identifiers and the relationship between data values is only implicitly apparent. By modelling relationships between data types- or values, graph databases have been used successfully in recent years to represent complex, inhomogeneous data. Furthermore, the exploration of the underlying data structure and the data itself is intuitively possible with graph databases. Neo4j as an example of a graph database system can be adapted in many ways with the help of interactive tools to provide a new way of data exploration and analysis. In the present work, we examine the benefit of graph databases as an exploratory and analytic tool for clinical data. In collaboration with domain experts in Obstetrics and Fetal Medicine, we demonstrate how this resource can improve the efficiency and comprehensiveness of hypothesis generation.

1. Introduction
1.1. Background

3. Implementation

Neo4j mas graph database use labeled 
#####################################################################################################################




### Big Data und nutzen für die Gesellschaft

> Für die Wissenschaft besitzen große Datensammlungen ein enormes Potenzial zur Beantwortung komplexer Fragestellungen. Die langfristigen Auswirkungen von Ereignissen wie Lärmbelastungen oder eines geringen sozioökonomischen Status in unterschiedlichen Altersstadien auf die Gesundheit im gesamten Lebensverlauf oder die Zusammenhänge zwischen Lebensstil, Genetik und dem Auftreten von Krankheiten wie Demenz oder Krebs sind hier nur zwei von vielen Beispielen. Aus den gewonnenen Ergebnissen lassen sich dann Handlungsempfehlungen und Leitlinien ableiten, die einen direkten Nutzen für die Bevölkerung und das sie behandelnde medizinische Fachpersonal haben. Gleichzeitig ebnen große Datensammlungen den Weg zu einer personalisierten und selbstbestimmteren medizinischen Versorgung. Mithilfe moderner Medien sind die Menschen in der Lage, ihren Gesundheitszustand eigenständig zu kontrollieren. Dabei könnten z. B. individuelle Grenzwerte für Blutdruck oder Blutzucker festgelegt werden. [Pigeot et al.](https://link.springer.com/article/10.1007%2Fs00103-015-2194-6)


### Big Data und drei "V"

Big Data wird in der Fachliteratur häufig mit den sogenannten drei „V“ in Verbindung gesetzt: große Datenmengen (Volume), die kaum oder sehr heterogen strukturiert vorliegen (Variety) und die mithilfe mathematisch-statistischer Verfahren und Optimierungsalgorithmen möglichst flexibel und in Echtzeit verarbeitet werden (Velocity). Big Data bezieht sich damit nicht nur auf große Datensammlungen, sondern ebenso auf die angewendeten Auswertungsmethoden, die grundsätzlich nicht hypothesengetrieben sind. 



## DWH
A data warehouse (DWH) is a complex system that is intended to facilitate the storage and exploration of large amounts of data from multiple sources. Data warehouse (DWH) systems are suitable for the scientific analysis of this clinical data. 

In the present work, we propose a graph-based approach of a DWH to demonstrate the potential benefit of this approach. In collaboration with domain experts in Obstetrics and Fetal Medicine, we demonstrate how this resource can improve the efficiency and comprehensiveness of hypothesis generation. A graph-based approach seems promising for the design of a data warehouse, but the real value of this concept must be continuously evaluated by continuing the work shown. 

\section{DWH erleichterte Datenanalyse}
> The integration and mapping of heterogeneous data sources is an important first step affecting all subsequent analyses for studies in scientific disciplines. The development of the BioDWH2 tool is intended to ease and simplify this process for researchers and to be usable with limited to no programming skills. The hope is that future research projects can focus more quickly on the analysis instead of integration problems using only the specified data sources needed. [Marcel Friedrichs](https://www.degruyter.com/document/doi/10.1515/jib-2020-0033/html)

\section{Nutzen von Data Warehouse}
>This growth in OMICS fields and data sources necessitates research projects to have a reliable and easy to use integration pipeline for data warehousing and information mapping. Additionally, data sources are heterogeneous in format and availability and have a specific focus to which the format is tailored to. A uniform integration process into a singular data format is therefore beneficial. Another issue is the loose coupling of data sources. Identification systems and external references for entities are included in data sources but can’t guarantee that the referenced data sources will not change. Strong mapping of entities in a data warehouse by introducing a mapping layer and connecting entities from different data sources is another important step. Bringing large amounts of data together helps researchers focus on the analyses they want to perform in one place. [Marcel Friedrichs](https://www.degruyter.com/document/doi/10.1515/jib-2020-0033/html)

\subsubsection{Warehouse mit relationalen DBvs graph Data}

The architecture of a data warehouse can differ depending on the application scenarios. Regardless of the architecture, there are components that should be present in a data warehouse system:
•	ETL Component: ETL stands for Extract, Transform, and Load. The staging layer uses ETL tools to extract the needed data from various formats and checks the quality before loading it into the data warehouse. The data coming from the data source layer can come in a variety of formats. Before merging all the data collected from multiple sources into a single database, the system must clean and organize the information.
•	Data storage component: The most crucial component and the heart of each architecture is the database. The warehouse is where the data is stored and accessed. When creating the data warehouse system, you first need to decide what kind of database you want to use. The most dominant form is the relational Database
•	Data Model: The necessary integration of different classes of heterogeneous information in a higher-level, connecting data model is a decisive step in the conception of a data warehouse and one of the decisive factors for the later usability of the system.
•	Data analysis component: Users interact with the gathered information through different tools and technologies. They can analyze the data, gather insight, and create new hypothesis.

\subsubsection{Analysemöglichkeiten für DWH}

- Kohortenselektion
- Kohortenorientierte Analyse
	- Laborverlauf
	- molekulare Befunde
- Kohortenvergleich
	- Kaplan - Meier
	- Patientenliste mit unterschiedlichen 
- Patientenorientierte Analyse
	- Patient Timeline
		- Diagnose
		- Diagnostik
			- Labordiagnostik
			- Apperative Diagnostik
		- Verlegungen
		- Apperative Therapien
		- Medikation
	- Genanalyse
- Patientenvergleich

> "kohortenbasierte Analysen durch Filterung und Kombination von logischen Operatoren (UND / ODER / NICHT) über alle enthaltenen Parameter durchzuführen und die entstehenden Kohorten als Balkendiagramm, Boxplot, Kaplan-Meier-Diagramm, im Genome Browser oder in einer Patientenliste zu visualisieren.Absolute und relative zeitliche Bezüge zwischen einzelnen Datenelementen stellen einen wesentlichen Aspekt bei der Analyse klinisch relevanter Datensätze dar. Beide Ansätze werden von MRI unterstützt. "(DTH- Routinepilot Abschlussbereicht)



\subsection{EHR}

### Electronic Helath records
In the medical field, a wealth of semantically similar clinical data has been collected through the dissemination of electronic health records (EHR).

\subsection{Graph Database}

\subsection{Graphische Datenbanken Nutzen}

In recent years graph databases have demonstrated that they can be used for storing and exploring complex interrelated data in many areas of application. 

> With the increasing and widespread use of graph databases [12], [13], [14], using a relational database for large data warehouses may not be best suited anymore. Especially for an additional mapping layer, the analysis of relational tables with joining queries will become very slow and sometimes unfeasible [15]. While graph databases can outperform relational databases, they also provide the opportunity to reveal novel relationships in heterogeneous data [12]. [Marcel Friedrichs](https://www.degruyter.com/document/doi/10.1515/jib-2020-0033/html)


Graphische Datenbanken haben beweisen, dass sie gerade bei heterogenen Datensätzen zum einen komplexe Verbindungen zwischen Datenelementen speichern und visualisieren können und zum anderen im Vergleich zu aktuell noch vorherrschenden Datenbanksystemen wie Relationalen Datenbanken auch einen Vorteil bezüglich ihrer allgemeinen Performance zeigen. Ferner liefern graphische Datenbanksysteme wie Neo4j umfangreiche Dateninteraktionswerkzeuge, die leicht erweitert werden können und dadurch graphische Datenbanken zu einem Speicher, Explorations- und Analysewerkzeug für den gesamten Datenanalyseprozess werden lassen. Das Konzept der Relationale Datenbanksysteme ist hier enger gedacht und umfasst hauptsächlich die Speicherung und das Datenmanagement in diesem Prozess. Die Aufbereitung, Exploration und Visualisierung verteilt sich hier auf unterschiedliche Teillösungen die sich je nach Präferenz der Nutzer oder den allgemeinen Anforderungen des Fachgebiets unterscheiden können und eine Wiederholung von Forschungsergebnissen von der Vertrautheit mit den Werkzeugen abhängig machen können.  

Der Datenanalyse Prozess der für jeden wissenschaftlich Tätigen und für jede Fachdisziplin individuell unterschiedlich ist setzt aus folgenden generellen Teil abschnitten zusammen, die vom verwendeten Werkzeug zunächst unabhängig sind.  

- Data collection
- Data storage
- Data analytics
- Data reporting and visualization


- Datenspeicherung bzw. Datenmnagement
- Datentransformation
- Datenexploration
- Datenanalyse

In der vorliegenden Arbeit möchten wir an einem konkreten klinischen Datensatz zeigen, dass graphische Datenbanken den gesamten Prozess der Analysen beeinflussen können und die Generierung von Hypothesen bereits durch die Nutzung und Interaktion mit einem graphischen Datenbanksystem ermöglicht wird.


\subsection{Datenanalyse}

### Wie laufen Datenanalysen ab
Raw Data -> 
 
### DWH

Große Datensammlungen sind für die Wissenschaft zur Beantwortung komplexer Fragestellungen sehr wertvoll und besitzen ein großes Potenzial
Graphische Datenbanken konnten in den letzten Jahren demonstrieren, dass sie sich zur Speicherung und Exploration komplexer Daten in vielen Anwendungsbereichen eignen können. Im medizinischen Bereich konnte durch die Verbreitung von electronic health records (EHR) eine fülle von semantisch ähnlichen klinischen Daten gesammelt werden. 
Für die wissenschaftliche Analyse dieser klinischen Daten eignen sich Data warehouse Systeme. In der vorliegenden Arbeit möchten wir die Eigenschaften von Graphischen Datenbanken in einen exemplarischen Data Warehouse Kontext überprüfen.

Ein data warehouse bietet die integrierten Daten, strukturiert und aufbereitet in einem einheitlichen Format zur domainspezifischen Datenanlyse und Exploration an. In der vorliegenden Arbeit wird ein Data Warehouse Ansatz basierend auf einer graphischen Datenbank eingesetzt um die Machbarkeit und 

 sodass sich die Anwender auf die Analyse der Daten fokussieren können.


Ein Data Warehouse stellt eine Plattform dar, welches die Speicherung und die Exploration großer Datenmengen durch spezielle Werkzeuge für eine möglichst große Anwendergruppe erleichtern soll. Wir sind der Meinung, dass graphische Datenbanken zum einen die Speicherung großer Datenmengen als auch die Exploration dieser Daten erleichtert und die Nutzbarkeit und Akzeptanz von Data Warehouses erhöhen k. 

### Daten Model DWH
Die hierzu notwendige Integration unterschiedlicher Klassen heterogener Informationen in ein übergeordnetes verbindendes Datenmodell ist ein entscheidender Schritt in der Konzeption eines Data Warehouses und mitentscheidend für die spätere Nutzbarkeit des Systems. Erfahrungsgemäß sollte ein Datenmodell im Bereich der Medizin oder im Bereich der Naturwissenschaften flexibel und leicht erweiterbar sein. Gleichzeitig sollte das erstellte Datenmodell alle semantischen Informationen der zugrundeliegenden Quellsysteme einschließen ansonsten sind diese für den Anwender in der Exploration nur schwer zu finden und reduzieren das Vertrauen in das System und erschweren die potentielle Nutzbarkeit. 
Anwender sollten einen intuitiven Überblick über das zugrundeliegenden Datenmodell haben um die gewünschten Abfragen optimal zu wählen. In den letzten Jahren zeigte sich, dass speziell graphische Datenbanken sowohl in der Speicherung als auch in der Datenexploration von komplexen zusammenhängenden Daten gut geeignet sein könnten. Mit der vorliegenden Arbeit zeigen wir eine mögliche Realisierung einer Explorationskomponente die für eine Data Warehouse genutzt werden soll und auf einer graphischen Datenbanken basiert. Wir versprechen uns dadurch eine größerer Nutzbarkeit und Akzeptanz des Data Warehouse. Ferner ist die Bereitschaft eigene Datenbestände in einen größeren Kontext einzuordnen.

### Objective and Requirements
Die Exploration von komplexen Daten wird durch das Verständnis der Datenstruktur erleichtert. Relationale Datenbanken basieren auf Verbindungen 
Personen mit Domainwissen bekommen leichteren Zugang zur Datenexploration. Können Hypothesen generieren und Selektionen von Kohorten erleichtern. Kann basis für ein Data Warehouse sein. 
Systemvoraussetzungen der DB. Wie aufgesetzt. Data-Explorer von yworks beschreiben. Vielleicht Tableau als ergänzendes Visualisierungstool beschreiben.


## Conclusion
Wir konnten zeigen, dass sich Graphische Datenbanken in einem Data Warehouse Ansatz in die Datenhaltung, Datenintegration und Datenvisualisierung eingliedern lassen und einen Nutzen für eine breite Anwendergruppe von Domainexperten bringen kann. In weiteren Schritten ist geplant das Data Warehouse für eine große Klinik bereitzustellen und schrittweise zu erweitern.


## Strukturexploration vs Dataexploration
Es soll nicht um die Strukturexploration (anders als [bei )sondern](brain://jhnfj16cFEqSPIMMZN928w/HetionetAnIntegrativeNetworkOfBiomedicalKnowledge) um eine Alternative zur Datenexploration mithilfe von graphischen Datenbanken gehen. Es soll eine schnelle Transformation in eine Graphische Datenbank möglich sein, die dann anschließend visuell exploriert werden kann. Daten werden mit Script in horizontale und vertikale Relationen übersetzt und anschließend mit vorhanden neo4j tools exploriert. Es ist wenig prozessorientiert Kenntnis notwendig und kann ähnlich wie eine Strukturexploration dienen die Daten zu erkunden un



# Einleitung Forschung

Möglichkeiten eine graphische Datenstruktur zu explodieren und dadurch Zusammenhänge explizit ersichtlich zu machen. Durch die Möglichkeit die Interaktion mit Neo4j über spezifische interaktive Werkzeuge zu erweitern könnte  spezielle interaktive Oberflächen ermöglichen es auch ungeübten Nutzern mit der Daten zu interagieren und relevante Zusammenhänge explizit zu erforschen. 

# Graphdata und Neo4j und die Tools




## Test_Introduction
In the medical field, a wealth of semantically similar clinical data has been collected through the dissemination of electronic health records (EHR). 

Die meisten dieser Daten liegen vermutlich in relationalen Datenbanken wie beispielsweise in PostgreSQL und MySQL Datenbanken.



rekonstruierbar. In dieser Struktur zusammenhänge zu erkennen gelingt häufig nach intensicer Ausseinandersetzung und kann sehr zeitaufwendig sein. Graphische Datenbanken eigenen sich Verknüpfungen zwischen Datentypen zu visualisieren und damit explizit der Einzelnen Einheiten häufig  für relationale Datenbanken üblich ist. 

verbunden und müssen für eine spezielle Untersuchung aufbereitet und  Um eine tiefere Analyse durchzuführen zu können und Zusammenhänge zu erkennen, die implizit in den Daten verborgen sind ist die Kenntnis der allgemeinen Datenstruktur notwendig. Die

Die Verknüpfung der einzelner Tabellen erfolgt beispielsweise in relationalen Datenbank architekturen über primary und foreign keys. Um neue Zusammenhänge zu erkennen ist eine Kenntnis der Datenstrukturen und der Datentypen notwendig. Graphische   liegt hierbei in  Die dabei verwendeten Werkzeuge  In dieser Form der Darstellung werde


#####################################################################################################################

## Welche möglichkeiten gibt es für Data analytics
### Data analytics

- Visual Analytics
- Statistical Analytics
	- Regression Analysis:
	It is a statistical tool for investigating the relationship between variables [Artikel](https://www.digitalvidya.com/blog/data-analytics-tools/)

	- Correlation Analysis:
	A statistical technique that allows you to determine whether there is a relationship between two separate variables and how strong that relationship may be. It is best to use when you know or suspect that there is a relationship between two variables and wish to test the assumption.[Artikel](https://www.digitalvidya.com/blog/data-analytics-tools/)

- Time Series Analysis:
	It is the data that is collected at uniformly spaced time intervals. You can use it when you want to assess changes over time or predict future events on the basis of what happened in the past. [Artikel](https://www.digitalvidya.com/blog/data-analytics-tools/)

#####################################################################################################################

\chapter{Ideen}
Datenvisualisierung, Exploration und Analyse von klinischen Daten mit Neo4j Tools am Beispiel einer klinischen Studie.

- Nachbauen von publizierten Analysen mit graphischen DBs
- welche schritte können mit Neo4j nicht neo4j abgedeckt werden?

- reicht graphische Datenvisualisierung um gesamte Datenanalyse zu modellieren mit den vorhandenen Tools um Zusammenhänge aus Daten schneller zu erkennen.
- Strukturexploration an vielen Beispielen bekannt. Einfaches Datenmodell abgeleitet von relationaler Struktur durch Umwandlung der Spalten in Typen und Zeilen in Pfade.
Funktioniert das? am Beispiel PRINCE. 

######
Big Data stellt eine große unstrukturierte Menge heterogener Daten da, die für die zielgerichtete Suche nach Erkenntnissen oft nur aufwendig zugänglich ist. Methoden des Data Minings stellen statistische Zusammenhänge zwischen zwischen Daten her. Eine hypothesengetriebene Forschung mit relationalen Datensätzen ist zeitaufwendig und nicht immer umsetztbar. Graphische Datenbanken wie beispielsweise Neo4j können zusammenhänge visualisieren und explorierbar machen, dadurch kann für den Anwender eine hypothesengetriebene Analyse möglich werden. Hypothesengetriebe Fragestellungen zielen häufig daurauf ab einen unterschied zwischen einer begrentzen Anzahl klar definierter Kohorten bzgl. interessanter Zielvariablen zu untersuchen. Dies könnte mit de

Wir möchten testen, ob die Transformation von großen relationalen Datenstrukturen mit Hilfe von graphischen Datenbanken in explorierbare Datensätze einen Mehrwert für die Anwender bilden kann. 




### Hypothesengetrieben vs. Nicht-Hypothesengetrieben
-  Hypothesengetriebene Ansätze: --> Wir wollen das an den Daten testen, geht das oder haben wir zu wenig material eher nicht -> Damit unterscheidet sich Big Data von groß angelegten Forschungsdatenbanken, die Daten, in der Regel strukturiert und qualitätsgeprüft, als Basis hypothesengetriebener Forschung bereitstellen.

- Nicht-Hypothesengetrieben Ansätze --> Data-Mining Methoden, die in möglichst kurzer Zeit Korrelationen, also Zusammenhang, in Datenbeständen identifizieren. -> eher ausgeführt auf unterschiedliche, nicht grundsätzlich qualitätsgeprüfte Quellsysteme


### Typen von Datensammlungen

Big-Data: eher ausgeführt auf unterschiedliche, nicht grundsätzlich qualitätsgeprüfte Quellsysteme

Forschung: Damit unterscheidet sich Big Data von groß angelegten Forschungsdatenbanken, die Daten, in der Regel strukturiert und qualitätsgeprüft, als Basis hypothesengetriebener Forschung bereitstellen.

Zwischen diesen beiden Extremen liegen große Datenbanken, die nicht primär zu Forschungszwecken angelegt werden, wie etwa Abrechnungsdaten der Krankenversicherungen, die aber dennoch ein großes Potenzial für die Forschung bieten.

#####################################################################################################################
\
\chapter{To DO}
 - Klärung yworks und Speicherung der Daten auf Server, falls öffentliche daten dann erstmal egal
 - Mapping PRINCE auf Ontologie SNOMEDCT/Datenstruktur von Het.io
 
 
Markus Scheller Travelmangement
Genehmigter Dienstreiseesteller
040 7410 54251

#####################################################################################################################

\chapter{Unklare Zuordnung}
Data Warehouse als Basis für Data Analysen. Mit diesem System wollen wir ein konzept für ein Data Warehouse vorstellen, welches auf Graphischen Datenbanken basiert und die Vorteile der Flexiblen Erweiterungen 


In addition to experience and domain knowledge, the analysis of complex, heterogeneous data sets also requires the targeted use of special tools that support the entire process of statistical data preparation and analysis. As experience has shown that every scientist and every discipline uses an individual set of statistical tools, depending on their own experience and preferences, in order to extract valid, reliable, complete and reusable information from semi-structured raw data. 


Even with experienced data experts and scientists, the entire process has a high temporal impact.

Die Analyse komplexer heterogener Datenbestände erfordert neben Erfahrung und Domainkenntnis zusätzlich den gezielten Einsatz spezieller Tools die den gesamten Prozess der statistischen Datenaufbereitung und- Analyse unterstützen. Erfahrungsgemäß nutzt jeder Wissenschaftler und jede Fachdisziplin in Abhängigkeit der eigenen Erfahrungen und Präferenzen einen individuellen Satz an statistischen Werkzeugen um aus semi-strukturierten Rohdaten valide, verlässliche, vollständige und wiederverwendbare Informationen zu extrahieren. Der gesamte Prozess hat selbst bei erfahrenen Datenexperten und Wissenschaftlern einen hohen zeitlichen Einfluss. 

Die zusätzliche Integration eines einzelnen Datensatzes in einen weiteren Datensatz erschwert den Prozess noch weiter.

Ein Data Warehouse kann in diesem Zusammenhang idealerweise diesen Prozess beschleunigen und den Fokus der Analyse auf die Generierung und Überprüfung von Wissen legen. Hierdurch besteht die Hoffnung eine größere Nutzergruppe mit qualitativ hochwertigem Datenmaterial zu versorgen und die domainspezifische Hypothesenbildung zu erleichtern um auf diesem Weg einen Mehrwert aus den Daten zu erzeugen. In einem Data Warehouse, werden die Aspekte der Datenhaltung, Datenkorrektheit, Datenintegration sowie die regelmäßige Aktualisierung vom Endnutzer abstrahiert und in Form einer explorierbaren Datenbasis zur Verfügung gestellt. 


Mit der vorliegenden Arbeit möchten wir einen ersten Schritt in Richtung eines auf graphischen Datenbanken basierenden Data Warehouse Systems legen und eine erste Integration eines klinischen Datensatzes demonstrieren. Wir verwenden hierzu Neo4j als Graphisches Management System und integrieren eine relationale Datenstruktur in ein Graphisches Datenbank Model. Im Anschluss nutzen wir bereits vorhandene Visualisierungsoberflächen, welche die Exploration erleichtern können.


Das Resultat sind auf den Datensatz spezifische  um den eigenen Datenbestand nach relevanten Zusammenhängen zu untersuchen und auf diesem Weg neuen Hypothesen zu generieren und neues Wissen zu erzeugen. 
So sind Statistikprogramme wie SPSS, SAS, GraphPad PRISM und viele weitere, ebenso wie höhere Programmiersprachen wie R oder Python bei der statistischen Datenanalyse nicht wegzudenken. Gleichzeitig werden auch Softwareprodukte wie Knime oder Tableau bei wiederkehrenden Analysen oder als Monitoringinstrument eingesetzt und helfen bei der visualisieren wiederkehrender Fragestellungen [Literatur Tableau und Knime](https://pubmed.ncbi.nlm.nih.gov/29777325/). Ebenso weit verbreitet sind maschinelle Lernverfahren und Methoden der künstlicher Intelligent in der Datenanalyse und Wissensgenerierung die speziell bei großen Datenmengen einen Mehrwert liefern. 

Der Ansatz einer Data Warehouses Plattform ist es, den gesamten skizzierten Prozess von der Datenhaltung über die Datenaufbereitung bis hin zur Datenexploration - und analyse zu abstrahieren und für eine möglichst breite Nutzergruppe anzubieten. Dies soll zu einer Beschleunigung wiederkehrender Analyseabläufe führen und die eigentliche Wissensgenerierung aus den Daten in den Fokus stellen. 

Gleichzeitig kann eine Abstraktion der Abläufe auch dazu führen das erfahrene Nutzergruppen die Nutzbarkeit des Systems als gering einschätzen, da bekannte Funktionen für die erweiterte Datenanalyse fehlen oder anders implementiert sind. 
Ein Data Warehouse sollte damit die grundlegende Funktionalität der etablierten Tools anbieten und gleichzeitig eine potentielle Erweiterbarkeit zur Verfügung stellen.

Unsere Konzeption eines Data Warehouse umfasst folgende Basis Componenten:
- 
- Datenintegration (Übersetzung der Quellsystem Daten in Zielontologie)
- Datapreparation
- Daten- und Strukturexploration
- Datenanalyse mit Datentransformation bzw. Datenerweiterung
- Data and Datastructur Exploration
- Data Visualisierung


Mit dieser Arbeit möchten wir den Einsatz von graphischen Datenbanken und ihren Nutzen als Speicher und Explorationswerkzeug für die Datenexploration untersuchen. Wir glauben, dass graphische Datenbanken das potential bieten den Datenanalyse Prozess zu erleichtern und im Rahmen eines Data Warehouse Projekts zu nutzen.   

Gleichzeitig kann ein Zugang zum Datenpool einer breiteren Nutzergruppe angeboten werden, wodurch die Wissensgenerierung und 


Datenvielfalt und Menge der Daten nimmt zu. Gleichzeitig auch Schwierigkeit dies zu überblicken und sinnvolle Schlüsse zu ziehen. Machine learning kann statistische Korrelationen aufzeigen und unterstützen, jedoch nicht ohne Domain Experten möglich. Graphische Daten liefern zusätzlich Einblicke. Dargestellte Arbeit soll dies unterstreichen.
Aktuellen Datenanalyseprozess skizzieren. Relationale Datenbanken mit Vor\- und Nachteilen beschreiben. Neo4j im Vergleich beschrieben. Beschreibung von Graph Apps als Interaktionsmöglichkeit, Starke Communitiy. Anwendungsgebiete von Neo4j am Beispiel Systembiologie (Reactome), Biologie und Medizin. Fokus auf Relationen der Daten hervorheben. Mit graphischen Datenbanken, können Ontologien ergänzt werden. Graphische Algorithmen sind bereits effizient beschrieben. Können mit Beschreibungslogiken zu Knowlege base ausgebaut werden. Automatisches Schließen möglich.  Unterstützung in der Entscheidungsfindung bei ausreichend großen Daten.
PRINCE Studie und Daten beschrieben. Datenmodell mit Studienzielen grob skizzieren

\chapter{Alles Andere}
Abstract
A Data Warehouse is a system of tools, that collects and combines multiple heterogeneous data and presents them in a comprehensive form to users. The ability to interact and explore this data collection may 



This data collection of big data enables the may lead to new insights and a new hypothesis.  In order to combine and merge multiple data types and sources into one big data source, the conception of a general data model that compromises all semantic aspects of the multiple data sources is an important and complex part of warehouse development. 

The general data model of the Data Warehouse provides the foundation of data interoperability and needs to be compressive and also complete so that every piece of information is easy to find and represented by the model. Every aspect that is captured by the general data model can be queried and accessed by the user. In order to address the right questions to the system, the structure of the data model needs to be present in the head of the users. Often it is also necessary to  



The underling semantic needs to In order to include every data type of the source data set

needed. This general data model might be slightly different from the initial data and implements a new terminology that 

 and needs to be created and necessary This kind of system is a useful tool to for users like researches who want to access the data and do there analysis 

Storing data in multiple tables and connecting these data via multiple-join statements is in most cases the predominant way to start the data analysis process. This approach might sufficient as long as you are familiar with the database schema, but 

Graph databases are getting more and more relevant for storing complex data and their relationships in different fields like medicine or biology. [PROTEOM, Hetionet]. Graph databases like neo4j already demonstrated their power by connecting heterogeneous data in a graph database [Hetionet] and an increasing number of projects starts connecting their data with graph databases. 
In contrast to, currently dominant relational databases like PostgreSQL or MySQL, graph databases are more focused on the connection between the data values and their data types. In addition to the storing function, which makes graphical databases interesting on their own, data exploration is another great opportunity, which graph databases like Neo4j may offer to their users. Furthermore, the great Neo4j community and their already implemented tools make Neo4j even more useful in the sense of exploring patient and clinical data sources. The following work suggests a simple workflow that may empower domain experts to explore their data visually and leverage connection in data to discover new hypothesises or new structures in their data which might be hidden in the table format.


Graph databases already demonstrated their power by connecting heterogeneous data in a graph database. Reactome for instance is a database collecting 

Introduction
The amount and complexity of data in the health industry are constantly raising. Every day a large volume of heterogeneous data is produced by electronic health records. The data compromise many different aspects of the health sector (from physical activities to laboratory tests, and from clinical diagnostics to insurance coverage).


 large More and more data is produced by the routine work of Even complex data is already represented in graphical 
Traditionally data is represented in tabular format for instance in a SQL based database like PostgreSQL. Here the connection between data is made by primary and foreign keys on every table. To analyse the structure of the data you 

Every day, the health industry is producing a large volume of heterogeneous clinical data. Different data types like clinical examinations, laboratory tests, apperativ diagnostics and even insurance data are stored by electronic health records. This amount of data gives us the opportunity to investigate questions and find answers by interpreting the underlying data. In order to make the best use of the data, we need analytic tools to explore these big datasets. Most of the data is stored in relational databases like PostgreSQL or MySQL databases.



The data compromise many different aspects of the health sector (from physical activities to laboratory tests, and from clinical diagnostics to insurance coverage). All of these 

Neo4 j structure
In this work, we used Neo4j as a graph database management system to store and analyze a data set collected from a prospectively designed, longitudinal population-based cohort study called PRINCE study (PRenatal DetermINants of Children’s HEalth). The data was collected from 2010 till now.
A graph is based on two components. The first component is a node with optional properties and optional labels. The second component is a directed relationship or edge with optional properties. Relationships have exactly one start and end node. The start and the end node may be the same node. With these components, it is possible to model complex interactions and relations between data objects. In mathematics, graph theory is used to model structures 

1.2 1 Objective and Requirements
The medical field is based on empirical information. Guidlines statements contain recommendations that are based on evidence from a rigorous systematic review and synthesis of the published medical literature.

Guidelines provided by comites 
A Data Warehouses (DW) for instance connect different data sources together and need to provide every contributor access to the expanded version of his data.  In most cases, the user of the DW wants to query an expanded version of his data. For instance, if someone whats to scan the data for a specific diagnosis or therapy the 

Before a user of Data Warehouses needs to understand the structure of the underlying data to perform well-suited queries and ask the right questions. 

Data
We used clinical data collected from a prospectively designed, longitudinal population-based cohort, the PRINCE study (PRenatal DetermINants of Children’s HEalth). The data was collected from 2010 till now.

Ziel: 

Clinical Data is complex, redundant and semi-structured.
Electronic health records traditionally store clinical data in tabular format in relational database architecture. 
This well-establish process has many advantages like many tools 

Relational Databases need the construct of primary keys and foreign keys to connect the information par

Non-primarily technical user groups like physicians have a lot of domain knowledge but not necessarily the opportunity to analyse data like a data scientist. 
The amount of data is steadily increasing and it is more and more important to link different sources semantically together. 



With this paper, we demonstrate a potential data analytics workflow based on a graph database with the aim to provide an additional way to explore complex heterogeneous data.

Our aim with this work is to create a workflow based on a graph database.

a non-primarily technical user group with an instance of a graph database and Tableau. We used clinical data collected from a prospectively designed, longitudinal population-based cohort, the PRINCE study (PRenatal DetermINants of Children’s HEalth)

Graph databases like neo4j, together with the developed applications for this graph database instance and a broad community offers a big opportunity to develop a visual exploratory toolset for complex data in a new and efficient manner. Data Warehouses for instance need a way to provide the data structure and the underlying metadata to increase the understanding of the data. Ony with an initial understanding of the underlying data structure, the generation of hypothesis or the systematical exploration of the data can be achieved. The representation of data in a tabular format is of 
 


 in comparison to relational databases. In the field of medicine data 





Neo4j as an example of a graph database (graph DB) instance already demonstrated its potential in the context of highly connected, semi-structured and unpredictable data structure. 

as a flexible, intuitive and fast data architecture in the field of biology, chemistry and... The amount and complexity of in comparison to other data storing mechanisms like relational databases to store heterogeneous datasets in the field of biology. Electronic health records (EHR) are traditionally used to store and analyze clinical routine data. 

Relational database architectures are 
Clinical data produced by hospital information systems (HIS) and documented by health care team members will traditionally be stored within relational databases. This type of databases stores the data in a tabular format usually by multiple rows and columns. This structure is well established and capable to save a huge amount of data. It seems like this

neo4j provides a strong community 

Exploration and analysing complex data is a difficult and time-consuming task in the daily routine of researcher and data scientists. Even if the workflow to analyse data and their connections might be well established The task gets even more challenging in the setting of a big data environment with multiple sources of heterogeneous data material. The in the conceptional phase of

With a relational database for instance you need to know the basic structure of your data before you can discover some new attributes. Graph Database could provide a flexible and new insight into the data that you are exploring. Neo4j seems to be a promising instance for graph databases and a great tool to explore data. With simple scripts, you can easily translate the given structure of a relational database into a visually explorable graphical data structure. Where you can obtain new 

Relational databases are well capable to save huge amount of data within a predefined schema. They are well established and offer a 
The complexity of data is 
The use of graphical databases in the clinical praxis is currently limited. Clinical data is stored in relational databases. This approach is well suited and 

With this paper we 