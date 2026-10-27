# AUTOSAR Adaptive Platform Training Guides

A series of training guides for engineers who are new to the AUTOSAR Adaptive Platform (AP). Each guide explains one functional cluster or topic in plain language: what it does, how it works, how to configure it and how to use its C++ API. The guides are based on the official AUTOSAR specifications, release **R25-11**, and on reputable public sources.

> **Author:** Hieu Do Minh/Claude

## Who These Guides Are For

- **Application developers** who write software that runs on the Adaptive Platform.
- **Integrators** who configure manifests, deploy software and debug ECUs.
- **Platform developers** who build or extend functional clusters.

Assumed background: modern C++, plus basic Linux/POSIX knowledge (processes, signals, sockets). No prior AUTOSAR knowledge is needed. AUTOSAR Classic experience helps but is optional.

## The Guides

Start with guide 00. It suggests shorter reading paths for specific roles, holds the glossary of the whole series and defines the running example. Otherwise, read the guides in the order of their numbers. Each guide can also be read on its own: it briefly recaps what it needs from other guides and links to them.

| # | Guide | Status |
| --- | --- | --- |
| 00 | [Learning Path, Series Glossary and Running Example](guides/00_LearningPath.md) | Available (v1.0) |
| 01 | [Adaptive Platform Overview and Architecture](guides/01_PlatformOverview.md) | In review |
| 02 | [Manifests and Methodology](guides/02_Manifests.md) | In review |
| 03 | [`ara::core` and General Conventions](guides/03_CoreAndGeneral.md) | In review |
| 04 | [Execution Management](guides/04_ExecutionManagement.md) | Available (v1.0) |
| 05 | State Management | Planned |
| 06 | Platform Health Management | Planned |
| 07 | Communication Management Part 1: `ara::com` Concepts and API | Planned |
| 08 | Communication Management Part 2: Network Bindings and Signal-to-Service Translation | Planned |
| 09 | Network Management, Time Synchronization and Raw Data Stream | Planned |
| 10 | Log and Trace | Planned |
| 11 | Persistency | Planned |
| 12a | Diagnostics Part 1 | Planned |
| 12b | Diagnostics Part 2 | Planned |
| 13 | Update and Configuration Management | Planned |
| 14 | Cryptography | Planned |
| 15 | Identity and Access Management | Planned |
| 16 | Intrusion Detection System Manager and Firewall | Planned |
| 17 | End-to-End Integration: A Day in the Life of the HPC | Planned |

The version in brackets is the current version of the guide. It increases when a revised guide is published.

All guides share one running example: an invented high-performance ECU called **HPC** that runs an ADAS feature. Every guide shows its topic on this example, so the pieces fit together as you read on.

## How the Guides Are Built

Every guide follows the same structure:

1. **About This Guide:** audience, learning objectives and the running example.
2. **Concept chapters:** each starts with *Why this matters* and ends with *Key takeaways*.
3. **Configuration:** what you must configure and where, what each setting means, its allowed values, its default and its effect at run time, plus a minimal configuration checklist.
4. **API chapter:** the `ara::` C++ interface with usage examples.
5. **Practice:** an end-to-end walkthrough, best practices, pitfalls and troubleshooting.
6. **Self-check quiz** with answers.
7. **Appendices:** glossary, cheat sheet, traceability to the specification, and notable changes between releases.

Conventions used throughout:

| Convention | Meaning |
| --- | --- |
| `[SWS_EM_01050]` | A requirement ID in the AUTOSAR specification. Search for it in the specification to read the exact normative text. |
| **Note (implementation example)** | How a typical implementation *might* realize something. This is not mandated by AUTOSAR. |
| **Pitfall** | A common mistake seen in real projects. |

## Viewing the Guides

The guides are plain Markdown with [Mermaid](https://mermaid.js.org/) diagrams. They render natively on GitHub and GitLab. In VS Code, install the *Markdown Preview Mermaid Support* extension.

## The AUTOSAR Specifications

The guides cite the specifications but do not include them. You can download them free of charge from <https://www.autosar.org/standards> (Adaptive Platform and Foundation, release R25-11). Guide 01 also cites two documents of the Classic Platform R25-11.

## Disclaimer

These guides are training material, not a normative reference. Where a guide and an AUTOSAR specification differ, the specification applies.
