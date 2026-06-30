<div align="center">

<img width="128" height="128" src="../assets/icons/engine.svg" alt="Uncertainty Engine logo" />

# Uncertainty Engine

### A modular framework for building and integrating uncertainty-aware AI systems.

</div>

## Framework

The core framework repositories define the shared interfaces, API surface, and client tooling used across the Uncertainty Engine ecosystem.

| Repository                                        | Status                                                                                                                                                      | Description                                                     |
| ------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------- |
| [Core](https://github.com/uncertaintyengine/core) | [![CI](https://github.com/uncertaintyengine/core/actions/workflows/ci.yaml/badge.svg)](https://github.com/uncertaintyengine/core/actions/workflows/ci.yaml) | Shared interfaces, models, validators, and type definitions.    |
| [API](https://github.com/uncertaintyengine/api)   | TODO                                                                                                                                                        | RESTful HTTP API for serving and orchestrating engine services. |
| [SDK](https://github.com/uncertaintyengine/sdk)   | TODO                                                                                                                                                        | Python client for interacting with the Uncertainty Engine API.  |

## Adapters

Adapters provide interchangeable implementations for service backends.

### Cache Service

Fast key-value storage for shared state, intermediate results, and lightweight coordination.

| Adapter                                                          | Status                                                                                                                                                                                  | Description                                                                |
| ---------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------- |
| [RAM](https://github.com/uncertaintyengine/CacheAdapter-RAM)     | [![CI](https://github.com/uncertaintyengine/CacheAdapter-RAM/actions/workflows/ci.yaml/badge.svg)](https://github.com/uncertaintyengine/CacheAdapter-RAM/actions/workflows/ci.yaml)     | In-memory cache adapter for local development and lightweight deployments. |
| [Redis](https://github.com/uncertaintyengine/CacheAdapter-Redis) | [![CI](https://github.com/uncertaintyengine/CacheAdapter-Redis/actions/workflows/ci.yaml/badge.svg)](https://github.com/uncertaintyengine/CacheAdapter-Redis/actions/workflows/ci.yaml) | Redis-backed cache adapter for shared or distributed deployments.          |

### Resource Service

Read and write large files, datasets, artefacts, and other persisted resources.

| Adapter                                                                                  | Status                                                                                                                                                                                                            | Description                                                             |
| ---------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------- |
| [Local Filesystem](https://github.com/uncertaintyengine/ResourceAdapter-LocalFilesystem) | [![CI](https://github.com/uncertaintyengine/ResourceAdapter-LocalFilesystem/actions/workflows/ci.yaml/badge.svg)](https://github.com/uncertaintyengine/ResourceAdapter-LocalFilesystem/actions/workflows/ci.yaml) | Resource adapter for reading and writing files on the local filesystem. |

### Execution Service

Run workloads using interchangeable execution backends.

| Adapter                                                            | Status                                                                                                                                                                                        | Description                                                                 |
| ------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------- |
| [Venv](https://github.com/uncertaintyengine/ExecutionAdapter-Venv) | [![CI](https://github.com/uncertaintyengine/ExecutionAdapter-Venv/actions/workflows/ci.yaml/badge.svg)](https://github.com/uncertaintyengine/ExecutionAdapter-Venv/actions/workflows/ci.yaml) | Execution adapter for running workloads inside Python virtual environments. |
