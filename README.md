# Varro Orchestrator

**Status:** Planned  
**Technologies:** Python · AsyncIO · HTTP APIs · MCP · LLMs

## Overview

Varro Orchestrator is a custom backend service responsible for conversations, agent coordination, memory retrieval, and tool execution in the Varro assistant. I am developing it to separate application logic from user interfaces and model-serving software.

The **Varro** name honors Marcus Terentius Varro, a Roman scholar known for organizing knowledge across diverse subjects.

## Key Design Choices

- **Single coordination layer:** Maintain conversation identity, task state, and tool execution in one service.
- **Priority scheduling:** Keep interactive requests responsive while lower-priority agents work concurrently.
- **Context selection:** Retrieve relevant memory and chat history instead of including all stored information in each request.
- **Tool control:** Use selected MCP tools with application-side routing and authorization checks; route simple deterministic commands without an LLM where practical.
- **Backend independence:** Call local or external language models through a configurable HTTP interface.

## Roadmap

- [ ] Define request, session, and tool interfaces.
- [ ] Implement the conversation and model-request loop.
- [ ] Add persistent memory and context retrieval.
- [ ] Implement MCP execution, delegated agents, and request priorities.
- [ ] Validate concurrent tasks and client integration.

## Usage

### Requirements

### Setup

### Configuration

### Operation
