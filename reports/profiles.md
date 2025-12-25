# OWL Profile Validation Report

**Ontology**: ontology/src/core.ttl
**Date**: 2025-12-25 14:25:24 UTC

---

## OWL2 DL Profile

✅ **Status**: PASSED

```
OWL 2 DL Profile Report: [Ontology and imports closure in profile]
```

## OWL2 RL Profile

⚠️ **Status**: VIOLATIONS DETECTED

```
OWL 2 RL Profile Report: Ontology and imports closure NOT in profile. The following violations are present:
Use of non-superclass expression in position that requires a superclass expression: ObjectUnionOf(<https://cdm.ovh/rsm/localisation/localisation#LinearLocation> <https://cdm.ovh/rsm/topology/topology#LinearElement>) [DataPropertyDomain(<https://cdm.ovh/rsm/adapters/geosparql_adapter/geo_ad#hasMetricLength> ObjectUnionOf(<https://cdm.ovh/rsm/localisation/localisation#LinearLocation> <https://cdm.ovh/rsm/topology/topology#LinearElement>)) in OntologyID(OntologyIRI(<https://cdm.ovh/rsm/adapters/geosparql_adapter/geo_ad>) VersionIRI(<https://cdm.ovh/rsm/adapters/geosparql_adapter/0.6/geo_ad>))]
Use of non-superclass expression in position that requires a superclass expression: ObjectUnionOf(<https://cdm.ovh/rsm/topology/topo#Navigability> <https://cdm.ovh/rsm/topology/topo#NonNavigability>) [SubClassOf(<https://cdm.ovh/rsm/topology/topo#NavigabilityRelation> ObjectUnionOf(<https://cdm.ovh/rsm/topology/topo#Navigability> <https://cdm.ovh/rsm/topology/topo#NonNavigability>)) in OntologyID(OntologyIRI(<https://cdm.ovh/rsm/topology/topo>) VersionIRI(<https://cdm.ovh/rsm/topology/1.0rc4/topo>))]
```
