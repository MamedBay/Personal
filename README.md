# Personal Knowledge Repository

This repository contains documentation on the projects I work on and functions as a shared project knowledge base.

## 🎯 Purpose

This repository is designed to:
- **Document projects** with comprehensive technical details
- **Record decisions** through Architecture Decision Records (ADRs)
- **Provide context** for GitHub Copilot to make informed suggestions
- **Serve as a reference** for future work and team members

## 📁 Structure

```
Personal/
├── .github/
│   └── copilot-instructions.md    # GitHub Copilot context and guidelines
├── docs/
│   ├── README.md                   # Documentation hub and index
│   ├── projects/                   # Project-specific documentation
│   ├── decisions/                  # Architecture Decision Records
│   └── templates/                  # Reusable documentation templates
└── README.md                       # This file
```

## 🚀 Getting Started

### For New Projects
1. Copy the [project template](./docs/templates/project-template.md)
2. Create a new file in `/docs/projects/`
3. Fill in all relevant sections
4. Commit your documentation

### For Recording Decisions
1. Copy the [ADR template](./docs/templates/adr-template.md)
2. Create a new file in `/docs/decisions/` with format: `YYYY-MM-DD-decision-title.md`
3. Document the context, options, and decision
4. Link from relevant project documentation

## 🤖 GitHub Copilot Integration

This repository is configured to help GitHub Copilot provide better, context-aware suggestions:

- **Copilot Instructions**: The `.github/copilot-instructions.md` file provides Copilot with repository context, conventions, and guidelines
- **Structured Documentation**: Organized project docs help Copilot understand architecture and patterns
- **Decision Records**: ADRs give Copilot historical context about why certain approaches were chosen
- **Templates**: Ensure consistency in documentation and Copilot suggestions

When you work in this repository with GitHub Copilot enabled, it will:
- Suggest documentation that follows established conventions
- Reference existing project information
- Provide context-aware completions
- Follow the repository's organizational structure

## 📚 Documentation

For detailed information, see the [Documentation Index](./docs/README.md).

Available resources:
- [Project Template](./docs/templates/project-template.md)
- [ADR Template](./docs/templates/adr-template.md)
- [Example Project Documentation](./docs/projects/knowledge-repository.md)
- [Example ADR](./docs/decisions/2025-11-18-use-copilot-instructions.md)

## 🤝 Contributing

1. Follow the existing documentation structure
2. Use the provided templates
3. Keep documentation clear and concise
4. Cross-reference related documents
5. Update the documentation index when adding new files

## 📖 Learn More

- [GitHub Copilot Documentation](https://docs.github.com/en/copilot)
- [Markdown Guide](https://www.markdownguide.org/)
- [Architecture Decision Records](https://adr.github.io/)
