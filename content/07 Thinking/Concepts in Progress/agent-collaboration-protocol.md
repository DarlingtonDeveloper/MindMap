---
title: "Agent Collaboration Protocol"
date: 2025-04-23
tags: [agents, protocol, collaboration, coordination, yc-idea]
---

## Overview

The **Agent Collaboration Protocol (ACP)** is a shared language and interaction model that enables multiple AI agents to coordinate, co-own tasks, resolve conflicts, and make joint decisions across long-running workflows.

## Problem

Current AI agents operate in silos. Multi-agent coordination is brittle, ad hoc, or entirely absent. Humans rely on messaging platforms, task boards, and standups — agents need a protocol that mirrors this:

- Shared task ownership
- Role-based contributions
- Status broadcasting
- Conflict resolution primitives

## Solution

ACP introduces a set of primitives:

- `join(task_id, role)`: declare interest and join a task with a purpose
- `propose(action)`: suggest an action or next step
- `vote(action_id)`: cast a weighted vote for a proposed action
- `status_update(task_id)`: share progress, blockers, or intents
- `resolve(conflict_id)`: engage arbitration or fallback strategies

## Format

Based on JSON-LD with semantic tagging for:

- Agent ID and capabilities
- Task graph modeling
- Communication history for auditing and reasoning

## Applications

- Complex software builds with multiple agents handling design, code, tests
- Cross-company B2B agent orchestration
- Decentralized workflows in DAOs or Web3 infra

## Roadmap

- v1: SDK in Python + TypeScript
- v2: Real-time collaboration channel (WebSocket-based)
- v3: Plug-in layer for popular agent frameworks (AutoGen, LangGraph, CrewAI)
