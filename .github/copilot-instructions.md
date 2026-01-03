# GitHub Copilot Instructions for `.github` Repository

This repository contains organization-wide GitHub community health files and VS Code workspace configuration for VOLT-BOX (Volt IQ).

## Repository Purpose

This is a **special `.github` repository** that provides default community health files for all repositories in the VOLT-BOX organization. Files here automatically apply to repos that don't have their own versions.

## Key Structure

-   **`profile/README.md`** - Organization profile displayed on github.com/VOLT-BOX
-   **`.github/ISSUE_TEMPLATE/`** - Issue form templates (YAML-based) for bug reports, feature requests, and tool requests
-   **`.vscode/`** - VS Code workspace configuration (excluded from git via `.gitignore`)

## Issue Template Conventions

All issue templates use **GitHub's YAML-based issue forms** (not legacy markdown templates):

### Bug Report Template (`bug-report.yml`)

-   **Targeted for Composio SDK users** (TypeScript/Python)
-   Structured fields: SDK language, version, runtime environment, deployment context
-   Requires minimal reproducible code examples with proper language syntax highlighting
-   Labels: `bug`, `needs-triage`

### Feature Request Template (`feature-request.yml`)

-   **Multi-area scope**: SDK, Dashboard, Integrations, MCP Server, Agentic Providers
-   Includes use case/motivation and impact assessment sections
-   Optional: API design proposals with code examples
-   Labels: `feature-request`, `enhancement`

### Tool Request Template (`tool-request.yml`)

-   **Redirects to external request board**: `https://request.composio.dev/boards/tool-requests`
-   This template does NOT collect information - it's purely instructional
-   Labels: `tool-request`, `integrations`

### Client Expert Request Template (`client-expert-request.yml`)

-   **Redirects to Microsoft Forms**: `https://forms.office.com/r/0dwK1iRzrm`
-   Collects only non-sensitive tracking info on GitHub (company name, expert title)
-   Full business requirements submitted via secure Microsoft Forms
-   Contact: ding.nie@volt-iq.com
-   Labels: `client-expert-request`, `expert-workflow`

## Editing Issue Templates

When modifying issue templates:

1. **Always use YAML syntax** - no markdown-based templates
2. **Field types**: `dropdown`, `textarea`, `input`, `checkboxes`, `markdown` (info only)
3. **Required validations**: Add `validations: required: true` for mandatory fields
4. **Code blocks in placeholders**: Use proper fenced code blocks with language identifiers
5. **Labels array**: Must be valid repository labels (create them first if needed)

Example field structure:

```yaml
- type: dropdown
  id: unique_field_id
  attributes:
      label: "Display Label"
      description: "Help text for the field"
      options:
          - Option 1
          - Option 2
      default: 0
  validations:
      required: true
```

## Organization Branding

**Volt IQ** is an Enterprise AI solutions company:

-   **Focus**: RAG technology, offline hosting, secure AI systems
-   **Contact**: Based in Lana, Bolzano, Italy
-   **GitHub Org**: VOLT-BOX (different from company name)

When updating `profile/README.md`, maintain:

-   Professional enterprise tone
-   Key technology highlights (RAG, Chain-of-Thought, Auto Annotation, Source Preview)
-   Security emphasis (offline hosting, "fully hackproof" messaging)

## VS Code Workspace Configuration

The `.vscode/` directory is **git-ignored** and contains team-specific settings:

-   `settings.json` - Custom title bar colors (blue: #128cff)
-   `folder-alias.json`, `private-folder-alias.json` - Local workspace aliases
-   `commands/` - Custom command definitions

Do not commit changes to `.vscode/` files - they are personal/team-local configurations.

## Common Tasks

### Add a new issue template

1. Create `ISSUE_TEMPLATE/<name>.yml` with proper YAML schema
2. Include `name`, `description`, `title` template, and `labels` array
3. Add structured `body` array with field definitions
4. Test the form on GitHub before committing

### Update organization profile

Edit `profile/README.md` - changes appear immediately on github.com/VOLT-BOX

### Check template validation

Push to GitHub and navigate to "New Issue" to verify rendering and validation rules
