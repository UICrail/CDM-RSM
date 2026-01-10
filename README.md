# RSM roots and design principles

RSM (in full: semantic rail system model) is the successor of RTM (rail topo model) released by UIC under IRS30100 in 2016. RTM itself is derived from early versions (before 2014) of the unreleased SNCF Infrastructure model ARIANE.

As the name does not suggest, RSM provides fundaments for the description of the railway network and its components. Details are expected to be provided by other, federated models. RSM is definitely a step away from an illusioned "God model" describing all possible aspects of rail for all possible usages. On the other hand, some RSM fundaments such as the topology model were widely adopted since 2016

RSM, like its predecessors, is construed as a conceptual and implementable model: conceptual in the sense that it expresses concepts relevant to the railway domain, and implementable in the sense that the path from model to real data exchange is kept as short and simple as possible.

# RSM at a glance

RSM presents a loose, modular structure: it is composed of several ontologies, following the "high coherence, low dependencies" principle shared by many software design areas. RSM also makes use of other ontologies to express common concepts, such as quantities, units, or geographic notions.

The present CDM-RSM repository contains only those RSM ontologies that are related to infrastructure topology, geometry, location in space, and location respective to the network topology. Other RSM modules shall be found under:

* CDM-RST : rolling stock-related ontologies
* CDM-OPE : train operations ontologies (including telematics)
* ...

In addition to the above "domain ontologies", specialized ontologies called "adapter ontologies" or "adapters" will also be added. Adapters have the sole purpose of coupling ontologies (RSM or "foreign") while ensuring semantic alignment and avoiding version propagation and mitigate the risk of snowballing.

# RSM technical fundaments

RSM, following the switch to semantic technologies (RDF/OWL, replacing UML class diagrams), has been entirely rewritten to make full use of the expressiveness of said technologies, and does not try to mimic the pecularities of the earlier, UML-based models when these peculiarities are _not_ rooted in railway domain concepts.

In particular, RSM takes advantage of RDF/OWL properties being first-class objects to avoid property reification ("association classes" in UML) whenever practical, resulting in simpler knowledge graphs kept closer to Domain notions. The latest version of the RDF standard, RDF* (RDF Star), is not used here because it is not universally supported; ultimately, adopting of RDF* will result in further simplifications.

Constraints (esp. cardinalities) are included in the RSM ontologies insomuch as they play a semantic role (e.g. a pair makes sense if two elements are provided, otherwise it is not a pair). Cardinalities that only express constraints that may be time-, engineering-,  or project-dependent (e.g. the constraints on the number of balises in a balise group) shall be expressed as SHACL shapes, with clear references to the time or context of validity. These SHACL shapes may be provided as samples, but are not part of the works.

RSM (as well as other CDM components) uses the DL profile of OWL2 in order to ensure the decidability of any query. In addition, RSM generally sticks to the slightly more restrictive RL profile in order to improve tractability: queries are guaranteed to be answered in polynomial, rather than exponential time.

Main consequence of this design choice is, cardinalities (multiplicities) can be expressed in terms of 0, 1, or * (undetermined) inside the ontologies; all other values shall be expressed as data constraints in SHACL shapes even if semantically relevant. Such cases are however rare.



