#### **Azure DT**  [^1]

Azure Digital Twins 
It is an enterprise-grade DT framework deployed as a platform as a service (PaaS) and hosted within the Microsoft cloud environment. It consists of a more generic framework that enables the creation of digital model-based twin graphs for a variety of use cases and scenarios. To define and build Azure DT models, a JSON-like language called Digital Twins Definition Language (DTDL) is made available. This language can be used to describe physical assets, including their data types, entries, states, properties, events, commands, and relationships. Moreover, Azure DT allows defining, creating, and building DT applications through a toolkit called Azure DT builder, which enables a more effective development DT process by creating and transforming building information modeling (BIM) into the corresponding DTs. Azure DT makes available a set of four DTDL-based industry ontologies that are compliant with the most relevant standards. This set of ontologies aims to assist solution providers in developing UDTs for smart buildings, smart cities, energy grids, and manufacturing. A short description for each of these ontologies is provided below.

- ontology for smart building modeling[^2]: it is based on relevant industry standards like BRICK Schema and W3C Building Topology Ontology;

- ontology for smart cities modeling[^3]: it is essentially based on the ETSI CIM NGSI-LD standard following a collaboration between Microsoft, Open Agile Smart Cities (OASC), and Sirus;

- ontology for energy grids modeling[^4]: it was obtained by adapting the Common Information Model, which is a global standard for energy grid asset management, modeling of power system operations, and the physical energy commodity market;

- ontologies for manufacturing[^5]: it consists of a subset of ontologies, which are obtained by adapting three global standards widely used in the manufacturing space, namely OPC UA, ISA95, and the Asset Administration Shell.

Finally, Azure Digital Twins Explorer is a visualization tool that shows how to interact with a DT graph corresponding to a physical building.

#### **AWS IoT TwinMaker** [^6]

AWS IoT TwinMaker is a commercial cloud-hosted framework that assists in the creation of DTs of real-world systems such as buildings, factories, industrial equipment, and manufacturing lines. Amazon IoT TwinMaker supports popular IoT protocols such as MQTT, HTTPS, and LoRaWAN. It also refers to Amazon Sumerian to develop DT-like apps by providing capabilities to support 3D building modeling and AR/VR interfaces. Additionally, Amazon provides a service called Device Shadow to assist the deployment of a shadow model related to a physical device, providing the corresponding application that manages its possible states. Device shadow metadata (such as states, versions, security tokens, and properties) is collected in JSON files and exchanged with DT services via REST APIs.

#### **Bosch IoT Suite** [^7]

Among the most advanced DT frameworks, Bosch IoT Suite aims to provide manufacturing companies with the totality of tools and technologies required to construct and expand their IoT-based architectures, especially supporting them in managing their corresponding DTs. It adopts open data models to implement digital representations of physical devices and unified device APIs that are based on Eclipse Vorto Information Models. Bosch IoT Suite is compliant with most of the standard protocols to interface IoT devices, such as MQTT and Advanced Message Queuing Protocol (AMQP). Bosch IoT Remote Manager is an online service that enables engineers, device manufacturers, and service providers to manage the entire IoT device life-cycle, by controlling the state of any deployed device and performing their centralized remote maintenance. This service is deployed on Microsoft Azure and runs on a Docker infrastructure to foster scalability and reliability. The open -source technologies adopted to implement by Bosch IoT Suite are capable of offering a fully managed cloud services environment while avoiding vendor lock-in phenomenon. This approach can also foster and stimulate future development of the Bosch IoT Suite by leveraging on the collaboration and participation of the underlying open-source communities.

#### **CPS Twinning** [^8]

CPS Twinning represents an open-source framework to create, produce, and implement DTs for cyber-physical systems (CPSs). It adopts a data interchange standard named Automation ML to support DT development. Moreover, it is capable of automatically generating virtual environments for DTs that are fully compliant with the corresponding specifications. The CPS Twinning architecture adopts a specific tool known as CPS State Replication to enable CPS Twinning's replication mode. This replication mode allows DT entities to passively monitor stimuli and follow the states of their physical counterparts. Finally, this framework provides many specific security modules to assist security analysts in monitoring CPSs and putting in place specialized and customized security features, such as intrusion detection, access control, audit, and accountability.

#### **Davra Platform** [^9]

Davra is a fully open-source Industrial IoT platform that supports the definition, development, and fast deployment of DTs for the creation of single, stable, secure, and scalable IoT applications. Davra provides an open library that enables secure access to the DT's connecting APIs. A TwinType Object is purposely defined to manage the entire life-cycle of DT data, which allows obtaining an existing twin's data, managing platform objects in the form of key/value pairs, listing all DT's attachments, and so on.

#### **Eclipse Ditto** [^10]:
The Eclipse community offers an IoT open-source framework called Ditto, which makes available a set of ready-to-use functionalities for managing the state of DTs. It can implement a middleware between the real-world asset and the corresponding digital model. Essentially, the feature set offered by Eclipse Ditto includes: (a) Device as a Service, which mirrors physical assets and devices using advanced web APIs for specifically interfacing devices remotely and interacting with the corresponding DTs; (b) DT State management, which provides an event-based mechanism to notify state changes, along with a single and real -time representation of a physical asset; and (c) DT Management, which makes available meta-data and meta-models to be used for querying, searching, and selecting entity's attributes of both a physical asset and the corresponding digital counterpart. In this regard, Eclipse Ditto makes available a set of REST APIs to be used for implementing backend-less IoT applications, allowing developers to focus on more relevant aspects related to the application's business logic and user experience. At the same time, Eclipse Ditto can support the integration of different network protocols, brokers, and messaging systems. By combining Eclipse Ditto with Eclipse Vorto, it is also possible to obtain a general-purpose and adaptable framework for DT development.

#### **Eclipse Vorto** [^11]:
Another open-source project from the Eclipse community is Vorto, which makes available a language for defining models and interfaces of IoT DTs. During the development phases of an IoT solution, the modeling contribution offered by Vorto aims to centralize the management of IoT devices and logical entities from different sources, in terms of provision, use, and configuration. Eclipse Vorto also makes available specific features for device integration, description, and abstraction. As a domain-specific language, Vortolang represents the reference language for implementing DTs in Vorto. In effect, an IoT solution developed using Eclipse Vorto can semantically describe its entities' capabilities using the Vortolang language. Eclipse Vorto provides a repository of information models, where the same models can be managed and shared. Each of these models consists of abstract representations corresponding to the device's characteristics and properties and is published by the corresponding device maker. In this way, each information model stored in the repository can be freely accessed and downloaded. Starting with an information model, it is possible to implement the corresponding platform-specific source code using Vorto's code generators, simplifying the device integration for a given platform. The Vortolang refers to a set of metamodel classes for defining the capabilities of DTs. Eclipse Vorto adopts two top-level classes to implement a DT and its capabilities, which are called Information Model and Function Block, respectively. In turn, DT capabilities are characterized by the following three metamodel classes: Properties, Events, and Operations. Beyond fully describing a DT as a physical asset, an Information Model outlines the collection of interfaces as Function Blocks that the DT implements. A Function Block consists of properties, events, and operations and can be reused by many information models.

#### **FIWARE** [^12]

The FIWARE community provides an ecosystem of Generic Enablers (GEs) that allows modeling DT context data using a catalog of components and smart data models. Physical assets are virtually represented as digital entities (static or dynamic) that are identified by a Universal Resource Identifier (URI) and characterized by a variety of properties and relations with other entities. In this way, DT entities are uniformly represented using standard data models as long as linked together and managed by the FIWARE solution. A Powered by FIWARE solution consists of an architecture that includes a Context Broker component (e.g., Orion -LD, Scorpio, and Stellio) and several optional GEs that expand its functionalities based on the use case requirements. The Context Broker enables the usage of NGSI/NGSI-LD APIs, which are RESTful APIs meant to simplify access to DT data along with its integration in the FIWARE DT architecture. The list of GEs includes a stack of components that simplify the development of integration with various counterparts. Available integration features include interfaces for IoT, robotics, and several third-party systems, as well as enabling Complex Event Processing (CEP), advanced big data processing engines (e.g. Apache Flink, Apache Spark), data visualization and monitoring tools (e.g. Grafana and web mash-up), management of historical data, real-time media stream processing, advanced authentication/authorization schema enablers, and a business framework for defining policies to publish and monetize data. The Smart Data Models initiative makes available an open -source catalog, which is kept up -to -date by the FIWARE community. This catalog continuously proposes new data models, but also amendments to the existing data models. The Smart Data Models catalog is conveniently organized in domains (e.g. Smart Cities, Smart Energy, Smart Industry, etc.), promoting the reuse of the existing data models when developing a smart solution. Data models proposed by this initiative are available in JSON and JSON-LD formats according to the specifications adopted by schema.org and NGSIv2/NGSI-LD APIs for standardization and interoperability purposes.

#### **IBM Digital Twin Exchange** [^13]

IBM Digital Twin Exchange is a marketplace resource for asset-intensive industries that supports the management of linked assets, equipment, and IoT solutions. IBM developed a virtual testbed to test and assess complex IoT systems using real-world and simulated data. In addition, IBM created an ontology-based knowledge graph for IoT architecture that enables real-time analysis and comprehension of the industrial process life-cycle by blending AI/ML reasoning with statistical analytics.

#### **Nvidia Omniverse Digital Twins** [^14]
Nvidia Omniverse is a platform for developing and running metaverse applications wherever the digital and real worlds collide. It offers procedural control of behavior, motion, and action using Generative Adversarial Networks (GAN), diffusion model-based neural rendering tools, and graph execution engines. It can be considered one of the most sophisticated commercial tools for processing the kinematics of complicated multi-part objects for synthetic data generation and DT simulations. Essentially, the feature set offered by Nvidia Omniverse includes: (1) the Replicator application, which is used to generate synthetic data for training self-driving cars, robots, and various computer vision models, (2) JT Connector, which is a connector for product life-cycle management based on the Siemens JT industry standard language, and (3) supports interoperability with most of the CAD systems such as NX, Creo, Catia, and Inventor. From design and engineering through manufacturing, marketing, and operations, various tools involved in the Omniverse Enterprise support different stages of the product life cycle. They allow the user to create an end-to-end 3D pipeline for building and managing factories and warehouses. This is the comprehensive package for generating synthetic data and simulating DTs, with a set of tools for various aspects of product development and operation. For instance, on the Omniverse platform, an AI factory can be built within a data center for processing data to train AI models that simulate DTs and map the physical world. Likewise, an AI computer can be embedded in automobiles to process sensor data for environmental perception, obstacle avoidance, and autonomous driving toward a specific destination.

#### **Oracle IoT DT** [^15]

Oracle IoT Digital Twin Simulator enables the creation of simulated IoT devices in a predefined environment, without requiring the connection of these devices to real-world hardware platforms. Data and models needed to build DT applications can be generated, including configuration data, alerts, and events related to simulated entities. Once a simulated scenario has been validated, it is possible to manage, monitor, and interact with IoT devices, even in real-time, using the corresponding DT application. Oracle's DT framework is built on three software pillars: (1) Virtual Twin, which employs a JSON-based data model to design virtualization of IoT devices and produce a virtual clone of the real-world physical asset in the cloud; (2) Predictive Twin, which uses AI/ML and analytical or statistical models to forecast the future evolution of processes; and (3) Twin Projections, which connect forecasts and insights with back-end business systems and third-party solutions through the usage of REST API libraries.

#### **Reflexer Digital Twin** [^16]

Reflexer Digital Twin was developed as an open-source modular toolkit by a private company called BlockScience. It refers to Python-based simulation scripts for designing, testing, and validating dynamical systems, which can be even complex and generalized. Reflexer Digital Twin supports the scheduling of various routine tests and system predictions within the CAD framework. To enable a variety of data-driven computations and decision-making processes, this toolkit can collect real-time data from both physical real-world assets and their corresponding virtual counterparts within a DT.

#### **ScaleOut** [^17]

ScaleOut represents a suite of software tools to create real-time DT models. It adopts an in-memory data grid for serializing DT instances expressed in JSON format. ScaleOut offers statistical analysis and ML capabilities for both trend change and anomaly detection using unsupervised and supervised learning techniques, respectively. Moreover, ScaleOut makes available the ScaleOut Digital Twin Builder software toolkit and the ScaleOut Model Development Tool to implement cloud-hosted stream processing services. Popular event hubs such as Microsoft Azure IoT Hub, Amazon AWS IoT Core, and Azure Kafka are used by the streaming service to support connections to various data sources. For this purpose, the streaming service makes available an integrated REST messaging service. It provides a user interface for aggregating real-time analytics and highlighting occurring state changes for each configured data source.

#### **SINTEF Digital Twin** [^18]

SINTEF Digital Twin consists of an architectural proposal to connect tools to design DTs of physical assets. For designing a DT, it adopts knowledge graph ontologies to model and integrate the corresponding data. In this way, SINTEF acts as a bridge that combines and connects data from multiple systems. The flexibility margins offered by this open-source architectural framework make it possible to be tailored for specific domains, such as smart manufacturing. Being deployable in Docker containers, its databases can be directly pulled from Docker Hub to generate quick DT prototypes. Furthermore, these databases can eventually be switched as needed and installed in a fully managed persistent infrastructure, once the most appropriate technology vendor has been identified, enabling a company to secure and share data cross-company or cross-process in a selective, tamperproof way while maintaining data sovereignty.

#### **Tributech DT Kit** [^19] 

Tributech DT Kit represents an open-source framework that supports DT application development by making available software modules such as Catalog API, Catalog UI, Client API, and Twin-API. Another relevant component offered by this framework is the DataSpace Kit (DSK) tool. DSK describes data assets using a specific language called Digital Twin Definition Language (DTDL). Implementing a dataspace, DSK makes available three fundamental components called DataSpace Hub, the DataSpace Node, and the DataSpace Agent corresponding to the concepts of ecosystem, platform, and device, respectively. DSK reduces the burden of managing twin instances and models through a separate web application by merging the configuration artifacts into a single, easy-to-use API and user interface. Additionally, Tributech's stack also includes an OEM Module hardware component that is intended to help smart product developers easily connect a device in the Tributech ecosystem. These connections can facilitate essential operations through a unified interface, managing telemetry information, settings, updates, provisioning, and security. They guarantee data integrity and sharing capabilities, enabling the creation of specialized data repositories for commercializing raw data or derived insights. By meeting these fundamental requirements during the design of physical IoT devices, it becomes possible for developers to implement optimized solutions without the need to take care of the overall complexity, which generally characterizes aspects such as connectivity and data management

#### **White Label Digital Twin** [^20]
White Label Digital Twin (WLDT) is a Java framework for building IoT-based DT applications. It is capable of efficiently replicating intelligent physical items in their digital equivalents by optimizing modularity, reusability, and adaptability. WLDT supports typical features and functionalities of a DT that are compatible and compliant with various communication protocols and standard data formats, including MQTT and CoAP protocols. Moreover, this framework adopts various communication paradigms such as Publish/Subscribe and Request/Response. WLDT can operate in the edge and cloud contexts of an edge-cloud software architecture. Beyond offering wide margins of flexibility and scalability, the WLDT framework facilitates the modular development of an IoT microservice architecture by integrating its modules seamlessly into the extensible API-based DT network. The framework's central component, known as the WLDT Engine, is responsible for creating, managing, and coordinating the DT actions. The remaining software components are active agents known as Workers. By using the Processing Pipeline layer offered by the framework, a Worker can be easily configured to either process incoming data or interact with external services for translating and transforming data formats. The WLDT framework provides increased modularity, reusability, and flexibility for DTs by effectively and efficiently supporting DT design and development.

[^1]: <https://learn.microsoft.com/en-us/azure/digital-twins/>

[^2]: <https://github.com/Azure/opendigitaltwins-building>

[^3]: <https://github.com/Azure/opendigitaltwins-smartcities>

[^4]: <https://github.com/Azure/opendigitaltwins-energygrid/>

[^5]: <https://github.com/digitaltwinconsortium/ManufacturingOntologies>

[^6]: <https://aws.amazon.com/it/iot-twinmaker>

[^7]: <https://bosch-iot-suite.com>

[^8]: SBA Research – CPS Twinning repository. <https://github.com/sbaresearch/cps-twinning>


[^9]: <https://github.com/Davra/>

[^10]: <https://eclipse.dev/ditto/>

[^11]: <https://eclipse.dev/vorto/>

[^12]: <https://smartdatamodels.org>

[^13]: <https://www.ibm.com/mysupport/s/topic/0TO0z000000ZevgGAC/digital-twin-exchange?language=en_US>


[^14]: <https://developer.nvidia.com/blog/building-an-active-digital-twin-using-nvidia-omniverse-and-project-gemini/>

[^15]: <https://docs.oracle.com/en/cloud/paas/iot-cloud/iotgs/oracle-iot-digital-twin-implementation.html>

[^16]: <https://github.com/reflexer-labs/reflexer-digital-twin/>

[^17]: <https://static.scaleoutsoftware.com/docs/digital_twin_user_guide/index.html>

[^18]: https://www.ibm.com/mysupport/s/topic/0TO0z000000ZevgGAC/digital-twin-exchange?language=en_US>


[^19]: <https://www.tributech.io/blog/oem-module>

[^20]: <https://github.com/ElsevierSoftwareX/SOFTX-D-20-00018>

