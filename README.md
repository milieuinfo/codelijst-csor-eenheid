# Codelijst CSOR Eenheid

Codelijst van eenheden voor het **Chemische Stoffen en Omgevingsparameters-Register (CSOR)** van de Vlaamse overheid, Departement Omgeving.

## Beschrijving

Een eenheid is een maat waarin een natuurkundige dimensie of een kwantificeerbaar aspect numeriek kan worden uitgedrukt.

Deze codelijst bevat **235 eenheden** gepubliceerd als [SKOS](https://www.w3.org/TR/skos-reference/) concept scheme via Linked Data.

- Concept scheme URI: `https://data.omgeving.vlaanderen.be/id/conceptscheme/csor/eenheid`
- CSOR namespace: `https://data.omgeving.vlaanderen.be/ns/csor#`
- Named graph (Virtuoso): `https://data.omgeving.vlaanderen.be/id/graph/codelijst-csor-eenheid`

## Bestandsformaten

De codelijst is beschikbaar in meerdere RDF-serialisatieformaten:

| Bestand | Formaat |
|---|---|
| `eenheid.ttl` | Turtle |
| `eenheid.jsonld` | JSON-LD |
| `eenheid.nt` | N-Triples |
| `eenheid.rj` | RDF/JSON |

De bestanden staan in:
```
src/main/resources/be/vlaanderen/omgeving/data/id/conceptscheme/csor/eenheid/
```

## Datamodel

Elke eenheid is een `csor:Eenheid` en een `skos:Concept` met volgende eigenschappen:

| Eigenschap | Beschrijving |
|---|---|
| `skos:prefLabel` | Nederlandse naam van de eenheid |
| `skos:notation` | Symbool / afkorting |
| `csor:symbool` | Symbool |
| `csor:conversiefactor` | Conversiefactor t.o.v. de basiseenheid |
| `csor:natuurkundigeDimensie` | Link naar de bijhorende natuurkundige dimensie |
| `csor:kwantificeerbareAspecten` | Link naar de kwantificeerbare aspecten waarbij deze eenheid gebruikt wordt |
| `csor:geldigTot` | Datum waarop de eenheid vervallen is (indien van toepassing) |
| `owl:deprecated` | Of de eenheid verouderd is |

### Gebruikte vocabularia

- [SKOS](https://www.w3.org/TR/skos-reference/) — Simple Knowledge Organization System
- [OWL](https://www.w3.org/OWL/) — Web Ontology Language
- [QUDT](http://qudt.org/) — Quantities, Units, Dimensions and Types
- [SHACL](https://www.w3.org/TR/shacl/) — Shapes Constraint Language (validatie)

## Licentie

[GNU General Public License v3.0](LICENSE)
