# Querschnittliche Konzepte



## Domain Model

```mermaid
classDiagram
    class User{

    }
    class Thing{

    }
    class Property{

    }

    class Place
    class Event
    class Product
    class Person
    class Organization

    Thing "0..*" --> "1..*" Property : has
    User "0..*" --> "0..*" Thing : has
    Place --|> Thing
    Event --|> Thing
    Product --|> Thing
    Person --|> Thing
    Organization --|> Thing
    Property --> "1..*" Thing 

```
### Examples
```JSONLD
{
    "@context": "https://schema.org/",
    "@type": "Thing",
    "name": "Schema.org Ontology",
    "subjectOf": {
        "@type": "Book",
        "name": "The Complete History of Schema.org"
    }
}
```
[Source](https://schema.org/Thing#examples)

## *\<Konzept 2>*

*\<Erklärung>*

…

## *\<Konzept n>*

*\<Erklärung>*
