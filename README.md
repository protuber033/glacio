# Glacio Klimaattechniek

Website voor Glacio, een fictief airco-installatiebedrijf: 8 modellen, tarieven
voor plaatsing (binnen/buiten) en onderhoud, en een intakeformulier voor het
plannen van een afspraak.

## Structuur

- `index.html` — de volledige site (HTML/CSS/JS, geen build-stap nodig)
- `server.js` — minimale Node-server die `index.html` serveert
- `package.json` — start-script voor deployment (o.a. Railway)

## Lokaal draaien

```bash
npm start
```

Bezoek daarna `http://localhost:3000`.

## Intakeformulier

Het formulier opent bij versturen een vooringevulde e-mail naar het
contactadres in `index.html` (zoek naar `mailto:`) — er wordt bewust niets
serverside opgeslagen, zodat bezoekersgegevens niet in de website zelf
terechtkomen. Vervang het placeholder-adres door het echte bedrijfsmailadres
voordat de site live gaat.

## Prijzen

Alle bedragen op de site zijn indicatieve richtprijzen en niet gekoppeld aan
een live prijzensysteem — pas ze aan in `index.html` (zoek naar `MODELS` voor
de modellen, en de `price-card`-secties voor de diensttarieven).
