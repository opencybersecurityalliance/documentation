# Architecture Terminology
This is a start to a terminology document that can support our architectural diagrams. The approach being taken is to stick to a taxonomic structure where possible, so that terms build upon other terms in a clear way. We've started off with the SCAPv2 prototype entities as expressed in our C4 diagrams.

## Terms
**Accessor:** A Posture Assessment Manager component that informs consumers of endpoint postures.

**Aggregator:** A Posture Assessment Manager component that aggregates computing resource postures.

**C4 Model Component (a.k.a. Component):** A grouping of related functionality encapsulated behind a well-defined interface.

**C4 Model Container (a.k.a. Container):** A software implementation representing an application or a data store, generally comprised of components.

**Computing Resource:** An enterprise resource that is a composite of software and/or hardware.

**Configuration Policy Management System:** A software system that primarily interacts with a Posture Assessment System to effect configuration management in the enterprise.

**Health:** A Posture Assessment Manager component that monitors computing resource health and activity telemetry.

**Orchestrator:** A Posture Assessment Manager component that dispatches endpoint posture requests based on computing resource attributes.

**Posture Assessment Collector (a.k.a. Collector):** A container that is responsible for receiving collection instructions from the Manager, targeting computing resources for posture attribute collection, performing collection, and storing collected information in the repository.

**Posture Assessment Manager (a.k.a. Manager):** A container that is responsible for receiving instructions from other software systems, identifying and invoking collection components, and persisting collected posture attributes to a repository. [QUESTION: Does the Manager persist collected posture attributes when the Collector is also doing that?]

**Posture Assessment Repository (a.k.a. Repository):** A container that provides persistent storage and interface capable of recording previously collected posture information and providing that posture information when requested.

**Posture Assessment System:** A software system that carries out assessment of one or more targets, where assessment is related to at least one of vulnerability state, configuration state, or software load.

**Posture Collection Engine:** A Posture Assessment Collector component that directly collects information about enterprise computing resources.

**Posture Collection Extension:** A Posture Assessment Collector component that acts as an add-on to a Posture Collection Service, allowing for extended collection capabilities.

**Posture Collection Service:** A Posture Assessment Collector component that receives collection instructions from the Manager, and either engages a Posture Collection Engine or a Posture Collection Extension to perform collection.

**Software System:** A system that consists of intercommunicating software components. The c4 model defines software system as "the highest level of abstraction and describes something that delivers value to its users, whether they are human or not."

**Target:** A computing resource that is the subject of a query or operation.

**Threat Intelligence Sharing System:** A software system that...TODO
