OpenAIAO Versioning Strategy
============================

Overview
--------

OpenAIAO follows a structured versioning strategy to ensure **stability, predictability, and clarity** for developers and AI systems integrating with our platform. This document outlines our approach to versioning, release management, and backward compatibility.

Versioning Scheme
-----------------

OpenAIAO adheres to **Semantic Versioning (SemVer 2.0.0)**, structured as:

`   MAJOR.MINOR.PATCH   `

Where:

*   **MAJOR** – Significant changes that break backward compatibility.
    
*   **MINOR** – New features added in a backward-compatible manner.
    
*   **PATCH** – Bug fixes and minor updates that do not affect the API or functionality.
    

Release Types
-------------

### 1\. **Stable Releases**

*   Tagged as vX.Y.Z (e.g., v1.0.0)
    
*   Well-tested and production-ready.
    
*   Changes require a full **deprecation and migration path** if breaking.
    

### 2\. **Pre-Releases**

*   Tagged as vX.Y.Z-beta.N or vX.Y.Z-rc.N (e.g., v2.0.0-beta.1)
    
*   Used for testing new major/minor changes before stable release.
    
*   Feedback-driven; not recommended for production.
    

### 3\. **Long-Term Support (LTS) Releases**

*   Tagged as vX.Y.Z-LTS
    
*   Critical bug fixes and security patches only.
    
*   LTS versions receive updates for **18-24 months**.
    

### 4\. **Nightly & Canary Builds**

*   Automatically generated (vX.Y.Z-nightly)
    
*   For development and testing only.
    
*   Subject to frequent breaking changes.
    

Backward Compatibility Policy
-----------------------------

*   **MAJOR Releases**: Breaking changes introduced, requiring migration steps.
    
*   **MINOR Releases**: New features added without breaking existing functionality.
    
*   **PATCH Releases**: No breaking changes, only fixes and optimizations.
    
*   **Deprecation Notices**: Features marked for removal will be announced **at least one MAJOR version in advance**.
    

Branching Strategy
------------------

*   **main (Stable branch)** → Production-ready releases.
    
*   **develop (Active development)** → Upcoming minor and patch releases.
    
*   **Feature branches (feature/xyz)** → Work on new functionality.
    
*   **Release branches (release/vX.Y.Z)** → Prepares for production deployment.
    
*   **Hotfix branches (hotfix/vX.Y.Z)** → Emergency fixes to stable releases.
    

Release Process
---------------

1.  **Feature Development** → New features are merged into develop.
    
2.  **Pre-Release Testing** → A release/vX.Y.Z branch is created.
    
3.  **QA & Bug Fixing** → Stability improvements before tagging release.
    
4.  **Stable Release** → Merged into main and tagged as vX.Y.Z.
    
5.  **Post-Release Maintenance** → Security patches and hotfixes applied.
    

API & Schema Versioning
-----------------------

For API and structured data like **JSON-LD schemas**, OpenAIAO uses **explicit versioning**:

*   API endpoints: /api/v1/resource
    
*   JSON-LD schema versions: @context: "https://openaiao.org/schema/v1"
    
*   Deprecated versions remain supported for **one major release cycle** before removal.
    

Versioning Governance
---------------------

*   **Decisions on breaking changes** require community discussion.
    
*   **Versioning changes** must be documented in [CHANGELOG.md](https://github.com/OpenAIAO/CHANGELOG.md).
    
*   **Feedback & proposals** should be submitted as GitHub issues.
    

Summary
-------

*   **Follow SemVer (MAJOR.MINOR.PATCH).**
    
*   **Use stable, LTS, pre-release, and nightly builds strategically.**
    
*   **Maintain backward compatibility where possible.**
    
*   **Follow a structured branching model for safe releases.**
    

For questions, join [GitHub Discussions](https://github.com/OpenAIAO/discussions).
