# PGB Meeting - July 30, 2020

**Attendees**
  * Adam Montville
  * Jason Keirstead
  * Charles Schmidt
  * David Solin
  * Duncan Sparrell
  * Forrest Hare
  * Jessica Fitzgerald-McKay
  * Jory Burson
  * Kelly Cullinane
  * Kent Landfield
  * Mitch Thomas
  * Sonu Shankar
  * Stephen Wood

**Note-taker's Note:** If you see any issues with these notes, let me (Adam) know; or add to them as appropriate. I tried to capture a lot of detail and hopefully I didn't editorialize or assume too much along the way.

**Agenda**
  * August Webinar
  * SCAP 2.0 Project Intake Review
  * Update on working groups
  
  
## August Webinar
OCA has been planning to have a webinar near the end of August to update the community on our progress and activities through the year. A hope is that the result of the second topic could be included as part of that webinar. The webinar is being organized by the marketing team, and PGB members have requested more transparency from that team (see first action below).

## SCAP 2.0 Project Intake Review
SCAP 2.0 work includes an Endpoint Data Collection (EDC) working group to address a gap from the SCAP 1.x specifications - get an architectural framework in place, so that the content specifications have a way to get around in an enterprise. The EDC group is interested in prototyping their current ideas, to learn from prototyping, and to eventually build a reference implementation that vendors can use to create ecosystem components. After Adam's brief introduction, Charles went through the intake form and diagrams from the EDC architecture document itself. Questions are captured below.

**Questions:**

  * **Is there a link to the architecture document?** Can the link be added into the project proposal? *Yes, there is a link and this can be added to the document* (See second action below.)
  * **SCAP has this as a skeleton, is it private or public at this point?** *Presently a local repository, but should be something that can be put in GitHub or some other public repository.* (See third action below.)
  * **You've seen the notional OCA reference architecture, and if we look at the diagram from the architecture draft, then are these messages part of the SCAP 2.0 specification?** *The standard shouldn't be tied to any specific fabric; what we'd "standardize" are the component roles, their interfaces, and payload formats. This is a detail that we're still working on.*
  * **Which SDO is that standard developed under (i.e. is there intent to eventually bring this work to an SDO)?** *Right now this is a NIST project and immediately intended to be published as a NIST specification. Ultimately, there is a hope that it would go into an SDO, and the SCAP community is open to whicih SDO would make the most sense when the time comes.*
  * **Is it safe to say that if there are existing standards you'll use them?** *SCAP intends to leverage existing standards where they exist. This architecture is data-collection-oriented and there is a larger ecosystem this work supports. SCAP itself is (and will continue to be) a "super-specification" that provides details on how to use a constituency of other specifications (i.e. XCCDF, OVAL, CVE, CPE, and the like).*
  * **What all ends up in the [architecture] repository?** *Collections, assessment results, an enterprise set of targets (computing resources intended to be assessed)*
  * **What are the primary use cases of this work?** *Inventory management, vulnerability management, configuration management, etc.*
  * **One of the issues we run into is terminology. We have something called the OpenDXL-Ontology project. Would you see this project working within that group?** *Yes, the probability that the SCAP work can inform the Ontology, and vice versa, is reasonably high.*
  * **We're a little fuzzy on resourcing and lifespan. If the project wraps up around the end of 2021, what's the plan for ongoing maintenance?** *The "grand hope" is that the work being done in the SCAP community will gradually transition to community ownership/management. Kent is additionally noting that this could be a community within OCA, which may help drive eventual adoption, which supports the cultivation of a healthy community.*
  * **Will this project be "fully engaged" throughout this time and after 2021 - will we be able to "help this project over the hump" so-to-speak?** *Presently, MITRE is developing the prototype, and they need more coders on the project. The intent is to have others involved in active development in the near future. The SCAP 1.x community is somewhat separate from the SCAP 2.0 community, and when the SCAP 1.x community is made more aware of this work, they'll likely come into this.*
  * **Is there intent to handle more cloud-native technologies?** *Yes, we've switched from talking about "endpoints" to talking about "targets" (any assessable computing resource).*
  
**Next Steps**

Jason is going to call for opening a ballot on this project (see second action below). In order for this to progress, we need a full majority vote. Because there aren't enough PGB members on the call, we'll do this electronically. The ballot will be issued this week and have a voting period for 10 days. 

## Update on working groups
Jory providing an update on the working group projects, though we only have five minutes left (good SCAP 2.0 discussion). A lot of this is being driven by work the OCA architecture working group has done, which is to build out some categorization of solutions. OCA has started to reach out for volunteers represented within the architecture working group, and outreach can be expanded. We've identified some gaps in coverage for these groups, and hope to close them. There is some concern that we may be experiencing continued issues with our communication tools.


## ACTIONS:

  * Add marketing report to standing PGB agenda goign forward; marketing team should also consider communication to the PGB distribution list for awareness
  * Charles (SCAP) embed link in proposal, send to Adam; Jason will attach to ballot
  * SCAP: Make current prototype available in a GitHub repository (location TBD, pending ballot)
    
    
  
  
