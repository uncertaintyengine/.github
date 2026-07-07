<div align="center">

<img width="128" height="128" src="../assets/icons/engine.svg" alt="Uncertainty Engine logo" />

# Uncertainty Engine

### A modular framework for building and integrating uncertainty-aware AI systems.

</div>

## Framework

The core framework repositories define the shared interfaces, API surface, and client tooling used across the Uncertainty Engine ecosystem.

| Repository                                        | Status                                                                                                                                                      | Description                                                  |
| ------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------ |
| [Core](https://github.com/uncertaintyengine/Core) | [![CI](https://github.com/uncertaintyengine/Core/actions/workflows/ci.yaml/badge.svg)](https://github.com/uncertaintyengine/Core/actions/workflows/ci.yaml) | Shared interfaces, models, validators, and type definitions. |
| [API](https://github.com/uncertaintyengine/API)   | [![CI](https://github.com/uncertaintyengine/API/actions/workflows/ci.yaml/badge.svg)](https://github.com/uncertaintyengine/API/actions/workflows/ci.yaml)   | Streaming API for Uncertainty Engine services.               |

## Adapters

Adapters provide interchangeable implementations for ports.

### Client

Client libraries for interacting with the Uncertainty Engine API.

| Adapter                                                             | Status                                                                                                                                                                                      | Description                                                            |
| ------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------- |
| [Python](https://github.com/uncertaintyengine/ClientAdapter-Python) | [![CI](https://github.com/uncertaintyengine/ClientAdapter-Python/actions/workflows/ci.yaml/badge.svg)](https://github.com/uncertaintyengine/ClientAdapter-Python/actions/workflows/ci.yaml) | Python client library for interacting with the Uncertainty Engine API. |

### Authentication

Authentication adapters for verifying and authorising requests to the Uncertainty Engine API.

| Adapter                                                                       | Status                                                                                                                                                                                                        | Description                                                                                                  |
| ----------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------ |
| [Static](https://github.com/uncertaintyengine/AuthenticationAdapter-Static)   | [![CI](https://github.com/uncertaintyengine/AuthenticationAdapter-Static/actions/workflows/ci.yaml/badge.svg)](https://github.com/uncertaintyengine/AuthenticationAdapter-Static/actions/workflows/ci.yaml)   | Authentication adapter for verifying and authorising requests using a static credentials configuration file. |
| [Cognito](https://github.com/uncertaintyengine/AuthenticationAdapter-Cognito) | [![CI](https://github.com/uncertaintyengine/AuthenticationAdapter-Cognito/actions/workflows/ci.yaml/badge.svg)](https://github.com/uncertaintyengine/AuthenticationAdapter-Cognito/actions/workflows/ci.yaml) | Authentication adapter for verifying and authorising requests using AWS Cognito.                             |

### Cache

Fast key-value storage for shared state, intermediate results, and lightweight coordination.

| Adapter                                                          | Status                                                                                                                                                                                  | Description                                                                |
| ---------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------- |
| [RAM](https://github.com/uncertaintyengine/CacheAdapter-RAM)     | [![CI](https://github.com/uncertaintyengine/CacheAdapter-RAM/actions/workflows/ci.yaml/badge.svg)](https://github.com/uncertaintyengine/CacheAdapter-RAM/actions/workflows/ci.yaml)     | In-memory cache adapter for local development and lightweight deployments. |
| [Redis](https://github.com/uncertaintyengine/CacheAdapter-Redis) | [![CI](https://github.com/uncertaintyengine/CacheAdapter-Redis/actions/workflows/ci.yaml/badge.svg)](https://github.com/uncertaintyengine/CacheAdapter-Redis/actions/workflows/ci.yaml) | Redis-backed cache adapter for shared or distributed deployments.          |

### Data Residency

Read and write large files, datasets, artefacts, and other persisted data.

| Adapter                                                                            | Status                                                                                                                                                                                                            | Description                                    |
| ---------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------- |
| [Filesystem](https://github.com/uncertaintyengine/DataResidencyAdapter-Filesystem) | [![CI](https://github.com/uncertaintyengine/DataResidencyAdapter-Filesystem/actions/workflows/ci.yaml/badge.svg)](https://github.com/uncertaintyengine/DataResidencyAdapter-Filesystem/actions/workflows/ci.yaml) | Data residency adapter for a local filesystem. |
| [S3](https://github.com/uncertaintyengine/DataResidencyAdapter-S3)                 | [![CI](https://github.com/uncertaintyengine/DataResidencyAdapter-S3/actions/workflows/ci.yaml/badge.svg)](https://github.com/uncertaintyengine/DataResidencyAdapter-S3/actions/workflows/ci.yaml)                 | Data residency adapter for AWS S3.             |

### Execution

Run workloads using interchangeable execution backends.

| Adapter                                                            | Status                                                                                                                                                                                        | Description                                                                 |
| ------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------- |
| [Venv](https://github.com/uncertaintyengine/ExecutionAdapter-Venv) | [![CI](https://github.com/uncertaintyengine/ExecutionAdapter-Venv/actions/workflows/ci.yaml/badge.svg)](https://github.com/uncertaintyengine/ExecutionAdapter-Venv/actions/workflows/ci.yaml) | Execution adapter for running workloads inside Python virtual environments. |
