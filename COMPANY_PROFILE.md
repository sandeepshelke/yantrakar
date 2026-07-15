# Yantrakar — Company Profile

## Overview

Yantrakar is a founder-led software engineering company based in Stavanger, Norway.

The company develops software for industrial robotics, drones, complex machine systems and long-lived engineering platforms. Its work is concentrated in environments where machines, control systems, communication technologies and operational applications must work together reliably.

Yantrakar develops solutions at two connected levels:

1. **Integration level** — connecting machines, PLCs, controllers, services and data sources through stable interfaces and communication technologies.
2. **Operations level** — building the applications and logic used to manage machine state, inventory, sequences, missions, rules and multi-machine workflows.

This combination is central to the company’s experience. Yantrakar does not only connect systems, and it does not only build operator-facing software. It works across the path from machine data and protocol integration to operational applications used by engineers and operators.

## Scope of work

Yantrakar is relevant when software must be developed around existing machines, robots, control systems or engineering platforms.

Typical work includes:

- understanding an existing machine and software architecture
- defining interfaces between machines, services and applications
- connecting systems that use different communication technologies
- collecting and normalising machine state
- building operational applications on top of integrated machine data
- developing configurable rule, mission and workflow logic
- supporting coordinated operation across several machines
- exposing mature C++ platforms through Python APIs
- improving maintainability in long-lived engineering software
- automating deployment in local, private or constrained environments

The company works across software design, implementation, testing, documentation, deployment and support.

## Integration-level experience

At the integration level, Yantrakar has developed software that connects machines, controllers, services and applications across different technologies and ownership boundaries.

### Common machine and service interfaces

Yantrakar has developed a common read/write interface across:

- PLCs
- DDS
- REST
- gRPC
- WebSockets

The purpose of this work was not only to hide protocol syntax. It also involved normalising differences in:

- addressing
- data types
- read and write behaviour
- connection lifecycle
- availability
- error handling
- update semantics
- ownership of state

This type of interface allows higher-level applications to work with machine and service data without being tightly coupled to each underlying technology.

### Distributed state collection

Yantrakar has developed software that gathers state from several distributed systems and makes that state available to operational logic.

Relevant experience includes:

- DDS data sources
- REST services
- gRPC services
- Redis-based state aggregation
- SQLite persistence
- local service communication
- handling several data producers with different update patterns

This work required deciding where state should be collected, how it should be represented, which system owns it and how downstream applications should consume it.

### Protocol and platform integration

Yantrakar has worked with a mixture of industrial and software communication technologies, including:

- DDS
- PLC interfaces
- REST
- gRPC
- WebSockets
- HTTP
- proprietary C++ APIs

The work has included adapters, service interfaces, common abstractions and application-facing access layers.

### C++ and Python interoperability

Yantrakar’s background includes development of Python APIs and bindings over mature C++ engineering platforms.

Relevant experience includes:

- Boost.Python
- API design
- object lifetime management
- exception translation
- conversion between Python and C++ data structures
- testing of bindings
- compatibility with existing client code
- Linux and Windows support

This is relevant where an existing C++ system needs automation, scripting, integration or gradual modernisation without replacing the core platform.

## Operations-level experience

At the operations level, Yantrakar has developed software used to represent, evaluate and manage how machine systems operate.

### Machine inventory and state management

Yantrakar has developed inventory and state-management software for drilling robots.

The work included:

- representing tools and inventory
- tracking operational state
- integrating machine data through DDS
- storing local data in SQLite
- using Python services
- integrating with an existing robotics framework

This required understanding how machine state changes during operation and how that state should be exposed to engineering and operational applications.

### Multi-machine sequence programming

Yantrakar has developed lightweight software for creating, inspecting and visualising sequences involving several manipulators or machines.

Relevant concerns included:

- representing multi-machine operations
- ordering and grouping sequence steps
- visualising execution flow
- coordinating activities across machines
- working with an existing robotics and motion-control framework
- making complex workflows understandable without exposing low-level control details

### Zone and rule management

Yantrakar has developed configurable zone-management logic based on preloaded expressions.

The work included:

- representing operational conditions as expressions
- loading configuration at startup
- evaluating rules against machine state
- separating operational logic from low-level control code
- integrating the result into existing machine software

### Mission Control

Yantrakar developed an independent Python application for collecting machine and service state and evaluating higher-level operational logic.

The system included:

- DDS, REST and gRPC inputs
- Redis-based state handling
- an expression parser implemented with Lark
- constants and variables
- arithmetic operations
- logical operations
- comparison operations
- configurable mission logic

This work addressed the need to place frequently changing operational logic outside individual machine-control components while still grounding decisions in live system state.

### Configuration preprocessing

Yantrakar has developed preprocessing and macro mechanisms for inventory and configuration data before runtime.

This addressed situations where:

- configuration values were repeated
- environment-specific substitution was required
- runtime systems needed resolved inputs
- configuration complexity was becoming difficult to maintain

## Industrial robotics and drilling automation

Yantrakar has delivered software related to robotic drilling systems and connected industrial equipment.

Relevant areas include:

- robot inventory management
- machine-state handling
- multi-machine sequence programming
- sequence visualisation
- zone logic
- mission logic
- distributed state collection
- unified read/write interfaces
- integration across PLCs, DDS, REST, gRPC and WebSockets
- local deployment automation

The work initially began through Head Energy and later continued directly through Yantrakar.

## Drone software and data infrastructure

Yantrakar has developed supporting software for drone applications and drone data handling.

### Interface-based application design

Yantrakar designed an interface-based solution for a drone application stack.

The purpose was to create clearer boundaries between components and reduce direct coupling to specific implementations.

Relevant outcomes included:

- replaceable implementations
- improved testability
- clearer ownership between components
- easier integration with surrounding services

### Standalone cloud backup

Yantrakar developed a standalone cloud-backup application for drone data.

Relevant technologies and concerns included:

- rsync
- Azure
- local and remote storage
- data synchronisation
- failure handling
- independent deployment
- operation alongside an existing drone application

### Local web service

Yantrakar developed a Drogon-based web server that interacted with a standalone application.

Relevant technologies included:

- C++
- Drogon
- Python
- HTTP interfaces
- local service communication

### Reproducible environments

Nix was used to support consistent software environments across development and deployment contexts.

## Engineering software experience

Yantrakar’s approach is informed by earlier work on mature engineering-software platforms.

Relevant experience includes:

- extending large C++ systems
- exposing C++ functionality through Python
- maintaining compatibility with existing users
- debugging production issues
- working on Linux and Windows
- adding tests around established behaviour
- improving maintainability without unnecessary rewrites

This is relevant to companies that have valuable software assets but need new APIs, integration points, automation or incremental modernisation.

## Local infrastructure and private AI deployment

Yantrakar has automated deployment of private local large-language-model infrastructure using Ansible.

Relevant experience includes:

- repeatable machine setup
- multi-machine deployment
- local model services
- controlled configuration
- local and private infrastructure
- reduction of manual setup
- operation without depending entirely on public cloud services

This experience is best described as deployment and integration of private AI infrastructure within existing engineering environments, rather than general AI consulting.

## Services

### Industrial robotics software

Development and improvement of software around robots and connected industrial equipment.

Typical work includes:

- robot-state applications
- inventory applications
- sequence tools
- workflow visualisation
- multi-machine coordination
- integration with existing robotics frameworks

### Machine and control-system integration

Integration of machines, PLCs, robot controllers, services and applications.

Typical work includes:

- protocol adapters
- common read/write interfaces
- state normalisation
- service integration
- application-facing APIs
- diagnosis of integration failures

### Operational applications

Development of software used by engineers and operators to understand and manage machine behaviour.

Typical work includes:

- machine-state views
- inventory management
- workflow tools
- sequence programming
- mission logic
- rule evaluation
- multi-machine coordination

### Mission, workflow and rule engines

Development of higher-level operational logic that should not be embedded directly in PLC or robot code.

Typical work includes:

- expression engines
- configurable rules
- mission evaluation
- state-driven workflow logic
- orchestration services
- sequence representation

### C++ and Python engineering

Development in systems that combine C++ and Python.

Typical work includes:

- Python bindings over C++ platforms
- C++ service development
- Python operational applications
- API design
- testing
- integration tooling

### Distributed industrial applications

Development of applications that consume data from several machines and services.

Typical work includes:

- state aggregation
- service communication
- local caching
- persistence
- reconnection handling
- interface standardisation

### Drone application infrastructure

Supporting software for drone applications and data workflows.

Typical work includes:

- interface-based application design
- local web services
- backup applications
- data synchronisation
- reproducible environments

### Private and local deployment infrastructure

Automation for systems that must run locally or within controlled infrastructure.

Typical work includes:

- Ansible automation
- repeatable deployment
- local model infrastructure
- configuration management
- restricted-network environments

### Engineering software modernisation

Incremental improvement of mature systems.

Typical work includes:

- new API boundaries
- Python access to C++ platforms
- selective refactoring
- test improvements
- deployment improvements
- extraction of tightly coupled operational logic

## Technology profile

### Programming languages

Primary:

- C++
- Python

Additional experience:

- C
- shell scripting
- SQL

### Robotics and machine systems

- Actin robotics framework
- industrial robot integration
- manipulator sequencing
- machine state and inventory systems
- PLC integration
- zone logic
- mission logic
- multi-machine coordination

### Communication and integration

- DDS
- REST
- gRPC
- WebSockets
- HTTP
- PLC interfaces
- proprietary C++ APIs

### Data and state management

- Redis
- SQLite
- distributed state aggregation
- local persistence
- configuration processing
- synchronisation workflows

### Web and service technologies

- Drogon
- Python services
- REST services
- local application servers

### Cloud and infrastructure

- Azure
- Ansible
- Nix
- rsync
- Linux
- Windows
- local and private infrastructure

### Parsing and configurable logic

- Lark parser
- expression languages
- constants and variables
- arithmetic operations
- logical operations
- comparison operations
- configuration-driven operational logic

### Engineering practices

- software design
- interface definition
- implementation
- testing
- documentation
- deployment
- support
- troubleshooting
- client communication
- technical presentations

## Client experience

### Canrig

Yantrakar has delivered software engineering work related to robotic drilling and automation systems for Canrig.

Relevant work includes:

- inventory and state-management software for drilling robots
- multi-machine sequence-programming and visualisation tools
- configurable zone logic
- configurable mission logic
- state collection through DDS, REST and gRPC
- Redis-based state aggregation
- a common read/write interface across PLCs, DDS, REST, gRPC and WebSockets
- deployment automation for private local LLM infrastructure

Public descriptions should remain at this level unless further disclosure is approved.

### KVS

Yantrakar has delivered software related to drone applications and drone data infrastructure for KVS.

Relevant work includes:

- interface-based application design
- standalone cloud backup
- Drogon-based local web service development
- C++ and Python development
- Azure integration
- rsync-based data synchronisation
- Nix-based environments

Public descriptions should avoid confidential implementation details.

## Relevant client situations

Yantrakar is relevant when:

- machine information is distributed across several protocols
- a new application must integrate with an existing robot or control system
- operational logic is embedded in code that is difficult to modify
- multiple machines need coordinated workflows
- machine-state ownership is unclear
- an existing C++ platform needs a Python API
- local applications need reliable data backup
- software deployment is manual or inconsistent
- private AI infrastructure must be deployed locally
- an existing system is valuable but difficult to extend

## Delivery model

Yantrakar is best suited to clearly scoped engineering work.

### Technical discovery

A short engagement to understand:

- existing architecture
- machine and service interfaces
- operational problems
- ownership boundaries
- technical risks
- realistic implementation options

Possible outputs include:

- system map
- interface inventory
- problem analysis
- architecture proposal
- implementation plan

### Prototype or proof of concept

A focused implementation used to validate:

- protocol integration
- state aggregation
- workflow representation
- rule evaluation
- local deployment
- technical feasibility

### Defined engineering project

Implementation of a clearly scoped component, service or integration.

Examples include:

- a machine-state service
- a common protocol interface
- a mission-rule engine
- a sequence tool
- a Python API over an existing C++ system
- a local deployment automation package

### Modernisation increment

Focused improvement of one part of an existing system without a full rewrite.

Examples include:

- introducing an API boundary
- extracting operational logic
- replacing direct protocol dependencies
- adding Python access
- improving testing and deployment

### Support and continuation

Maintenance and incremental improvement of systems Yantrakar has designed or implemented.

## Positioning boundaries

Yantrakar should be described as a specialist software engineering company for integration-heavy industrial and machine systems.

The company should not be presented as:

- a robot manufacturer
- a PLC safety-system supplier
- a large automation engineering house
- a general web-development company
- a general AI consultancy
- a full-service cloud consultancy
- a product company with a finished commercial platform

## Concise company description

Yantrakar develops software at both the integration and operational levels of industrial machine systems.

At the integration level, it connects robots, PLCs, controllers, services and data sources through common interfaces and technologies such as DDS, REST, gRPC and WebSockets.

At the operational level, it develops software for machine state, inventory, sequencing, mission logic, rules and multi-machine workflows.

The company works primarily with C++ and Python and is based in Stavanger, Norway.

## One-sentence profile

Yantrakar develops the software that connects machines and control systems to the operational applications used to understand and manage them.
