# Kontextabgrenzung


![System Scope and Context](./images/system%20scope%20and%20context.svg)
Erster Entwurf System Context

## C4 Model - Context
```mermaid
C4Context
    Person(User, "User")
    Person(Moderator, "Moderator")
    Person(Admin, "Administator")
    
    Boundary(b1, "", "") {
        System(OpenDataSpace, "OpenDataSpace", "Erlaubt Benutzer offene Daten zu erstellen und bearbeiten")
    }
    Boundary(b2, "", "") {
        System(TourismusSysteme, "Tourismus Systeme", "Bspw. CMS, PIM, ContentHubs, etc.")
    }

    Rel(User, OpenDataSpace, "Erstellen und Bearbeiten")
    Rel(Moderator, OpenDataSpace, "Archivieren")
    Rel(Admin, OpenDataSpace, "Löschen/Bereinigen")
    BiRel(OpenDataSpace, TourismusSysteme, "Lesen und Schreiben")

    UpdateLayoutConfig($c4ShapeInRow="3", $c4BoundaryInRow="1")
```


## Fachlicher Kontext

**\<Diagramm und/oder Tabelle>**

**\<optional: Erläuterung der externen fachlichen Schnittstellen>**

## Technischer Kontext

**\<Diagramm oder Tabelle>**

**\<optional: Erläuterung der externen technischen Schnittstellen>**

**\<Mapping fachliche auf technische Schnittstellen>**
