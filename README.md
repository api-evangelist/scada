# SCADA

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
