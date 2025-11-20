# Documentation Index

Welcome to the personal knowledge repository! This repository contains documentation on various projects and serves as a central knowledge base.

## 📁 Structure

### Projects
Project-specific documentation is located in [`/docs/projects/`](./projects/).

Each project should have its own documentation file that includes:
- Project overview and purpose
- Technical stack and dependencies
- Setup and installation instructions
- Architecture and design decisions
- Usage examples
- Troubleshooting guide

### Decisions
Architecture Decision Records (ADRs) and important decisions are documented in [`/docs/decisions/`](./decisions/).

Decision records help track:
- Why certain approaches were chosen
- What alternatives were considered
- Context at the time of the decision
- Consequences and trade-offs

### Templates
Reusable templates for documentation are available in [`/docs/templates/`](./templates/).

Available templates:
- [Project Template](./templates/project-template.md) - For documenting new projects
- [ADR Template](./templates/adr-template.md) - For recording architectural decisions

## 🎯 Purpose

This repository serves as:
1. **Knowledge Base** - Centralized documentation for all projects
2. **Decision Log** - Historical record of important technical decisions
3. **Reference Material** - Templates and guidelines for future work
4. **Context Provider** - Information source for GitHub Copilot to make informed suggestions

## 🚀 Getting Started

### For New Projects
1. Copy the [project template](./templates/project-template.md)
2. Create a new file in `/docs/projects/`
3. Fill in all relevant sections
4. Link to related projects or decisions

### For Recording Decisions
1. Copy the [ADR template](./templates/adr-template.md)
2. Create a new file in `/docs/decisions/` with format: `YYYY-MM-DD-decision-title.md`
3. Document the context, options, and decision
4. Reference the ADR from relevant project documentation

## 📚 Best Practices

- Keep documentation close to the code when possible
- Update documentation when making changes
- Use clear, concise language
- Include examples and diagrams where helpful
- Cross-reference related documents
- Review and update documentation regularly

## 🤖 GitHub Copilot Integration

This repository is configured to help GitHub Copilot provide better suggestions:
- Copilot reads `.github/copilot-instructions.md` for context
- Project documentation helps Copilot understand architecture
- Decision records provide historical context
- Templates ensure consistency

When working in this repository, Copilot will use this documentation to:
- Suggest code that aligns with existing patterns
- Provide context-aware completions
- Follow established conventions
- Reference past decisions
