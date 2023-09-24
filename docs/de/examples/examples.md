# Beispiele

## Thing
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

## Place - Allgemeine Öffnungszeiten
```JSONLD
{
    "@context": "https://schema.org",
    "@type": ["TouristAttraction", "AmusementPark"],
    "name": "Disneyland Paris",
    "description": "It's an amusement park in Marne-la-Vallée, near Paris, in France and is the most visited theme park in all of France and Europe.",
    "openingHours":["Mo-Fr 10:00-19:00", "Sa 10:00-22:00", "Su 10:00-21:00"],
    "isAccessibleForFree": false,
    "currenciesAccepted": "EUR",
    "paymentAccepted":"Cash, Credit Card",
    "url":"http://www.disneylandparis.it/"
}
```
[Source](https://schema.org/openingHours#eg-0432)

## Place mit spezifischen Öffnungszeiten
```JSONLD
{
    "@context": "https://schema.org",
    "@type": "Store",
    "name": "Middle of Nowhere Foods",
    "openingHours": "Mo,Tu,We,Th,Fr,Sa,Su 09:00-14:00",
    "openingHoursSpecification":
    [
        {
            "@type": "OpeningHoursSpecification",
            "validFrom": "2013-12-24",
            "validThrough": "2013-12-25",
            "opens": "09:00:00",
            "closes": "11:00:00"
        },
        {
            "@type": "OpeningHoursSpecification",
            "validFrom": "2014-01-01",
            "validThrough": "2014-01-01",
            "opens": "12:00:00",
            "closes": "14:00:00"
        }
    ]
}
```
[Source](https://schema.org/OpeningHoursSpecification#eg-0193)
