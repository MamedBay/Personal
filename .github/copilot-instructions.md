# GitHub Copilot Instructions

## Repository Purpose
This is a personal knowledge repository that contains documentation on various projects and serves as a shared project knowledge base.

## Key Context for Copilot

### Repository Structure
- `/docs/` - Contains project documentation and knowledge base articles
- `/docs/projects/` - Individual project documentation
- `/docs/decisions/` - Architecture Decision Records (ADRs) and important decisions
- `/docs/templates/` - Templates for creating new documentation

### Documentation Standards
When creating or updating documentation:
1. Use clear, concise language
2. Follow the existing template structure in `/docs/templates/`
3. Include context about why decisions were made
4. Reference related documents when applicable
5. Keep a changelog section when appropriate

### Coding and Documentation Guidelines
- Use Markdown for all documentation
- Follow consistent heading hierarchy (# for title, ## for sections, ### for subsections)
- Include code examples where relevant
- Add links to related resources
- Keep documentation up-to-date with actual implementations

### Decision-Making Context
When suggesting code or documentation changes:
1. Check existing project documentation in `/docs/projects/`
2. Review past decisions in `/docs/decisions/`
3. Follow established patterns and conventions
4. Consider cross-project consistency
5. Prioritize maintainability and clarity

### File Naming Conventions
- Use lowercase with hyphens for file names (e.g., `project-name.md`)
- Use descriptive names that reflect content
- Date-prefix decision records: `YYYY-MM-DD-decision-title.md`

## Common Tasks

### Adding New Project Documentation
1. Create a new file in `/docs/projects/`
2. Use the template from `/docs/templates/project-template.md`
3. Fill in all relevant sections
4. Link to related projects if applicable

### Recording a Decision
1. Create a new ADR in `/docs/decisions/`
2. Use the template from `/docs/templates/adr-template.md`
3. Include context, options considered, and rationale
4. Update related project documentation

## References
- Main documentation index: `/docs/README.md`
- Project templates: `/docs/templates/`
- Existing projects: `/docs/projects/`
