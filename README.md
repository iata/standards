# IATA Data Exchange Standards Registry

The IATA Standards Registry is a central repository to discover and retrieve IATA data exchange standards artifacts, published from the latest release and historical releases. It supports consistent access, release traceability, and the use of standards by the airline and aviation industry stakeholders.

## Scope

Published releases include:

- OpenAPI specifications
- JSON Schemas
- XSD Schemas
- Other related technical artifacts and documents

IATA standards are published according to formal IATA release cycles. The [official Standards Registry](https://github.com/iata/standards) contains officially published artifacts.

## Publication principles

- **Traceability:** Each published artifact is associated with an official IATA release, a Git tag, and a corresponding GitHub Release.
- **Historical access:** Latest and earlier published releases remain accessible to industry stakeholders.
- **Immutability:** Published tags, artifacts, and GitHub Releases are not changed after publication. Corrections are made available in a subsequent maintenance release.

## Intended use

Use the registry primarily during design and development for artifact discovery, dependency resolution, validation setup, code generation, and implementation onboarding. Retrieve, cache, and package the artifacts and dependencies required by your implementation as part of your build or deployment process.

**Do not depend on live registry retrieval at production runtime.** Production systems should use locally managed copies in deployment packages or internal artifact repositories. The registry is a reference and distribution mechanism, not a runtime service with production service-level guarantees.

## Repository layout

By default, published standards artifacts governed under the IATA [Passenger Standards Conference](https://www.iata.org/en/about/corporate-structure/passenger-standards-conference/) are located under `psc/`:

```text
standards/
├── README.md
└── psc/
     └── Standards artifacts
```

## Find a release

- **Latest published artifacts:** Browse the `main` branch of the repository or use the [official Standards Registry](https://github.com/iata/standards). The registry makes the latest published release available from `main` through GitHub Pages.
- **A specific or historical release:** Open the [repository's Releases page](https://github.com/iata/standards/releases), select the IATA release number, to access its release notes, artifacts, and publication date.
