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

    Thing "0..*" --> "0.*" Property : has
    User "0..*" --> "0..*" Thing : has
```

*\<Erklärung>*

## *\<Konzept 2>*

*\<Erklärung>*

…

## *\<Konzept n>*

*\<Erklärung>*
