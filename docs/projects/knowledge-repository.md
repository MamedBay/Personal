# Personal Knowledge Repository

## Overview
This repository serves as a centralized knowledge base for documenting projects, architectural decisions, and shared learnings.

## Status
- **Current Status**: Active
- **Last Updated**: 2025-11-18
- **Maintained By**: Repository Owner

## Purpose
The Personal Knowledge Repository exists to:
1. Provide a single source of truth for project documentation
2. Enable GitHub Copilot to make informed suggestions based on existing context
3. Track architectural decisions and their rationale
4. Serve as a reference for future projects and team members

## Technical Stack

### Languages
- Primary: Markdown
- Secondary: N/A (documentation-focused repository)

### Frameworks & Libraries
- GitHub-flavored Markdown
- Mermaid diagrams (for visual documentation)

### Infrastructure
- Hosting: GitHub Pages (optional)
- Version Control: Git/GitHub

## Architecture

### High-Level Overview
The repository is structured to provide clear separation between different types of documentation:
- Project-specific docs in `/docs/projects/`
- Decision records in `/docs/decisions/`
- Reusable templates in `/docs/templates/`

### Key Components
1. **Copilot Instructions**: `.github/copilot-instructions.md` provides context for AI-assisted development
2. **Documentation Hub**: `/docs/README.md` serves as the entry point for all documentation
3. **Templates**: Standardized formats ensure consistency across documentation
4. **Project Docs**: Individual project documentation with detailed technical information
5. **ADRs**: Architecture Decision Records capture important choices and their context

### Data Flow
1. Developer creates/updates documentation using templates
2. Documentation is committed to repository
3. GitHub Copilot reads `.github/copilot-instructions.md` and project docs
4. Copilot provides context-aware suggestions based on existing documentation
5. Future developers reference documentation for understanding and consistency

## Setup & Installation

### Prerequisites
- Git installed
- GitHub account
- Text editor (VS Code recommended for GitHub Copilot integration)

### Installation Steps
```bash
# Clone the repository
git clone https://github.com/MamedBay/Personal.git

# Navigate to the repository
cd Personal

# Start documenting!
```

### Configuration
No specific configuration required. For GitHub Copilot integration:
- Ensure GitHub Copilot extension is installed in your IDE
- Copilot will automatically read `.github/copilot-instructions.md`

## Usage

### Basic Usage
To add new documentation:
1. Choose the appropriate template from `/docs/templates/`
2. Copy the template to the appropriate location
3. Fill in the sections
4. Commit and push

### Common Scenarios
1. **Documenting a New Project**:
   ```bash
   cp docs/templates/project-template.md docs/projects/my-new-project.md
   # Edit the file with your project details
   git add docs/projects/my-new-project.md
   git commit -m "Add documentation for my new project"
   ```

2. **Recording an Architectural Decision**:
   ```bash
   cp docs/templates/adr-template.md docs/decisions/2025-11-18-use-markdown-for-docs.md
   # Fill in the decision details
   git add docs/decisions/2025-11-18-use-markdown-for-docs.md
   git commit -m "ADR: Use Markdown for documentation"
   ```

## Development

### Getting Started
This is primarily a documentation repository. To contribute:
1. Fork the repository
2. Create a new branch for your changes
3. Add or update documentation
4. Submit a pull request

### Documentation Standards
- Use Markdown for all documents
- Follow the template structure
- Include examples where helpful
- Keep documentation up-to-date
- Cross-reference related docs

## Key Decisions

### Architecture Decisions
The structure of this repository was designed to:
- Make it easy for GitHub Copilot to find relevant context
- Provide clear organization for different types of documentation
- Enable quick onboarding for new projects
- Maintain historical context through ADRs

### Technology Choices
**Markdown**: Chosen for its simplicity, wide support, and readability in both raw and rendered forms.

**GitHub Copilot Instructions**: Using `.github/copilot-instructions.md` allows Copilot to provide better, more context-aware suggestions.

## Troubleshooting

### Common Issues
**Issue**: GitHub Copilot not using repository context  
**Solution**: Ensure `.github/copilot-instructions.md` exists and is properly formatted. Copilot needs to index the file, which may take a few minutes after creation.

**Issue**: Can't find the right template  
**Solution**: Check `/docs/templates/` directory. All available templates are listed in `/docs/README.md`.

**Issue**: Unsure where to place new documentation  
**Solution**: 
- Project-specific docs → `/docs/projects/`
- Architectural decisions → `/docs/decisions/`
- New templates → `/docs/templates/`

## Related Projects
This repository can reference other projects you're working on. Add links here as needed.

## Resources
- [GitHub Copilot Documentation](https://docs.github.com/en/copilot)
- [Markdown Guide](https://www.markdownguide.org/)
- [Architecture Decision Records](https://adr.github.io/)

## Changelog

### Initial Setup - 2025-11-18
- Added GitHub Copilot instructions
- Created documentation structure
- Added project and ADR templates
- Set up example documentation
