# RSM roots and design principles

RSM (in full: semantic rail system model) is the successor of RTM (rail topo model) released by UIC under IRS30100 in 2016. RTM itself is derived from the SNCF Infrastructure model ARIANE (unreleased).

As the name does not suggest, RSM provides fundaments for the description of the railway network and its components. Details are expected to be provided by other, federated models.

RSM, like its predecessors, is construed as a conceptual and implementable model: conceptual in the sense that it expresses concepts relevant to the railway domain, and implementable in the sense that the path from model to real data exchange is kept as short and simple as possible.

RSM, following the switch to semantic technologies (RDF/OWL, replacing UML class diagrams), has been entirely rewritten to make full use of the expressiveness of said technologies, and does not try to mimic the pecularities of the earlier, UML-based models when these peculiarities are not rooted in the railway domain concepts.

# RSM at a glance

RSM presents a modular structure: it is composed of several ontologies, following the "high coherence, low dependencies" principle. RSM also makes use of other ontologies to express common concepts, such as quantities, units, or geographic notions.

The present CDM-RSM repository contains only those RSM ontologies that are related to infrastructure topology, geometry, location in space, and location respective to the network topology. Other modules shall be found under:

* CDM-RST : rolling stock-related ontologies
* CDM-OPE : train operations ontologies (including telematics)
* ...

In addition to the above "domain ontologies", specialized ontologies called "adapter ontologies" or "adapters" will also be added. Adapters have the sole purpose to couple ontologies (RSM or others) while ensuring semantic alignment and avoiding version propagation (snowballing).


