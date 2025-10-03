# Claude Agents Library

A versioned collection of 29 specialized agents for Claude Code projects.

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

### Research (4 agents)
Documentation and analysis
- **research-manager** - Technical research, documentation gathering
- **documentation-expert** - Technical writing, documentation structure
- **agent-testing-engineer** - Agent behavior validation
- **memory-system-engineer** - Knowledge persistence, data storage

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
