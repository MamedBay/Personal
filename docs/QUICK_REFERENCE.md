# Quick Reference Guide

## Common Commands

### View Documentation
```bash
# Open the documentation index
cat docs/README.md

# List all projects
ls docs/projects/

# List all decisions
ls docs/decisions/

# View a specific project
cat docs/projects/knowledge-repository.md
```

### Create New Documentation

#### New Project Documentation
```bash
# Copy the template
cp docs/templates/project-template.md docs/projects/your-project-name.md

# Edit the new file
nano docs/projects/your-project-name.md

# Commit
git add docs/projects/your-project-name.md
git commit -m "Add documentation for your-project-name"
```

#### New Architecture Decision Record
```bash
# Copy the template with today's date
cp docs/templates/adr-template.md docs/decisions/$(date +%Y-%m-%d)-your-decision-title.md

# Edit the new file
nano docs/decisions/$(date +%Y-%m-%d)-your-decision-title.md

# Commit
git add docs/decisions/$(date +%Y-%m-%d)-your-decision-title.md
git commit -m "ADR: Your decision title"
```

## File Naming Conventions

### Project Documentation
- Location: `docs/projects/`
- Format: `project-name.md`
- Example: `docs/projects/web-application.md`

### Decision Records
- Location: `docs/decisions/`
- Format: `YYYY-MM-DD-decision-title.md`
- Example: `docs/decisions/2025-11-18-use-docker.md`

### Templates
- Location: `docs/templates/`
- Format: `template-name-template.md`
- Example: `docs/templates/project-template.md`

## GitHub Copilot Tips

### How Copilot Uses This Repository
1. Copilot reads `.github/copilot-instructions.md` for context
2. It references project docs when making suggestions
3. It understands the repository structure from documentation
4. It can suggest code/docs that align with existing patterns

### Maximizing Copilot Effectiveness
- Keep documentation up-to-date
- Use descriptive file names
- Cross-reference related documents
- Include examples in documentation
- Follow the templates consistently

### Example Copilot Prompts
When working in this repository, you can ask Copilot:
- "Create documentation for a new Python web service"
- "Record a decision about database choice"
- "Generate a project overview for a mobile app"
- "Create an ADR for switching to microservices"

Copilot will use the templates and existing docs to provide relevant suggestions.

## Directory Structure Overview

```
Personal/
├── .github/
│   └── copilot-instructions.md    # Instructions for GitHub Copilot
│
├── docs/
│   ├── README.md                   # Documentation hub
│   │
│   ├── projects/                   # Project documentation
│   │   ├── knowledge-repository.md
│   │   └── [your-project].md
│   │
│   ├── decisions/                  # Architecture Decision Records
│   │   ├── 2025-11-18-use-copilot-instructions.md
│   │   └── [YYYY-MM-DD-title].md
│   │
│   └── templates/                  # Documentation templates
│       ├── project-template.md
│       └── adr-template.md
│
└── README.md                       # Repository overview
```

## Maintenance

### Regular Tasks
- Review and update project documentation when changes occur
- Add new ADRs when making significant technical decisions
- Keep Copilot instructions current with repository changes
- Archive or update outdated documentation

### Quality Checks
Before committing documentation:
- [ ] Followed the appropriate template
- [ ] Used consistent formatting
- [ ] Added cross-references where relevant
- [ ] Checked for spelling and grammar
- [ ] Included examples where helpful
- [ ] Updated the documentation index if needed
