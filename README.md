# GOV.UK Prototype Demo Component

Example of a component (sass, nunjucks) automantically imported into the GOV.UK protoytype kit with the ability to remove styles.

## Getting started

```bash
npm i https://github.com/htmlandbacon/govuk-prototype-demo-component
```

## Examples

We have two marcos `prototypeCard` and `prototypeCards` which provides a 3 column layout on desktop and 1 column on mobile for `prototypeCard`.

### Example of a single card

```njk
{{ 
    prototypeCard({
    title: "Example card 1",
    titleUrl: "/example-card-1-link",
    description: "This is information about an example card."
    })
}}
```

### Example of a multiple cards

```njk
{{ 
    prototypeCards({
    cards: [
        {
        title: "Card 1",
        titleUrl: "/card1",
        description: "More info about card 1"
        },
        {
        title: "Card 2",
        titleUrl: "/card2",
        description: "More info about card 2"
        },
        {
        title: "Card 3",
        titleUrl: "/card3",
        description: "More info about card 3"
        },
        {
        title: "Card 4",
        titleUrl: "/card4",
        description: "More info about card 4"
        },
        {
        title: "Card 5",
        titleUrl: "/card5",
        description: "More info about card 5"
        },
        {
        title: "Card 6",
        titleUrl: "/card6",
        description: "More info about card 6"
        }
    ]
    })
}}
```

## Remove styles

In either your layout or page you are working on set the following.

```njk
{% set bodyClasses = "prototype-component--remove-style" %}
```

## Example template

Once installed you should be able to view a template page in the [manage prototype](http://localhost:3000/manage-prototype) section.