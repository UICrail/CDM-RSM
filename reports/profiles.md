# OWL Profile Validation Report

**Ontology**: ontology/src/core.ttl
**Date**: 2026-03-12 13:18:17 UTC

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
Use of non-superclass expression in position that requires a superclass expression: ObjectSomeValuesFrom(<https://cdm.ovh/rsm/topology/topo#toPort> owl:Thing) [SubClassOf(<https://cdm.ovh/rsm/topology/topo#Navigability> ObjectSomeValuesFrom(<https://cdm.ovh/rsm/topology/topo#toPort> owl:Thing)) in OntologyID(OntologyIRI(<https://cdm.ovh/rsm/topology/topo>) VersionIRI(<https://cdm.ovh/rsm/topology/1.0rc7/topo>))]
Use of non-superclass expression in position that requires a superclass expression: ObjectSomeValuesFrom(<https://cdm.ovh/rsm/topology/topo#fromPort> owl:Thing) [SubClassOf(<https://cdm.ovh/rsm/topology/topo#Navigability> ObjectSomeValuesFrom(<https://cdm.ovh/rsm/topology/topo#fromPort> owl:Thing)) in OntologyID(OntologyIRI(<https://cdm.ovh/rsm/topology/topo>) VersionIRI(<https://cdm.ovh/rsm/topology/1.0rc7/topo>))]
```
