# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [0.1.1][0.1.1] - 2025-12-13

### Added

- Initial release
- MQTTConnector for Niko Home Control 2 MQTT communication
- Device base class for generic device control
- Lamp class with on/off and brightness control
- NHC2FileReader for reading .nhc2 configuration files
- Support for TLS encryption and JWT authentication
- MessageHandler class for single device automation
- MultiMessageHandler class for multi-device automation

[0.1.1]: https://github.com/kevinghekiere/pynhc2/releases/tag/v0.1.1

## [0.1.2][0.1.2] - 2026-03-12

### Changed

- Made the MessageHandler and MultiMessageHandler classes stateful: added 'state' attribute that toggles between off/on

[0.1.2]: https://github.com/kevinghekiere/pynhc2/releases/tag/v0.1.2


## [0.1.3][0.1.3] - 2026-03-13

### Changed

- Fixed feedback loop in MessageHandler and MultimessageHandler classes by adding cooldown period

[0.1.3]: https://github.com/kevinghekiere/pynhc2/releases/tag/v0.1.2
