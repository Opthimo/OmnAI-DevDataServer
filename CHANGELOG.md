## Changelog 

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

### Added
- Introduce **API versioning**; all endpoints now live under **`/v1/…`**.
- Introduce CORS rule to grant access to the server APIs for browser applications running on **`http://localhost:4200`** 
- Add javascript server example 
- Add .gitignore (#5)
- Add requirements.txt (#5)

### Changed
**BREAKING CHANGE**  
  - Move HTTP endpoint: `/UUID` → `/v1/get_devices`  
  - Move Websocket endpoint: `/ws` → `/v1/subscribe_ws`
  - Update README.md description (#5)
  - Registering sigint handlers for pyhton example (#9)

### Removed
- Remove un-versioned endpoints (`/UUID`, `/ws`).