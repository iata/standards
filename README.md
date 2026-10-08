# IATA Data Exchange Standards GitHub Repository

The IATA Data Exchange Standards GitHub Repository is a central place to discover and retrieve IATA data exchange standards artifacts from the latest release and historical releases. It supports consistent access, release traceability, and the use of standards by the airline and aviation industry stakeholders.

## Scope

Published releases include:

- OpenAPI specifications
- JSON Schemas
- XSD Schemas
- Other related technical artifacts and documents

IATA standards are published according to formal IATA release cycles. The published artifacts and release history are maintained in the [official Standards GitHub Repository](https://github.com/iata/standards). 

Published standard artifacts from the latest release can be accessed through the public [**IATA Data Exchange Standards Registry**](https://standards.developer.iata.org/). Individual artifacts can also be accessed directly using their Registry URL, for example: [https://standards.developer.iata.org/README.md](https://standards.developer.iata.org/README.md)

## Publication principles

- **Traceability:** Each published artifact is associated with an official IATA release, a Git tag, and a corresponding GitHub Release.
- **Historical access:** Latest and earlier published releases remain accessible to industry stakeholders.
- **Immutability:** Published tags, artifacts, and GitHub Releases are not changed after publication. Corrections are made available in a subsequent maintenance release.

## Intended use

Use the artifacts in the registry primarily during design and development for artifact discovery, dependency resolution, validation setup, code generation, and implementation onboarding. Retrieve, cache, and package the artifacts and dependencies required by your implementation as part of your build or deployment process.

**Do not depend on live retrieval from the IATA Standards Registry or GitHub Repository at production runtime.** Production systems should use locally managed copies in deployment packages or internal artifact repositories. The registry is a reference and distribution mechanism, not a runtime service with production service-level guarantees.

## Repository layout

By default, published standards artifacts governed under the IATA [Passenger Standards Conference](https://www.iata.org/en/about/corporate-structure/passenger-standards-conference/) are located under `psc/`.

```text
/
├── README.md
└── psc/
     └── Standards artifacts
```

## Find a release

- **Latest published artifacts:** Browse the `main` branch of the [Standards GitHub Repository](https://github.com/iata/standards) or use the [Standards Registry](https://standards.developer.iata.org/). 

- **A specific or historical release:** Open the [repository's Releases page](https://github.com/iata/standards/releases), select the IATA release number, to access its release notes, artifacts, and publication date.
