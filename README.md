# Climate Digital Twin Collaboration Elements

## One-sentence benefit

Coordinate shared climate scenarios, models and adaptation evidence through reusable API-connected web components.

## Live demo

[Watch the workflow](docs/demo.webm).

## Screenshots

![Climate digital twin collaboration dashboard](docs/screenshot.png)

## Main features

- Search twin cases by hazard, region, model, owner or status.
- Create new collaboration cases through the Java API.
- Advance scenarios through evidence review and approval.
- Display loading, empty, error and success feedback.
- Reuse encapsulated metric and workspace components responsively.

## Technology used

Lit, TypeScript, native custom elements, shadow DOM, Vite, Spring Boot and Java 21.

## Installation instructions

Install Node.js 22 and Java 21. Run `npm install`, then start the backend with `cd backend && mvn spring-boot:run`. In another terminal run `npm run dev`.

## Commercial licensing/contact

Commercial licensing and integration support are available. Use the repository contact options to discuss deployment.

## Business problem and users

Climate centres, public authorities and research partners need shared scenarios, comparable model evidence and accountable dataset ownership.

## Key workflows

Find a scenario, create a digital-twin case, review its model owner, advance its evidence state and inspect updated metrics.

## Lit/Web Components framework highlights

Lit reactive properties drive API state, repeat directives render keyed records, shadow DOM encapsulates styles and custom elements make the metrics reusable.

## Java backend highlights

Spring Boot provides validated list, search, create and update endpoints, structured errors, health status and domain service tests.

## Architecture and state flow

The custom element fetches `/api/items`; Vite proxies to Spring Boot, where the controller validates data and the service returns updated climate-twin records.

## Accessibility and responsive behaviour

Labelled controls, semantic regions, visible states, keyboard-ready buttons and responsive components support both compact and wide layouts.

## Verification commands

Run `npm test`, `npm run build`, `cd backend && mvn test` and `cd backend && mvn package`.

## Structure

`src` contains the custom elements, `backend` contains the Java API, and `docs` contains inspected product media.

## Tradeoffs

The sample uses in-memory data and simplified workflow states. Production use should add verified factors, persistent datasets and audit trails.

## Roadmap

Add model provenance, scenario comparison, map layers and adaptation decision exports.
