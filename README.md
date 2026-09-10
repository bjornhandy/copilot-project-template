# GitHub Copilot Project Template

Reusable project template for GitHub Copilot-powered development.

This repository provides a preconfigured Copilot setup with:

- Repository-wide instructions
- Language-specific instructions
- Custom agents
- Reusable skills
- Agent behavior rules
- Testing, debugging, database, API, and deployment guidance

The goal is to make every new project start with a consistent AI-assisted development setup.

---

## Included Structure

```text
.github/
├── copilot-instructions.md
│
├── instructions/
│   ├── python.instructions.md
│   ├── react.instructions.md
│   ├── database.instructions.md
│   └── tests.instructions.md
│
├── agents/
│   ├── backend.agent.md
│   ├── frontend.agent.md
│   ├── database.agent.md
│   ├── debugger.agent.md
│   ├── reviewer.agent.md
│   └── security.agent.md
│
└── skills/
    ├── python-backend/
    │   └── SKILL.md
    ├── react-typescript/
    │   └── SKILL.md
    ├── postgresql/
    │   └── SKILL.md
    ├── code-review/
    │   └── SKILL.md
    ├── testing/
    │   └── SKILL.md
    ├── debugging/
    │   └── SKILL.md
    ├── api-designer/
    │   └── SKILL.md
    ├── docker-deployment/
    │   └── SKILL.md
    └── database-migration/
        └── SKILL.md

AGENTS.md
```

---

## Purpose

This template provides a consistent baseline for AI-assisted software development.

Instead of configuring GitHub Copilot separately for every new repository, projects created from this template inherit:

- Coding standards
- Security expectations
- Testing rules
- Debugging methodology
- Architecture preferences
- Database practices
- Specialized development agents
- Reusable development skills

Project-specific instructions can then be added on top of this baseline.

---

## How to Use

### Create a project from GitHub

1. Open this repository on GitHub
2. Click **Use this template**
3. Select **Create a new repository**
4. Enter the project name
5. Create the repository
6. Clone the new repository locally

The new repository will contain the complete Copilot configuration automatically.

### Create a project with GitHub CLI

```bash
gh repo create my-new-project \
  --template YOUR_USERNAME/copilot-project-template \
  --private \
  --clone
```

Replace `YOUR_USERNAME` with your GitHub username.

---

# Copilot Configuration

## Repository Instructions

File:

```text
.github/copilot-instructions.md
```

Contains general rules that apply across the entire repository.

Examples:

- Architecture preferences
- Security requirements
- Code quality rules
- Testing requirements
- Debugging expectations

These instructions define the default engineering standards for the project.

---

## Path-Specific Instructions

Directory:

```text
.github/instructions/
```

These instructions apply only to matching files.

### Python

```text
python.instructions.md
```

Used for Python files.

Includes guidance for:

- PEP 8
- Type hints
- Error handling
- Logging
- Backend architecture
- Testing

### React / TypeScript

```text
react.instructions.md
```

Used for frontend code.

Includes guidance for:

- React
- TypeScript
- Components
- Hooks
- State management
- Accessibility
- API integration

### Database

```text
database.instructions.md
```

Used for SQL and migration-related files.

Includes guidance for:

- SQL safety
- Indexing
- Constraints
- Transactions
- Migration safety
- Performance

### Testing

```text
tests.instructions.md
```

Used for test files.

Includes guidance for:

- Unit tests
- Integration tests
- Regression testing
- Failure scenarios
- Deterministic tests

---

# Custom Agents

Directory:

```text
.github/agents/
```

Custom agents provide specialized roles for different development tasks.

## Backend Agent

Focuses on:

- Python
- Django
- Flask
- FastAPI
- REST APIs
- Authentication
- Business logic
- Backend architecture

## Frontend Agent

Focuses on:

- React
- TypeScript
- Components
- Hooks
- State management
- API integration
- Accessibility

## Database Agent

Focuses on:

- PostgreSQL
- Schema design
- SQL
- Indexing
- Query optimization
- Transactions
- Migrations

## Debugger Agent

Uses a root-cause-first debugging approach.

Focuses on:

- Reproducing bugs
- Tracing execution
- Identifying root causes
- Regression testing
- Avoiding workaround-based fixes

## Reviewer Agent

Performs production-focused code reviews.

Reviews for:

- Correctness
- Security
- Architecture
- Maintainability
- Performance
- Testing
- Backwards compatibility

## Security Agent

Focuses on application security.

Reviews for issues such as:

- Broken authentication
- Broken authorization
- SQL injection
- XSS
- CSRF
- SSRF
- IDOR
- Path traversal
- Secret exposure
- Unsafe file handling

---

# Skills

Directory:

```text
.github/skills/
```

Skills provide reusable knowledge and workflows that Copilot can apply when relevant.

| Skill               | Purpose                          |
| ------------------- | -------------------------------- |
| Python Backend      | Python backend development       |
| React / TypeScript  | Frontend development             |
| PostgreSQL          | Database design and optimization |
| Code Review         | Structured code review           |
| Testing             | Automated testing guidance       |
| Debugging           | Root-cause debugging             |
| API Designer        | REST API design                  |
| Docker / Deployment | Containers and deployment        |
| Database Migration  | Safe schema and data migrations  |

---

# AGENTS.md

The root file:

```text
AGENTS.md
```

defines general instructions for AI agents working in the repository.

It provides guidance for:

- Inspecting existing code before making changes
- Understanding architecture
- Avoiding unrelated modifications
- Running tests
- Debugging correctly
- Preserving existing functionality

Additional `AGENTS.md` files can be created deeper in the project.

Example:

```text
project/
├── AGENTS.md
├── backend/
│   └── AGENTS.md
└── frontend/
    └── AGENTS.md
```

More specific files can extend or override the root-level agent instructions for that part of the project.

---

# Recommended Project Customization

After creating a new repository from this template, update the Copilot configuration to match the actual project.

Typical additions include:

```text
backend/AGENTS.md
frontend/AGENTS.md
```

Project-specific instructions may include:

- Framework versions
- Folder structure
- Architecture decisions
- Naming conventions
- API patterns
- Database rules
- Deployment environment
- Testing framework
- CI/CD requirements

---

# Recommended Development Principles

Projects based on this template should generally follow these principles:

- Clean architecture
- Separation of concerns
- Secure coding by default
- Explicit validation
- Strong database integrity
- Automated testing
- Root-cause debugging
- Small and focused changes
- Minimal unnecessary dependencies
- Production-oriented implementations
- Maintainability over cleverness

---

# Typical Stack

This template is designed primarily around:

## Backend

- Python
- Django
- Flask
- FastAPI

## Frontend

- React
- TypeScript
- JavaScript
- Vite

## Database

- PostgreSQL

## Infrastructure

- Docker
- Docker Compose
- CI/CD
- GitHub Actions

The template can also be adapted to other languages and frameworks.

---

# Maintaining the Template

When improvements are made to the Copilot setup, update this template repository first.

Examples:

- New agent
- New skill
- Better security rules
- Updated testing instructions
- Improved database practices
- New framework-specific instructions

New projects created afterward will automatically inherit the updated configuration.

Existing projects will not automatically receive template changes and must be updated separately.

---

# Goal

The goal of this repository is simple:

> Start every project with a strong engineering and AI-assisted development baseline instead of rebuilding the Copilot configuration from scratch.
