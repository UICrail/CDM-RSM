# OWL Profile Validation Report

**Ontology**: ontology/src/core.ttl
**Date**: 2026-02-15 09:38:44 UTC

---

## OWL2 DL Profile

⚠️ **Status**: VIOLATIONS DETECTED

```
OWL 2 DL Profile Report: Ontology and imports closure NOT in profile. The following violations are present:
Use of undeclared annotation property: <http://creativecommons.org/ns#license> in annotation [Annotation(<http://creativecommons.org/ns#license> "http://creativecommons.org/licenses/by/3.0/") in null]
Use of undeclared annotation property: <http://purl.org/dc/elements/1.1/creator> in annotation [Annotation(<http://purl.org/dc/elements/1.1/creator> "Pieter Pauwels (pipauwel.pauwels@ugent.be)") in null]
Use of undeclared annotation property: <http://purl.org/dc/elements/1.1/creator> in annotation [Annotation(<http://purl.org/dc/elements/1.1/creator> "Walter Terkaj (walter.terkaj@itia.cnr.it)") in null]
Use of undeclared annotation property: <http://purl.org/dc/elements/1.1/date> in annotation [Annotation(<http://purl.org/dc/elements/1.1/date> "2015/12/11") in null]
Use of undeclared annotation property: <http://purl.org/dc/elements/1.1/description> in annotation [Annotation(<http://purl.org/dc/elements/1.1/description> "OWL ontology for LIST concepts") in null]
Use of undeclared annotation property: <http://purl.org/dc/elements/1.1/language> in annotation [Annotation(<http://purl.org/dc/elements/1.1/language> "en") in null]
Use of undeclared annotation property: <http://purl.org/dc/elements/1.1/title> in annotation [Annotation(<http://purl.org/dc/elements/1.1/title> "LIST") in null]
Use of undeclared annotation property: <http://purl.org/vocab/vann/preferredNamespacePrefix> in annotation [Annotation(<http://purl.org/vocab/vann/preferredNamespacePrefix> "list") in null]
Use of undeclared annotation property: <http://purl.org/vocab/vann/preferredNamespaceUri> in annotation [Annotation(<http://purl.org/vocab/vann/preferredNamespaceUri> "https://w3id.org/list") in null]
```

## OWL2 RL Profile

⚠️ **Status**: VIOLATIONS DETECTED

```
OWL 2 RL Profile Report: Ontology and imports closure NOT in profile. The following violations are present:
Use of undeclared annotation property: <http://creativecommons.org/ns#license> in annotation [Annotation(<http://creativecommons.org/ns#license> "http://creativecommons.org/licenses/by/3.0/") in null]
Use of undeclared annotation property: <http://purl.org/dc/elements/1.1/creator> in annotation [Annotation(<http://purl.org/dc/elements/1.1/creator> "Pieter Pauwels (pipauwel.pauwels@ugent.be)") in null]
Use of undeclared annotation property: <http://purl.org/dc/elements/1.1/creator> in annotation [Annotation(<http://purl.org/dc/elements/1.1/creator> "Walter Terkaj (walter.terkaj@itia.cnr.it)") in null]
Use of undeclared annotation property: <http://purl.org/dc/elements/1.1/date> in annotation [Annotation(<http://purl.org/dc/elements/1.1/date> "2015/12/11") in null]
Use of undeclared annotation property: <http://purl.org/dc/elements/1.1/description> in annotation [Annotation(<http://purl.org/dc/elements/1.1/description> "OWL ontology for LIST concepts") in null]
Use of undeclared annotation property: <http://purl.org/dc/elements/1.1/language> in annotation [Annotation(<http://purl.org/dc/elements/1.1/language> "en") in null]
Use of undeclared annotation property: <http://purl.org/dc/elements/1.1/title> in annotation [Annotation(<http://purl.org/dc/elements/1.1/title> "LIST") in null]
Use of undeclared annotation property: <http://purl.org/vocab/vann/preferredNamespacePrefix> in annotation [Annotation(<http://purl.org/vocab/vann/preferredNamespacePrefix> "list") in null]
Use of undeclared annotation property: <http://purl.org/vocab/vann/preferredNamespaceUri> in annotation [Annotation(<http://purl.org/vocab/vann/preferredNamespaceUri> "https://w3id.org/list") in null]
Use of non-equivalent class expression in position that requires an equivalent class expression: ObjectIntersectionOf(<https://w3id.org/list#OWLList> ObjectComplementOf(ObjectSomeValuesFrom(<https://w3id.org/list#isFollowedBy> owl:Thing))) [EquivalentClasses(<https://w3id.org/list#EmptyList> ObjectIntersectionOf(<https://w3id.org/list#OWLList> ObjectComplementOf(ObjectSomeValuesFrom(<https://w3id.org/list#isFollowedBy> owl:Thing)))) in OntologyID(OntologyIRI(<https://w3id.org/list>) VersionIRI(<null>))]
Use of non-superclass expression in position that requires a superclass expression: owl:Thing [SubClassOf(<https://w3id.org/list#OWLList> owl:Thing) in OntologyID(OntologyIRI(<https://w3id.org/list>) VersionIRI(<null>))]
Use of non-equivalent class expression in position that requires an equivalent class expression: ObjectIntersectionOf(<https://w3id.org/list#OWLList> ObjectComplementOf(ObjectSomeValuesFrom(<https://w3id.org/list#hasContents> owl:Thing))) [EquivalentClasses(<https://w3id.org/list#EmptyList> ObjectIntersectionOf(<https://w3id.org/list#OWLList> ObjectComplementOf(ObjectSomeValuesFrom(<https://w3id.org/list#hasContents> owl:Thing)))) in OntologyID(OntologyIRI(<https://w3id.org/list>) VersionIRI(<null>))]
```
