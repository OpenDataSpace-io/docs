# Kontextabgrenzung


![System Scope and Context](./images/system%20scope%20and%20context.svg)
Erster Entwurf System Context

## C4 Model - Context
```mermaid
C4Context
    Person(Benutzer, "Benutzer")
    System(TourismusSysteme, "Tourismus Systeme")

    Boundary(b1, "", "") {
        System(OpenDataSpace, "OpenDataSpace", "Software System")
    }

    Rel(Benutzer, OpenDataSpace, "Erstellen und Bearbeiten")
    Rel(OpenDataSpace, TourismusSysteme, "Lesen und Schreiben")

    UpdateLayoutConfig($c4ShapeInRow="3", $c4BoundaryInRow="1")
```


## Fachlicher Kontext

**\<Diagramm und/oder Tabelle>**

**\<optional: Erläuterung der externen fachlichen Schnittstellen>**

## Technischer Kontext

**\<Diagramm oder Tabelle>**

**\<optional: Erläuterung der externen technischen Schnittstellen>**

**\<Mapping fachliche auf technische Schnittstellen>**
