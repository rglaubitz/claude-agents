# Claude Agents Library

A versioned collection of 42 specialist agents for Claude Code projects.

> **The Workforce Library** - Import only the agents you need for your project.
>
> **Looking for the workflow system?** See [claude-workflow-starter](https://github.com/rglaubitz/claude-workflow-starter)
>
> **Architecture details:** See [ARCHITECTURE.md](./ARCHITECTURE.md)

## Agent Summary

| Category | Count | Purpose |
|----------|-------|---------|
| **Orchestration** | 4 | Planning & coordination |
| **Development** | 6 | Core implementation |
| **Quality** | 4 | Testing & compliance |
| **Research** | 17 | Research & documentation ⭐ |
| **Review** | 4 | Code review & validation |
| **Support** | 7 | Specialized tools |
| **Total** | **42** | Complete workforce library |

## How This Works

This library provides specialist agents that you "hire" during **Phase 3: Execution Planning** of the [claude-workflow-starter](https://github.com/rglaubitz/claude-workflow-starter) workflow.

**You don't need all 42 agents** - only import the ones your project needs.

**Example:** A web app might only need:
- task-manager, project-task-planner (orchestration)
- backend-developer, frontend-developer, database-architect (development)
- qa-engineer, code-review-expert (quality)

## Installation

### Option 1: Install All Agents
```bash
git clone https://github.com/yourusername/claude-agents ~/.claude/agents
```

### Option 2: Install Specific Category
```bash
# Install only orchestration agents
cp claude-agents/orchestration/* ~/.claude/agents/
```

### Option 3: Install Individual Agent
```bash
# Download single agent
curl -o ~/.claude/agents/task-manager.md \
  https://raw.githubusercontent.com/yourusername/claude-agents/main/orchestration/task-manager.md
```

## Agent Categories

### Orchestration (4 agents)
Strategic planning and coordination
- **task-manager** - Director of execution, workflow orchestration
- **project-task-planner** - Task breakdown, dependency mapping
- **prd-expert** - PRD creation, requirements specification
- **agent-architecture-designer** - Multi-agent system design

### Development (6 agents)
Core implementation specialists
- **database-architect** - Schema design, database optimization
- **graph-database-specialist** - Neo4j, Cypher, GraphRAG systems
- **ai-ml-engineer** - RAG pipelines, embeddings, vector databases
- **frontend-developer** - React, Next.js, modern web apps
- **backend-developer** - APIs, services, business logic
- **devops-engineer** - CI/CD, deployment, infrastructure

### Quality (4 agents)
Quality assurance and compliance
- **security-auditor** - Vulnerability scanning, penetration testing
- **performance-engineer** - Optimization, load testing, profiling
- **accessibility-specialist** - WCAG compliance, a11y testing
- **qa-engineer** - Test strategy, quality gates orchestration

### Review (4 agents)
Code review and validation
- **code-review-expert** - Parallel code review, deep analysis
- **database-reviewer** - Database design validation
- **frontend-reviewer** - Frontend code quality validation
- **backend-reviewer** - Backend code quality validation

### Support (7 agents)
Specialized technical support
- **api-architect** - REST/GraphQL design, API contracts
- **ui-ux-designer** - Design systems, user experience
- **data-pipeline-engineer** - ETL, data processing pipelines
- **knowledge-graph-engineer** - GraphRAG ontologies, entity extraction
- **sql-specialist** - Query optimization, indexing strategies
- **integration-specialist** - API/service integration
- **mcp-bridge-engineer** - MCP server integration

### Research (17 agents) ⭐ EXPANDED
Research, documentation, and knowledge gathering

**Core Research Team (4 agents):**
- **research-manager** - Research orchestration, quality validation
- **documentation-expert** - Technical writing, documentation structure
- **agent-testing-engineer** - Agent behavior validation
- **memory-system-engineer** - Knowledge persistence, data storage

**Research Specialists (13 agents):**
- **deep-researcher** - In-depth technical investigation
- **research-coordinator** - Multi-source research coordination
- **technical-validator** - Validates technical accuracy
- **standards-researcher** - Framework standards, best practices
- **company-researcher** - Organization and product research
- **competitive-intelligence-analyst** - Market and competitor analysis
- **technical-trend-analyst** - Technology trend forecasting
- **documentation-hunter** - Finds official docs and guides
- **github-examples-hunter** - Discovers quality code examples
- **pattern-implementation-analyst** - Analyzes implementation patterns
- **api-documentation-specialist** - API reference expertise
- **citation-manager** - Source validation and citation
- **code-quality-validator** - Validates code quality standards

## Version Compatibility

| Agent Library | Claude Code | Notes |
|--------------|-------------|-------|
| v1.0.0 | ≥1.0.0 | Initial release |
| v1.1.0 | ≥1.2.0 | Added parallel support |
| v2.0.0 | ≥2.0.0 | Constitution compliance |

## Agent Format

All agents follow Claude Code standards:
```yaml
---
name: agent-name
description: "When this agent should be invoked"
tools: Tool1, Tool2, Tool3
model: sonnet|opus|haiku (optional)
---

[Agent prompt and instructions]
```

## Contributing

1. Follow the agent formatting guide
2. Test with constitution compliance
3. Submit PR with description
4. Bump version appropriately

## License

MIT
