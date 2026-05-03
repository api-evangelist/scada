# SCADA

SCADA (Supervisory Control and Data Acquisition) is an industrial control system architecture used to monitor and control industrial processes, infrastructure, and facility-based equipment. It is widely used in manufacturing, energy, water treatment, oil and gas, transportation, and other critical infrastructure sectors to collect real-time data from remote sensors and control equipment. Modern SCADA systems increasingly expose REST APIs, OPC-UA endpoints, and MQTT brokers for integration with enterprise systems and cloud platforms.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/scada/refs/heads/main/apis.yml)

- **Standards Body:** https://opcfoundation.org/
- **ISA:** https://www.isa.org/
- **CISA ICS Resources:** https://www.cisa.gov/topics/industrial-control-systems

## Scope

- **Type:** Index
- **Position:** Consuming
- **Access:** 3rd-Party

## Tags

SCADA, Industrial Automation, ICS, Industrial IoT, OT Security, Critical Infrastructure

## Timestamps

- **Created:** 2025-01-01
- **Modified:** 2026-05-02

## APIs and Protocols

### OPC Unified Architecture (OPC-UA)

OPC-UA (IEC 62541) is the industrial interoperability standard for secure, reliable data exchange in industrial automation and IoT environments. Supports client/server and pub/sub models for SCADA tag access.

**Human URL:** https://opcfoundation.org/about/opc-technologies/opc-ua/

**Tags:** OPC-UA, IEC 62541, Industrial Interoperability, Real-Time Data

**Properties**

- [Documentation](https://opcfoundation.org/about/opc-technologies/opc-ua/)
- [Specification](https://reference.opcfoundation.org/Core/Part1/v105/docs/)

### MQTT Protocol

MQTT (ISO/IEC 20922) is a lightweight pub/sub messaging protocol used in SCADA and IIoT for high-volume sensor data streaming via brokers such as Mosquitto, EMQX, and HiveMQ.

**Human URL:** https://mqtt.org/

**Tags:** MQTT, IoT, Messaging, Pub/Sub, Telemetry

### Modbus Protocol

Modbus is the most widely deployed field device protocol in SCADA, enabling communication with PLCs and RTUs over serial and TCP/IP networks.

**Human URL:** https://modbus.org/

**Tags:** Modbus, Field Protocol, PLC, Industrial Automation

### Ignition SCADA REST API

Inductive Automation's Ignition SCADA platform provides a REST API for reading and writing tag values, managing alarms, and retrieving historical data.

**Human URL:** https://docs.inductiveautomation.com/

### Historian and Alarm Data APIs

Major historian vendors (AVEVA PI System, Aspen InfoPlus.21, GE Proficy Historian) expose REST APIs for querying historical process data.

**Human URL:** https://techsupport.osisoft.com/Documentation/PI-Web-API/

## JSON Schema

- [json-schema/scada-tag-schema.json](json-schema/scada-tag-schema.json) — Schema for SCADA tag data points including real-time value, quality, alarm limits, and device source
- [json-schema/scada-alarm-schema.json](json-schema/scada-alarm-schema.json) — Schema for SCADA alarm events including priority, state, timestamps, and operator acknowledgment

## JSON Structure

- [json-structure/scada-tag-structure.json](json-structure/scada-tag-structure.json) — Field-level documentation for the SCADA tag data structure

## JSON-LD

- [json-ld/scada-context.jsonld](json-ld/scada-context.jsonld) — Linked data context mapping SCADA concepts to W3C SOSA/SSN sensor ontologies and schema.org

## Examples

- [examples/scada-tag-reading-example.json](examples/scada-tag-reading-example.json) — Real-time tag reading from an Ignition SCADA REST API with OPC-UA quality codes

## Vocabulary

- [vocabulary/scada-vocabulary.yml](vocabulary/scada-vocabulary.yml) — SCADA domain vocabulary covering system architecture, process data, alarm management, communication protocols, and OT security

## Common Properties

- [Standards Body - OPC Foundation](https://opcfoundation.org/)
- [ISA - International Society of Automation](https://www.isa.org/)
- [IEC Standards](https://www.iec.ch/)
- [CISA ICS Resources](https://www.cisa.gov/topics/industrial-control-systems)
- [SCADA GitHub Topics](https://github.com/topics/scada)

## Maintainers

**FN:** Kin Lane  
**Email:** kin@apievangelist.com
