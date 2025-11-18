# ADR-001: Use GitHub Copilot Instructions for Context-Aware AI Assistance

**Date**: 2025-11-18  
**Status**: Accepted  
**Deciders**: Repository Owner  
**Tags**: github-copilot, documentation, ai-assistance

## Context and Problem Statement

GitHub Copilot can provide code suggestions and completions, but without proper context about the repository's structure, conventions, and purpose, its suggestions may not align with the project's goals or existing patterns.

How can we provide GitHub Copilot with enough context to make informed, relevant suggestions that align with our documentation standards and project structure?

## Decision Drivers

- Need for consistent documentation across projects
- Desire for GitHub Copilot to understand repository structure
- Want AI assistance that respects established conventions
- Requirement for maintainable and organized documentation
- Goal of reducing cognitive load when creating new documentation

## Considered Options

### Option 1: Use `.github/copilot-instructions.md`
Create a dedicated file that GitHub Copilot reads to understand project context, conventions, and structure.

**Pros:**
- Official GitHub Copilot feature designed for this purpose
- Automatically read by Copilot when present
- Can include detailed context, guidelines, and conventions
- Easy to update and maintain
- Visible to all contributors

**Cons:**
- Requires manual maintenance
- May become outdated if not regularly reviewed
- Limited to text-based instructions

### Option 2: Rely on README and inline comments
Use only existing README files and inline comments for context.

**Pros:**
- No additional files needed
- Documentation already exists
- Familiar to developers

**Cons:**
- Copilot may not prioritize README content
- Less structured guidance
- Harder to provide comprehensive context
- No centralized place for Copilot-specific instructions

### Option 3: No special configuration
Let Copilot work with whatever context it can infer from the code.

**Pros:**
- No additional work required
- Simplest approach

**Cons:**
- Inconsistent suggestions
- May not follow repository conventions
- Misses opportunity for better AI assistance
- No guidance on documentation structure

## Decision Outcome

**Chosen option**: "Option 1: Use `.github/copilot-instructions.md`"

### Rationale
The `.github/copilot-instructions.md` file is specifically designed for this use case and provides a structured way to give GitHub Copilot context about the repository. This aligns perfectly with the goal of enabling Copilot to "pull information from the existing files for requests on informed decisions."

By creating comprehensive instructions, we can:
1. Guide Copilot to understand our documentation structure
2. Ensure consistency across new documentation
3. Provide context about templates and conventions
4. Help Copilot make suggestions that align with our goals

### Consequences

**Positive:**
- GitHub Copilot will provide more relevant and context-aware suggestions
- New contributors can reference the same file to understand conventions
- Documentation quality and consistency will improve
- Reduced time spent on documentation setup
- Better alignment between AI suggestions and project goals

**Negative:**
- Requires maintaining another documentation file
- Need to keep instructions updated as the repository evolves
- May need to educate users about the file's purpose

**Neutral:**
- Adds one more file to the repository structure
- Creates a dependency on GitHub Copilot for optimal experience

## Implementation

### Steps
1. Create `.github` directory
2. Create `.github/copilot-instructions.md` file
3. Document repository structure and conventions
4. Include guidance for common tasks
5. Add references to templates and documentation
6. Test with GitHub Copilot to validate effectiveness

### Timeline
Implemented on 2025-11-18 as part of initial repository setup.

### Risks and Mitigation
- **Risk**: Instructions become outdated
  - **Mitigation**: Include regular review in documentation maintenance process

- **Risk**: Instructions become too long or complex
  - **Mitigation**: Keep instructions focused and well-organized with clear sections

## Validation

### Success Criteria
- GitHub Copilot suggests documentation that follows repository conventions
- New documentation created with Copilot assistance uses correct templates
- Suggestions reference appropriate existing files
- Documentation quality improves over time

### Monitoring
- Review Copilot suggestions periodically
- Gather feedback from users about suggestion quality
- Update instructions based on gaps or issues identified

## Links and References

- [GitHub Copilot Documentation](https://docs.github.com/en/copilot)
- [Copilot Instructions Feature](https://github.blog/changelog/2024-01-30-copilot-instructions-in-github-copilot-chat/)
- [Project Documentation](../projects/knowledge-repository.md)

## Notes

This decision was made as part of the initial repository setup to address the requirement: "I want github copilot to pull information from the existing files for requests on informed decisions."

The `.github/copilot-instructions.md` file serves as the primary mechanism for providing this context to Copilot.

---

## Revision History

| Date | Author | Changes |
|------|--------|---------|
| 2025-11-18 | Copilot Agent | Initial version |
