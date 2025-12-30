<!-- Sync Impact Report:
Version change: N/A (initial creation) → 1.0.0
Added sections: All sections (new constitution)
Removed sections: None
Modified principles: N/A (new constitution)
Templates requiring updates: N/A (initial creation)
Follow-up TODOs: None
-->
# AI/Spec-Driven Book with Embedded RAG Chatbot Constitution

## Core Principles

### I. Spec-Driven Development (NON-NEGOTIABLE)
All development follows Spec-Kit Plus methodology with formal specifications, plans, and testable tasks. Every feature must be defined in spec.md before implementation begins, with corresponding plan.md architecture and tasks.md implementation steps. This ensures systematic, traceable, and reproducible development.

### II. Accuracy and Strict Grounding
All AI responses must be strictly grounded in indexed book content with zero hallucinations permitted. The RAG system may only reference full book content or user-selected text. No external knowledge sources are allowed in chatbot responses. Content accuracy is verified through citation to source material.

### III. Clear Technical Writing
All documentation, specifications, and user-facing content must follow clear, accessible technical writing standards. Content should be structured, well-organized, and comprehensible to the target audience. Code comments and documentation must be precise, helpful, and maintained alongside implementation changes.

### IV. Reproducible Builds and Deployments
All build processes and deployments must be fully reproducible with deterministic outcomes. Docusaurus builds must succeed consistently across environments. Deployment to GitHub Pages must follow automated, version-controlled processes with clear rollback procedures. Environment dependencies must be explicitly documented and managed.

### V. AI-Native Book + Chatbot Integration
The book platform must seamlessly integrate the RAG chatbot as a core feature. The chatbot must provide contextual responses based on book content with minimal latency. User experience must be intuitive and responsive across different devices and browsers. Integration points between book content and chatbot functionality must be well-defined and maintained.

### VI. Security and Data Protection
All user interactions and data must be handled securely with appropriate privacy protections. Secrets and API keys must be managed through environment variables, never hardcoded. Database connections must use secure protocols. User query logs and personal information must be protected according to privacy standards.

## Standards and Constraints

### Technology Stack Requirements
- Frontend: Docusaurus (Markdown/MDX) for documentation and book content
- Backend: FastAPI for RAG service and API endpoints
- Vector Database: Qdrant Cloud (Free Tier) for content indexing
- Database: Neon Serverless Postgres for user data and metadata
- SDKs: OpenAI Agents / ChatKit for AI integration
- Deployment: GitHub Pages for static content delivery

### Content and Integration Standards
- No hallucinations: RAG responses must cite source content
- RAG chatbot answers must come from indexed book content or user-selected text only
- Authoring must be done with Claude Code + Spec-Kit Plus tools
- Secrets must be managed via environment variables only
- External knowledge beyond indexed content is strictly prohibited

## Development Workflow

### Spec-First Development
- All features must begin with formal specification in spec.md
- Architectural decisions must be documented in plan.md
- Implementation tasks must be broken down in tasks.md
- Implementation follows the red-green-refactor cycle with testable tasks

### Quality Gates
- Docusaurus builds must complete without errors
- Chatbot responses must be verified for accuracy and grounding
- All code changes must pass security and dependency checks
- Performance benchmarks must meet defined thresholds

### Review Process
- All pull requests must include spec, plan, and task documentation
- Code reviews must verify compliance with constitutional principles
- Integration tests must validate RAG functionality and accuracy
- Deployment readiness must be confirmed before merging

## Governance

This constitution governs all development activities for the AI/Spec-Driven Book with Embedded RAG Chatbot project. All team members must adhere to these principles and standards. Amendments to this constitution require formal approval and must be documented with clear rationale. All pull requests and code reviews must verify compliance with these constitutional requirements. Deviations from these principles must be explicitly justified and approved.

**Version**: 1.0.0 | **Ratified**: 2025-12-23 | **Last Amended**: 2025-12-23