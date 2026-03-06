# RSM — Semantic Rail System Model

The **Semantic Rail System Model (RSM)** provides the foundational ontology layer for describing the railway system, in particular its infrastructure.

RSM focuses on the **structural representation of the railway system** (topology, geometry, and spatial relationships). More specialized aspects of the railway domain are described by additional, federated ontologies.

RSM is compatible with the broader **Conceptual Data Model (CDM)** architecture.

---

# Origins

RSM is the successor of the **RailTopoModel (RTM)** released by UIC under **IRS30100** in 2016.

RTM itself evolved from earlier versions of the SNCF infrastructure model **ARIANE** developed before 2014.

While the technologies and modeling approach have evolved significantly, RSM inherits key domain concepts from these earlier models—most notably the **railway topology model**, which has been widely adopted across the industry.

---

# Purpose and scope

Despite its name, RSM is **not intended to model every aspect of the railway system**.

Instead, it provides **core semantic foundations** for describing the railway network and its components. More detailed domain models are expected to be built on top of these foundations.

This approach intentionally moves away from the idea of a single monolithic “God model” describing all railway data. Instead, RSM supports a **federated ecosystem of interoperable ontologies**.

---

# Architectural principles

## Modular ontology design

RSM follows a **loosely coupled modular architecture**.

It is composed of several ontologies designed according to the principle:

> **high internal coherence, low external dependencies**

This design approach is widely used in software architecture and helps ensure maintainability and extensibility.

## Reuse of existing ontologies

Whenever possible, RSM reuses established ontologies for common concepts such as:

- quantities and units
- geographic and spatial concepts
- general semantic modeling constructs

This avoids reinventing widely accepted vocabulary and improves interoperability.

---

# Repository structure

The present **CDM-RSM repository** contains only the ontologies related to:

- infrastructure topology
- infrastructure geometry
- spatial location
- positioning relative to the network topology

Other railway domains are modeled in separate repositories:

- **CDM-RST** — rolling stock ontologies  
- **CDM-OPE** — train operations ontologies (including telematics)

This separation supports the federated architecture of the CDM ecosystem.

---

# Adapter ontologies

In addition to domain ontologies, the CDM architecture includes **adapter ontologies**.

Adapters serve a single purpose: **aligning and connecting ontologies while preserving modularity**.

They allow different ontologies—whether internal RSM modules or external models—to be coupled without introducing tight dependencies.

This approach provides several benefits:

- semantic alignment between models
- controlled integration between ontology versions
- reduced risk of cascading dependency changes
- preservation of modular architecture

---

# Technical design principles

## Transition to semantic technologies

Earlier railway models were primarily expressed using **UML class diagrams**.

RSM has been fully rewritten using **Semantic Web technologies**, specifically:

- **RDF**
- **OWL**

The model therefore takes advantage of the expressiveness of these technologies rather than reproducing the structural constraints of UML where they do not reflect domain concepts.

## Property-based modeling

In RDF/OWL, properties (binary relations) are **first-class objects**.

RSM therefore avoids UML-style **association classes** (property reification) whenever possible. This leads to simpler knowledge graphs that remain closer to the underlying domain semantics.

The newer RDF standard **RDF*** is not used in the current version because support across tools and platforms is still incomplete. Future adoption of RDF* may allow further simplification.

---

# Constraints and validation

RSM distinguishes between two types of constraints.

## Semantic constraints

Constraints that express **intrinsic domain meaning** may be included directly in the ontology.

Example:

A *pair* logically requires two elements.

## Contextual or engineering constraints

Constraints that depend on:

- time
- engineering practice
- operational context
- project requirements

are expressed using **SHACL shapes** rather than embedded in the ontology.

Examples include constraints such as the number of balises in a balise group.

These SHACL shapes may be provided as examples but are not part of the core ontology.

---

# Reasoning profiles

RSM ontologies use the **OWL 2 DL profile** in order to guarantee **decidable reasoning**.

In practice, the model generally follows the more restrictive **OWL 2 RL profile**, which improves computational tractability.

Under the RL profile:

- queries can be answered in **polynomial time**
- reasoning remains scalable for large knowledge graphs

---

# Cardinality rules

Because of the chosen OWL profiles, ontology-level cardinalities are limited to:

- **0**
- **1**
- **\*** (unbounded)

Other cardinality constraints are expressed through **SHACL validation rules**, even when they have semantic relevance.

In practice, such cases remain relatively rare.
