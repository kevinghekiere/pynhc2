# pynhc2 documentation

Python library for controlling Niko Home Control 2 devices via MQTT.

## Features

- MQTT connection to Niko Home Control 2 systems
- Device control (lamps, switches, dimmers)
- Automation handlers for multi-device triggers
- Configuration file reader for .nhc2 files

```{toctree}
:maxdepth: 2
:caption: Contents:

installation
quickstart
examples
api/index
```

## Quick Start

```python
from pynhc2 import MQTTConnector, Lamp

# Connect to broker
connector = MQTTConnector(
    broker="Niko1CA4.local",
    jwt="your-jwt-token",
    ca_cert="ca-chain.cert.pem"
)
connector.connect()

# Control a lamp
lamp = Lamp(mqttconnector=connector, device_uuid="device-uuid-here")
lamp.switch_on()
```

## Indices and tables

* {ref}`genindex`
* {ref}`modindex`
* {ref}`search`