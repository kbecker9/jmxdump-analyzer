# jmxdump-analyzer
The JMXDump Analyser Utility is a small, internal-only, self-contained JavaFX application which allows you to open an Alfresco 'JMX dump' file and will split the contents in manageable tabs. Highlighting the important stuff first and then breaking down the settings into the relevant topics, the utility makes JMX dumps much easier to read!

## Original Author 
[astrachan](https://github.com/astrachan)

## Current version
2.1.6

## Features
* You can run multiple JMXdump-analyzer's and open multiple zip files
* Allow you to drag and drop JMXDump zip files directly into the application
* Allows you to load in a JMXDump file from any version of Alfresco (including version 5.2 +)
* Allows you to drag and drop a JMXDump text file directly into the application
* Allows you to load in an Alfresco-generated JMXDump zip file
* Displays at-a-glance important information (Basic tab)
* Breaks down the settings into relevant sections (tabs) in fixed-width font for easier reading and copying/pasting
* Separates Global Properties from JMX-persisted settings (Global Properties are prepended with ** in the tabs)
* Analyses memory management/GC and availability
* Makes recommendations based on the data within the JMX Dump
* Gives a break-down of contentstore information (mount points and space)
* Gives a break-down of transactional cache statistics breakdown
* Shows Lucene/SOLR/SOLR4/SOLR6 cache information if applicable (plus approximate number of docs in the index)
* Shows the upgrade path
* Search through both the original jmxdump text as well as through the displayed tab information
* Ability to change font size in the UI

## Downloading, building and running the application
The name of the application is **jmxdump-analyzer-fx** and can be run on any platform (Windows, MacOS or Linux).
First you can clone this repository.

**Pre-requisites**
* Maven 3.9.9 or above
* Java 17

**Building**
`mvn clean install`

**Building the site/docs**
`mvn clean site:site`

This will create the docs/change reports etc... 

Browse to ~/target/site/index.html

**Running the application**
`java -jar target\jmxdump-analyzer-fx-x.x.x-jar-with-dependencies.jar`

The jar is also executeable, and will open with a double click :)

