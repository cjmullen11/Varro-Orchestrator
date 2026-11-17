# Varro Orchestrator

**Status:** Planned  
**Technologies:** Python · AsyncIO · HTTP APIs · MCP · LLMs

## Overview

Varro Orchestrator is a custom service that manages conversations, agent tasks, memory, and tool calls for the Varro AI assistant. I am developing it to keep application logic independent of the model-serving backend and individual client interfaces.

The **Varro** name references Marcus Terentius Varro, a Roman scholar associated with broad, organized knowledge.

## Key Design Choices

- **Central control plane:** Own chat state, task delegation, and tool execution rather than relying on client-side logic.
- **Prioritized concurrency:** Schedule interactive requests ahead of lower-priority background agents.
- **Selective context:** Retrieve relevant memory and conversation history instead of sending all stored data to each model request.
- **Controlled tools:** Expose selected MCP capabilities with application-side permission and execution checks.
- **Backend independence:** Use a configurable HTTP inference endpoint for local or external models.

## Roadmap

- [ ] Define the request, session, and tool-execution interfaces.
- [ ] Implement the conversation and model-request loop.
- [ ] Add persistent memory and relevant-context retrieval.
- [ ] Implement MCP calls, delegated tasks, and priority scheduling.
- [ ] Test concurrent workflows and client integration.

## Usage

### Requirements

### Setup

### Configuration

### Operation
