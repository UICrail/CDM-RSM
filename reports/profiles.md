# OWL Profile Validation Report

**Ontology**: ontology/src/core.ttl
**Date**: 2025-12-24 13:59:11 UTC

---

## OWL2 DL Profile

⚠️ **Status**: VIOLATIONS DETECTED

```
OWL 2 DL Profile Report: Ontology and imports closure NOT in profile. The following violations are present:
Use of reserved vocabulary for annotation property IRI: owl:versionIRI [null in OntologyID(OntologyIRI(<https://cdm.ovh/rsm/adapters/geosparql_adapter/geosparql_adapter>) VersionIRI(<https://cdm.ovh/rsm/adapters/geosparql_adapter/0.3/geosparql_adapter>))]
Use of reserved vocabulary for annotation property IRI: owl:versionIRI [Declaration(AnnotationProperty(owl:versionIRI)) in OntologyID(OntologyIRI(<https://cdm.ovh/rsm/adapters/geosparql_adapter/geosparql_adapter>) VersionIRI(<https://cdm.ovh/rsm/adapters/geosparql_adapter/0.3/geosparql_adapter>))]
```

## OWL2 RL Profile

⚠️ **Status**: VIOLATIONS DETECTED

```
OWL 2 RL Profile Report: Ontology and imports closure NOT in profile. The following violations are present:
Use of reserved vocabulary for annotation property IRI: owl:versionIRI [null in OntologyID(OntologyIRI(<https://cdm.ovh/rsm/adapters/geosparql_adapter/geosparql_adapter>) VersionIRI(<https://cdm.ovh/rsm/adapters/geosparql_adapter/0.3/geosparql_adapter>))]
Use of non-superclass expression in position that requires a superclass expression: DataSomeValuesFrom(<https://cdm.ovh/rsm/adapters/geosparql_adapter/geosparql_adapter#hasMetricLength> rdfs:Literal) [SubClassOf(<https://cdm.ovh/rsm/localisation/localisation#LinearLocation> DataSomeValuesFrom(<https://cdm.ovh/rsm/adapters/geosparql_adapter/geosparql_adapter#hasMetricLength> rdfs:Literal)) in OntologyID(OntologyIRI(<https://cdm.ovh/rsm/adapters/geosparql_adapter/geosparql_adapter>) VersionIRI(<https://cdm.ovh/rsm/adapters/geosparql_adapter/0.3/geosparql_adapter>))]
Use of reserved vocabulary for annotation property IRI: owl:versionIRI [Declaration(AnnotationProperty(owl:versionIRI)) in OntologyID(OntologyIRI(<https://cdm.ovh/rsm/adapters/geosparql_adapter/geosparql_adapter>) VersionIRI(<https://cdm.ovh/rsm/adapters/geosparql_adapter/0.3/geosparql_adapter>))]
Use of non-superclass expression in position that requires a superclass expression: ObjectUnionOf(<https://cdm.ovh/rsm/localisation/localisation#LinearLocation> <https://cdm.ovh/rsm/topology/topology#LinearElement>) [DataPropertyDomain(<https://cdm.ovh/rsm/adapters/geosparql_adapter/geosparql_adapter#hasMetricLength> ObjectUnionOf(<https://cdm.ovh/rsm/localisation/localisation#LinearLocation> <https://cdm.ovh/rsm/topology/topology#LinearElement>)) in OntologyID(OntologyIRI(<https://cdm.ovh/rsm/adapters/geosparql_adapter/geosparql_adapter>) VersionIRI(<https://cdm.ovh/rsm/adapters/geosparql_adapter/0.3/geosparql_adapter>))]
Use of non-superclass expression in position that requires a superclass expression: DataSomeValuesFrom(<https://cdm.ovh/rsm/adapters/geosparql_adapter/geosparql_adapter#hasMetricLength> rdfs:Literal) [SubClassOf(<https://cdm.ovh/rsm/topology/topology#LinearElement> DataSomeValuesFrom(<https://cdm.ovh/rsm/adapters/geosparql_adapter/geosparql_adapter#hasMetricLength> rdfs:Literal)) in OntologyID(OntologyIRI(<https://cdm.ovh/rsm/adapters/geosparql_adapter/geosparql_adapter>) VersionIRI(<https://cdm.ovh/rsm/adapters/geosparql_adapter/0.3/geosparql_adapter>))]
Use of non-superclass expression in position that requires a superclass expression: ObjectUnionOf(<https://cdm.ovh/rsm/topology/topo#Navigability> <https://cdm.ovh/rsm/topology/topo#NonNavigability>) [SubClassOf(<https://cdm.ovh/rsm/topology/topo#NavigabilityRelation> ObjectUnionOf(<https://cdm.ovh/rsm/topology/topo#Navigability> <https://cdm.ovh/rsm/topology/topo#NonNavigability>)) in OntologyID(OntologyIRI(<https://cdm.ovh/rsm/topology/topo>) VersionIRI(<https://cdm.ovh/rsm/topology/1.0rc4/topo>))]
```
