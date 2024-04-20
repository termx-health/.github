TermX is an open-source knowledge management and sharing platform, including a terminology server, Wiki, model designer, transformation editor, and tools for authoring and publishing. 

The core development goals of TermX were to enhance the interoperability of software and systems, particularly within the healthcare sector, by improving access to terminology, simplifying the design of data models, optimising the efficiency of data transformations across various data models, and developing implementation guides through an intuitive web interface. It aims to guarantee open and standardised access to published terminology, data models and schemas, ensuring semantic interoperability in accordance with the FHIR standard.

### Installation Guide
Follow [step-by-step instructions](https://github.com/termx-health/termx-quick-start) to install TermX.

### Demo
Try TermX in the [development environment](https://termx.kodality.dev/).

### Read more
Visit TermX [website](https://termx.org).

### Architecture
TermX consists of the internally and externally developed micro-services required to run TermX. The TermX micro-services include: 
- [TermX server](https://github.com/termx-health/termx-server), the main back-end application, written in Java, responsible for orchestrating TermX modules;
- [TermX web](https://github.com/termx-health/termx-WEB), an Angular-based front-end application, communicates with the server via a RESTful API, offering a user-friendly interface for effortless task execution;
- [FML editor](https://github.com/termx-health/termx-fml) (FHIR Mapping Language editor), an Angular-based front-end application for data transformation management that interacts with FHIR StructureDefinition and StructureMap resources while implementing the FHIR FML specification;
- [Chef](https://github.com/termx-health/termx-chef), the wrapper for Mitre Sushi and GoFSH projects that provides the ability to transform the FHIR JSON notation of the resources into Shorthand FSH notation and vice versa;
- [Structure definition viewer](https://github.com/termx-health/structure-definition-viewer), an Angular-based front-end application for visualization of FHIR StructureDefinition;
- [Static site generator](https://github.com/termx-health/termx-ssg), the wrapper for the Jekyll static website generator that generates sites based on TermX Wiki content.
