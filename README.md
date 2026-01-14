<div align="center">

# 🏭 Industrial Signal Platform (ISP)

[![TypeScript](https://img.shields.io/badge/TypeScript-5.0-blue.svg)](https://www.typescriptlang.org/)
[![React](https://img.shields.io/badge/React-18.x-61dafb.svg)](https://reactjs.org/)
[![Vite](https://img.shields.io/badge/Vite-6.x-646cff.svg)](https://vitejs.dev/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Version](https://img.shields.io/badge/Version-2.4.0-orange.svg)](#)

**A desktop-native, local-first engineering environment for industrial signal management.**

[Features](#-features) • [Quick Start](#-quick-start) • [Documentation](#-documentation) • [Libraries](#-libraries) • [Contributing](#-contributing)

</div>

---

## 📋 Overview
The **Industrial Signal Platform (ISP)** is a comprehensive engineering software designed to achieve the functional density and reliability of industry leaders such as **AUCOTEC Engineering Base**, **EPLAN Electric P8**, and **Siemens TIA Portal**.

### Core Philosophy
| Principle | Description |
| :--- | :--- |
| 🏠 **Local-First** | Resilience against network failure and high-speed local data processing. |
| 🔒 **Type-Safe** | Strict TypeScript enforcement for industrial data integrity. |
| 📊 **High-Density** | Optimized for complex, data-heavy engineering workflows. |
| 🔌 **Signal-Centric** | `OUTPUT → INPUT` polarity validation at the core of every connection. |

---

## ✨ Features

### ✅ Currently Implemented
* **Authentication & RBAC:** Login/logout with 4 roles and 16 granular permissions.
* **User Interfaces:** * Classic tabbed interface (Hierarchy, Devices, Connections, Audit, Users).
    * Modern IDE Workspace (toggle via purple button in toolbar).
* **Device Management:** * Creation from **111+ templates**.
    * Signal connections with real-time `OUTPUT → INPUT` validation.
    * Comprehensive audit trail logging for every change.
* **Compatibility Engine:** Soft validation with 5 compatibility levels for Protocol-Cable matching.
* **AI Collaboration:** Built-in `CLAUDE.md` rules and a code-bundling system for LLM-assisted development.
* **Testing:** 110+ passing tests with Vitest.

### 🔜 Coming Soon
* [ ] Generic Panels/Devices/Cables creation UI.
* [ ] Electron desktop shell integration.
* [ ] SQLite persistence layer.
* [ ] File save/load system (`.isp` files).
* [ ] Import/Export (Excel, CSV).

---

## 🚀 Quick Start

### Prerequisites
* **Node.js**: `22.14.0 LTS` or higher
* **npm**: `10.x` or higher

### Installation
```bash
# Clone the repository
git clone [https://github.com/Oluwasedago/SE_Design.git](https://github.com/Oluwasedago/SE_Design.git)

# Navigate to project directory
cd SE_Design

# Install dependencies
npm install

# Start development server
npm run dev
The application will be available at http://localhost:5173.Available ScriptsCommandDescriptionnpm run devStart development servernpm run buildCreate production buildnpm run testRun test suite (110+ tests)npm run test:coverageRun tests with coverage reportnpx tsc --noEmitRun TypeScript type check📁 Project StructurePlaintextindustrial-signal-platform/
├── 📂 .ai/                 # AI collaboration system (Rules & Bundles)
├── 📂 Docs/                # ADRs, Roadmap, and Guides
├── 📂 electron/            # Electron shell (planned)
├── 📂 src/
│   ├── 📂 core/            # Business logic, factories, and services
│   ├── 📂 database/        # Persistence layer (planned)
│   ├── 📂 library/         # ⚡ MASTER LIBRARIES (Devices/Protocols/Cables)
│   │   ├── 📂 devices/     # 111+ Industrial templates
│   │   ├── 📂 protocols/   # 32 Communication protocols
│   │   └── 📂 cables/      # 38 Cable specifications
│   ├── 📂 renderer/        # React components, hooks, and stores
│   └── main.tsx            # Entry point
└── vite.config.ts          # Build configuration
📚 LibrariesDevice Library (111+ Templates)IconCategoryTemplates⚡Power Systems18🛡️Substations & Protection9🕹️Manufacturing PLCs~15⚙️Manufacturing Drives7🔬Process Instrumentation26🖥️Process Control19🛢️Oil & Gas25🏢Building Automation16Protocol & Cable CompatibilityThe system uses a 5-level validation engine to ensure engineering integrity:LevelIconMeaningVERIFIED✅Industry-standard combinationCOMPATIBLE⚠️Works with minor advisoriesUNVERIFIED❓User-defined, not in libraryUNLIKELY⛔Physical mismatchPENDING📋Generic placeholder📖 Industry Standards ReferencedISP is built against global engineering standards:Instrumentation: ISA 5.1, IEC 61508, IEC 61511Power: IEC 61850, IEEE 1815 (DNP3), IEEE C37.118Cables: UL 83/44, NEC Article 310, TIA/EIA-568Compliance: 21 CFR Part 11, GAMP 5, NERC CIP🤖 AI Collaboration SystemThis project is optimized for AI-assisted development (Claude/ChatGPT).Bundling: Use node .ai/scripts/bundle-split.cjs to generate context bundles for AI.Rules: Refer to CLAUDE.md for project-specific coding standards.🤝 ContributingFork the repository.Create a feature branch: git checkout -b feature/YourFeature.Commit changes: git commit -m 'Add YourFeature'.Push to branch: git push origin feature/YourFeature.Open a Pull Request.[!IMPORTANT]Always run npm run test and npx tsc --noEmit before submitting a PR.📄 LicenseThis project is licensed under the MIT License - see the LICENSE file for details.<div align="center">Built with ❤️ for Industrial EngineersVersion 2.4.0 • 2025-01-14⬆ Back to Top
