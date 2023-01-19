This is a public Wiki page for the InterConnect project. It lists the main technical results of the project and all resources that are needed for integrators to become part of the existing InterConnect semantically interoperable ecosystems, or build their own interoperable solutions.

[[_TOC_]]

# Project goals

<span dir="">Energy and IoT domain convergence through cross-domain semantic interoperability is at the forefront of the InterConnect project.</span>

The project aims to establish interoperability framework validating semantic interoperability based on SAREF ontology.

The project will produce innovative, user centric energy and non-energy services.

The technological approaches will be validated in 7 large scale pilots in Belgium, France, Germany, Greece, Portugal and The Netherlands also including an overarching use case across all pilots.

# Project Organization

Organization of the project work packages and consortium can be seen [here](https://interconnectproject.eu/consortium/#structure).

# Cascade Funding Opportunities

Here you can find the latest information about the project funding opportunities for European SMEs and Startups: <https://interconnect-opencalls.fundingbox.com/>

# Project outcomes and KERs

Here we list projects key exploitable results (KER) and outcomes that can be used by the wider public. Each KER has its own sub-section including figures, short introductory text and links towards detailed technical documentation, guidelines and software artefacts. The listed KERs are available for 3rd part integrators as complete set of enablers for joining the existing or building the new semantically interoperable ecosystems.

## InterConnect Ontology

The starting point is the ETSI SAREF or Smart Applications Reference ontology with its distributions for energy and buildings.

The project extends this ontology family with concepts specific to the cross-domain semantic interoperability requirements of the project.

So we have extensions for representing the user information and profiles, Device and sensor information and profiles, forecast and flexibility information which are very important in the scope of the project and finally connection information.

The project also uses other available ontologies for measurements, time representation and geo locations.

This document introduces the ontologies that have been developed in the context of the InterConnect project to cope with the variety of use cases and services implemented by the Interconnect large scale pilots. According to ontology engineering best practices, the Interconnect ontologies reuse already existing ontologies and, in particular, they extend the SAREF suite of ontologies promoted and maintained by ETSI.

Fig. 1- _Overview of InterConnect ontologies_ in relation to SAREF and other existing ontologies

![Ontologies_overview_v2](uploads/c99f9d492d48364d2d398389de151f41/Ontologies_overview_v2.png)

**External Ontologies**

Reuse of existing models is one of the pillars of the semantic web and linked data modelling paradigm. In the subsequent table, we provide a visual overview of the other external ontologies and data models that we have reused, in addition to SAREF, as basis for the InterConnect ontologies.

Table 1 – _Prefixes and namespaces_ of the _external_ ontologies reused by InterConnect
| Prefix | Namespace | Main concepts |
|--------|-----------|---------------|
| foaf | <http://xmlns.com/foaf/0.1/> | Agent |
| geo | <http://www.w3.org/2003/01/geo/wgs84_pos#> | Spatial Thing, geo coordinates |
| geosp | <http://www.opengis.net/ont/geosparql#> | Geographical Feature |
| schema | <https://schema.org/> | Address, Countries, Postal Codes |
| om | <http://www.ontology-of-units-of-measure.org/resource/om-2/> | Quantity, Unit, Measure |
| saref | <https://saref.etsi.org/core/> | Device, Function, Command, State, Measurement, Unit of Measure, Feature of Interest |
| s4bldg | <https://saref.etsi.org/saref4bldg/> | Building, Building Space, Building Object |
| s4city | <https://saref.etsi.org/saref4ener/> | Power Profile, Alternatives, Power Sequence, Slot |
| s4ener | <https://saref.etsi.org/saref4city/> | Facility, Administrative Area, City Object |
| time | <http://www.w3.org/2006/time#> | Instant, Interval, Duration |

**InterConnect Ontologies**

Within the framework of InterConnect project, the following nine ontologies have been modeled. Their prefixes and namespaces are presented hereunder.

Table 2 – _Prefixes and namespaces_ of the InterConnect ontologies
| Prefix | Namespace | Main concepts |
|--------|-----------|---------------|
| ic-data | <http://ontology.tno.nl/interconnect/datapoint#> | Datapoint, TimeSeries, Message, Utility Purpose |
| ic-dev | <http://ontology.tno.nl/interconnect/device#> | Device, State, Function |
| ic-flex | <http://ontology.tno.nl/interconnect/flexibility#> | Flex Offer, Flexibility Source, Control Type, Power Envelope |
| ic-fc | <http://ontology.tno.nl/interconnect/forecast#> | Forecast, Point Forecast, Stochastic Forecast (Gaussian, Quantile, Trajectory), Gaussian Data Point |
| ic-inc | <http://ontology.tno.nl/interconnect/incentivetable#> | Incentive Table, Incentive Tiers, Scope and Type |
| ic-pwlm | <http://ontology.tno.nl/interconnect/powerlimit#> | Power Limit (Nominal, Contractual and Failsafe) |
| ic-tplg | <http://ontology.tno.nl/interconnect/topology#> | Topological Location, Grid Segment, Market Segment, Regulation Zone, Electrical Phases |
| ic-uom | <http://ontology.tno.nl/interconnect/units#> | Additional Units of Measure (not considered yet in SAREF) |
| ic-user | <http://ontology.tno.nl/interconnect/user#> | User, User Profile, Preference, Priority, Interest, Activity, Time, Location |

More information about the InterConnect ontologies can be found at the following _Individual pages_.

1. [Datapoint, Timeseries and Message (ic-data)](https://gitlab.inesctec.pt/interconnect-public/ontology/-/wikis/ic-data)
2. [Forecast (ic-fc)](https://gitlab.inesctec.pt/interconnect-public/ontology/-/wikis/ic-fc)
3. [Incentive Table (ic-inc)](https://gitlab.inesctec.pt/interconnect-public/ontology/-/wikis/ic-inc)
4. [Power Limit (ic-pwlm)](https://gitlab.inesctec.pt/interconnect-public/ontology/-/wikis/ic-pwlm)
5. [User (ic-user)](https://gitlab.inesctec.pt/interconnect-public/ontology/-/wikis/ic-user)
6. [Flexibility (ic-flex)](https://gitlab.inesctec.pt/interconnect-public/ontology/-/wikis/ic-flex)
7. [Units of Measure (ic-uom)](https://gitlab.inesctec.pt/interconnect-public/ontology/-/wikis/ic-uom)
8. [Topology (ic-tplg)](https://gitlab.inesctec.pt/interconnect-public/ontology/-/wikis/ic-tplg)
9. [Device and sensor (ic-dev)](https://gitlab.inesctec.pt/interconnect-public/ontology/-/wikis/ic-dev)
10. [S2 standard (ic-s2)](https://gitlab.inesctec.pt/interconnect-public/ontology/-/wikis/ic-s2)

[InterConnect Ontology repository](https://gitlab.inesctec.pt/interconnect-public/ontology)

## InterConnect Interoperability Framework

The InterConnect delivers an Interoperability Framework capable of bridging the integration gaps “within” and “between” the IoT and the energy domains.

The Interoperability Framework comprises:

* **Semantic interoperability layer** (using InterConnect ontology over SAREF) based on distributed enablers interconnecting all resources, platforms and services and enabling them to exchange data and instructions in a uniform and secure manner while relying on widely adopted interfacing technology (RESTful). Exchanged data is not stored or processed anywhere in between communicating parties.
* **Service Store** a catalogue of all interoperable services, including knowledge exploring capabilities, service testing sandbox and automated interoperability compliance tests, streamline onboarding of 3rd parties’ services and systems to become part of the InterConnect ecosystem ensuring growth of the interoperable ecosystems and creation of new ones.
* **DLT based P2P marketplace enablers** allowing community-based energy and data trading use cases to be implemented in a way interoperable with project’s ecosystem.
* Configurable **access control and knowledge handling procedures** so that stakeholders can maintain business logic behind their services.
* A **methodology** for building semantically interoperable ecosystem by instantiating and configuring Interoperability Framework enablers within and among digital platforms and services comprising the interoperable ecosystem.

The Interoperability Framework provides different means for instantiation from centrally hosted facilitator to distributed framework maintained by interoperable ecosystem stakeholders. The result is enabling components (services, devices, digital platforms) to interact with each other without having to know each other’s local native API, but purely based on the knowledge of ontologies and what ontology (category) a component belongs to (e.g., forecaster service). Finally, the knowledge-centric interface made available by the Interoperability Framework, based on SAREF, becomes the interoperable and common vision that links all stakeholders in InterConnect, while not limiting the expressiveness nor the diversity of each party.

_High level architecture of the InterConnect Interoperability Framework:_

![Picture1](uploads/4ab71303f55008586f68a46083605833/Picture1.png)

_Levels of interoperability provided by the Interoperability Framework:_

![IF_architecture_SGAM](uploads/ab0d232e6621bed46498f0a55831367c/IF_architecture_SGAM.png)

### Service Store

<span dir="">As one of the main IC Interoperability Framework tools, the IC service store will provide a single stop for all providers and adopters of interoperable services from energy and non-energy domains. The service store is conceptualized as a web service with its front-end and back-end modules and processes. The main objective is to enable building of the InterConnect ecosystem of service providers and adopters by allowing them to register new interoperable services and browse existing ones to identify services best suited for the challenge at hand and get all necessary information for accessing and properly utilizing selected services.</span>

[Service Store web application](https://store.interconnectproject.eu/ServiceStore/#/auth/login?returnUrl=%2Fdashboard%2Fhome)

[Service store backend source code](https://gitlab.inesctec.pt/interconnect-public/service-store-backend)

[Service store frontend source code](https://gitlab.inesctec.pt/interconnect-public/service-store-frontend)

[Service store documentation](https://gitlab.inesctec.pt/interconnect-public/service-store-frontend/-/wikis/home)

### Semantic Interoperability Layer - Knowledge Engine

<span dir="">The Semantic Interoperability Layer (SIL) is the main component of the InterConnect Interoperability Framework. It is implemented as a distributed middleware responsible for facilitating secure and trusted semantic and syntactic interoperability between digital systems.</span>

<span dir="">Central to the design of the Knowledge Engine is the concept of a **Knowledge Base (KB)**. A KB is a logical unit where knowledge flows to and/or from. These KBs can be anything like apps, services or existing databases and their nature depends on the use case that is being implemented. Also, the size of a KB is flexible, it can represent a single device or a whole platform with multiple devices and services.</span>

<span dir="">Each KB instantiates a **Smart Connector (SC)** which allows it to register its capabilities and exchange data with other KBs connected to the **Knowledge Network (KN)**. The SC is the generic software component that does all the heavy lifting within the Knowledge Engine. Each SC registers itself in a **Knowledge Directory (KD)** with a description of the capabilities that it wants to make available to other SCs. These KB capabilities supported by the SC are called **Knowledge Interactions (KI)**. Each KI is a capability description of the KB and each KB has one or more KIs. There are four types of KIs: **Ask, Answer, Post and React**. Both the Ask/Answer and Post/React are opposites of each other where the Post and Ask Knowledge Interactions represent the capability of the KB proactively posting or asking data to/from the KN. While the React and Answer KIs represent the capability of the KB reactively reacting to or answering a question from a Post or Ask, respectively.</span>

<span dir="">A KI also contains one or two **graph patterns** (depending on its type) that uses the terminology from a common ontology to describe the actual type of data that the KB produces or consumes. The Ask and Answer KI expects a single graph pattern, while the Post and React require a single argument graph pattern, but optionally allow a result graph pattern as well. These graph patterns use a subset of the </span>[<span dir="">SPARQL syntax</span>](https://www.w3.org/TR/rdf-sparql-query/#BasicGraphPatterns)<span dir=""> and an example looks like this:</span>

<span dir="">_?mm rdf:type saref:Measurement ._</span>

<span dir="">_?mm ex:hasValueInCelcius ?v ._</span>

<span dir="">This graph pattern could be used in combination with the Post KI for a sensor KB that regularly publishes measurements of the temperature in degrees Celsius. These types of KIs together with the graph patterns cover most data exchange scenarios necessary for realizing the InterConnect pilots. After a KB has register its capabilities using KIs, the data exchange starts depending on their types.</span>

* <span dir="">In case of an **Ask KI**, the KB is expected to proactive trigger the Smart Connector to ask the registered question optionally providing bindings for the variables in its graph pattern. Any KB that can answer such questions will be involved by the SC.</span>
* <span dir="">In case of an **Answer KI**, the KB will be contacted by its SC whenever another KB asks the type of data it can provide.</span>
* <span dir="">In case of a **Post KI**, the KB can post data to its SC whenever it sees fit. Any KB with compatible KIs will get a chance to react to the publication of data.</span>
* <span dir="">In case of a **React KI**, the KB will be contacted by its SC whenever another KB posts data to which it wants to react.</span>

<span dir="">In short, a SC of KB A will involve any other KB B that has compatible capabilities with any of the capabilities of KB A. In the front of semantic reasoning the Knowledge Engine supports two approaches for checking KI compatibility and executing knowledge discovery and exchange:</span>

* **<span dir="">Graph pattern matcher</span>**<span dir=""> – this is approach where KIs will execute knowledge exchange only if the graph patterns completely match. This approach ensures high speed knowledge exchanges.</span>
* **<span dir="">Semantic reasoner</span>**<span dir=""> – this approach will ensure knowledge exchange through KIs with graph patterns that do not necessarily match completely. Partial matching is enabled and with it, new knowledge inference is possible in a wide Knowledge Network. The semantic reasoner is slower than the matcher, but it provides more flexibility in defining graph patterns for KBs.</span>

<span dir="">The Knowledge Engine Runtime comprises a set of Smart Connectors and internal interfaces needed for facilitating KIs between KBs. This KE Runtime can be deployed on different system levels: on level of single service runtime, on a level of one digital platform, shared among multiple services and digital platforms (e.g. on a pilot level) and on a global/project level. This flexibility in deploying KE Runtime constitutes the distributed nature of the Interoperability Framework.</span>

_Knowledge Engine as a distributed knowledge network:_

![image](uploads/18db3fa98f813a8c38e1fde58dd0af1c/image.png)

[Knowledge Engine Documentation](https://gitlab.inesctec.pt/interconnect-public/knowledge-engine/-/tree/main/docs)

[Knowledge Engine OpenAPI specification of developer REST API](https://gitlab.inesctec.pt/interconnect-public/knowledge-engine/-/blob/main/openapi-sc.yaml)


### Generic Adapter

In the InterConnect project we define the following adapters:

* **<span dir="">Service Specific Adapter (SSA)</span>**<span dir=""> – configuration/mapping point between legacy interface and data model of the service and the InterConnect SIL.</span>
* **<span dir="">Generic Adapter (GA)</span>**<span dir=""> – a generic software component that provides communication gateway for secure and trusted integration into a wider Interoperability Framework instance.</span>
* **<span dir="">InterConnect Service Adapter</span>**<span dir=""> – a combination of SSA and GA representing a semantically interoperable service in a wider InterConnect Interoperability Framework instance (e.g. within and between project pilots).</span>

_Adapter terminology used in InterConnect:_

![image](uploads/b8d474a41171d068a74f3e510eddcc94/image.png)

<span dir="">The Generic Adapter (GA) is a software gateway for secure and trusted communication between a service and a wider Interoperability Framework instance</span>. <span dir="">The GA enables:</span>

* <span dir="">A unified and secured communication interface using REST API;</span>
* <span dir="">Authentication and authorization point for IF access;</span>
* <span dir="">Deployment flexibility – Docker, with and without Knowledge Engine Runtime;</span>
* <span dir="">Automates registration of knowledge base and common knowledge interactions on boot.</span>

_High level architecture of the Generic Adapter:_

![image](uploads/8a736d893762e952995b23bf8bb9407b/image.png)

[Generic adapter source code](https://gitlab.inesctec.pt/interconnect-public/generic-adapter)

[Generic adapter REST API docs](https://gitlab.inesctec.pt/interconnect-public/generic-adapter/-/blob/master/generic-adapter-rest-OpenAPI.yaml)

[Generic adapter support documentation](https://gitlab.inesctec.pt/interconnect-public/generic-adapter/-/blob/master/docs/00_home.md)

[Generic adapter Docker containers](https://gitlab.inesctec.pt/interconnect-public/generic-adapter/container_registry/313)

### P2P Marketplace Enablers

<span dir="">The P2P marketplace enablers include:</span>

* **<span dir="">Hyperledger Fabric blockchain configurations</span>**<span dir=""> for different types of P2P marketplaces (different hierarchies, consortium organizations, stakeholders, nodes and channels).</span>
* **<span dir="">Smart contract templates</span>**<span dir=""> for different types of orders and transactions to be featured in the marketplace. Smart contracts will include APIs for end user GUIs (web application) and APIs for services for automated P2P trading.</span>
  * <span dir="">Smart contract templates for generating reports and audits about status of the marketplace and executed transactions - in line with regulatory and business requirements.</span>
  * <span dir="">Smart contract implemented as semantic interoperability adapter for interfacing with the wider InterConnect Interoperability Framework.</span>
  * <span dir="">Smart contracts for registering and identifying key actors and resources constituting P2P marketplaces.</span>
  * <span dir="">Smart Contracts for integration of interoperable services which write data to or read data from the Hyperledger Fabric. This ensures that the P2P marketplaces are integrated with a wider instance of Interoperability Framework.</span>
* **<span dir="">Configurable order matching engine</span>**<span dir=""> for managing regulatory constraints, transaction priorities and conflict resolutions. The ordering engine also chains the smart contract calls performed by services participating in the P2P marketplace.</span>
* **<span dir="">White-labelled web application</span>**<span dir=""> for providing interface through which end users place orders. The web application can be instantiated and adapted to specific needs of a community establishing the P2P marketplace.</span>

<span dir="">The Interoperability Framework provides these P2P marketplace enablers as part of its toolbox. The enablers are provided as deployable containers that allow pilot owners and integrators to deploy and fully manage P2P marketplace instances. The established P2P marketplaces are in full control and under jurisdiction (regulatory, market wise, data privacy protection) of the integrators.</span>

_InterConnect P2P marketplace enablers:_

![image](uploads/44add4a2118f84fd561462d142c4df37/image.png)

<div>

<span dir="">The P2P marketplace can be an energy marketplace or a marketplace for data transactions required for the realization of the community-based use cases. In the scope of the Task 5.4 the following P2P marketplace configurations are implemented and made available for the pilots and 3<sup>rd</sup> party integrators:</span>

* **<span dir="">Generic P2P marketplace configuration</span>**<span dir=""> that can be easily adapted to specific use cases in energy and IoT domains. This implementation also features a web application for demonstration purposes.</span>
* **<span dir="">Specialized configurations</span>**<span dir=""> based on participating pilots (each having specific set of requirements for integration of P2P marketplaces into instances of the Interoperability Framework):</span>
  * **<span dir="">Dutch pilot</span>**<span dir=""> - IoT data exchange with loyalty tokens realized through P2P marketplace.</span>
  * **<span dir="">Portuguese pilot</span>**<span dir=""> - flexibility and energy profile trading/aggregation in communities through P2P marketplace instance.</span>
  * **<span dir="">Belgium pilot from Think E! and VUB</span>**<span dir=""> - P2P energy trading within and between energy communities through instantiated P2P marketplace.</span>

</div>[P2P marketplace enablers repository](https://gitlab.inesctec.pt/interconnect-public/p2p-marketplace)

[Generic P2P marketplace configuration, code and documentation](https://gitlab.inesctec.pt/interconnect-public/p2p-marketplace/-/tree/p2p-sample-marketplace)

[Dutch pilot (P2P marketplace for IoT data) configuration, code and documentation](https://gitlab.inesctec.pt/interconnect-public/p2p-marketplace/-/tree/p2p-data-mp-activities-mg)

[Portuguese pilot (flexibility and energy profile trading/aggregation in communities) configuration, code and documentation](https://gitlab.inesctec.pt/interconnect-public/p2p-marketplace/-/tree/p2p-flex-sharing)

[Belgian pilot (P2P energy trading within and between energy communities) configuration, code and documentation](https://gitlab.inesctec.pt/interconnect-public/p2p-marketplace/-/tree/p2p-energy-trading)

## Service Specific Adapters

<span dir="">The Service Specific Adapter (SSA) is a custom software component developed and configured for a specific service/Knowledge Base. Each service provider goes through a process of implementing SSA. The main functionalities of the SSA are:</span>

* <span dir="">SSA Service endpoint functionality – includes all necessary functionality to interact with the service via the offered (legacy) service API.</span>
* <span dir="">SSA mapping functionality – performs mapping of parameter bindings (semantic interface) to service API parameters and vice versa. Can be one-to-one mapping or more complex logic to combine for instance several API calls to complete one binding set.</span>
* <span dir="">SSA GA endpoint functionality:</span>
  * <span dir="">Register the Generic Adapter instance for this service.</span>
  * <span dir="">Register the Knowledge Base - this creates a smart connector.</span>
  * <span dir="">Register the Knowledge Interactions (Graph Patterns).</span>
  * <span dir="">Offer Knowledge Interaction execution.</span>

_Knowledge Base with its SSA and GA:_

![image](uploads/43d1371e9b1d92df29c7b8cd16fd6f7f/image.png)

_Interoperability chain and message sequence chart between two interoperable services:_

![image](uploads/4a86df7bc7a04907ee82a549b8e9cbe4/image.png)

[Service SAREFization process guidelines.](https://gitlab.inesctec.pt/interconnect-public/service-specifc-adapters/-/blob/main/docs/sarefisation_process.md)

## Supporting Tools

Two supporting tools allow complementary action to assess pre-testing and visualisation. 

### SSA Test Tool:
The SSA Test Tool is integrated within the Generic adapter's control panel. It is directly accessible via the Generic Adapter local address. 
Refer to this link for more detailed information.

### Graph Pattern Visualiser.
The Graph pattern visualiser tool is available here. It allows to create a graphical representation of a graph pattern. It allows to identify all the nodes and connection among nodes of the pattern, leading to a better understanding of the data representation. Moreover, it also allows to find and solve loops in the data representation. 

## Tutorials


**Semantic Interoperability Framework: Overview**
[![Semantic Interoperability Framework: Overview](uploads/1d9a6f30f78b203c7bbf571209b9126f/SIF.png)](https://youtu.be/sSXDMCeIw2o)

**Semantic Interoperability Framework: Technical Integration Overview**
[![Semantic Interoperability Framework: Technical Integration Overview](uploads/0c04a745d85eaa1dc50de2ed636f6e4c/Tut.png)](https://youtu.be/-GCfEj-FAkUo)

**SAREFization process: Graph Pattern Creation - part 1**
[![SAREFization process: Graph Pattern Creation - part 1](uploads/2520713fe34c7c90065a52100d0e125c/Screenshot_2022-07-06_at_16.47.42.png)](https://www.youtube.com/watch?v=FM30JOFQDLo&ab_channel=InterconnectProject)

**SAREFization process: Graph Pattern Creation - part 2**
[![SAREFization process: Graph Pattern Creation - part 2](uploads/2520713fe34c7c90065a52100d0e125c/Screenshot_2022-07-06_at_16.47.42.png)](https://www.youtube.com/watch?v=l_QI7zoTazQ&ab_channel=InterconnectProject)

**SAREFization process: Create an SSA - part 1**
[![SAREFization process: Create an SSA - part 1](uploads/94b4c74edce550912d978841cbb717ea/Screenshot_2022-07-06_at_16.46.59.png)](https://www.youtube.com/watch?v=GOUCN0KKpuo&ab_channel=InterconnectProject)

**SAREFization process: Create an SSA - part 2**
[![SAREFization process: Create an SSA - part 2](uploads/94b4c74edce550912d978841cbb717ea/Screenshot_2022-07-06_at_16.46.59.png)](https://www.youtube.com/watch?v=W7ywyJSNEGs&ab_channel=InterconnectProject)

# Useful links

[InterConnect project website](https://interconnectproject.eu/)

[InterConnect YouTube channel](https://www.youtube.com/channel/UCGMdrFeqQyu88e0Liw_izRQ)

[InterConnect LinkedIn page](https://www.linkedin.com/company/interconnect-project/)

[InterConnect on Twitter](https://twitter.com/interconnectprj)

[InterConnect on Facebook](https://www.facebook.com/InterConnectPrj/)

[InterConnect Community on FundingBox](https://spaces.fundingbox.com/c/interconnect)

# InterConnect Project Prototypes

[InterConnect Prototypes](https://gitlab.inesctec.pt/groups/interconnect-public/-/wikis/Project-Prototypes)
