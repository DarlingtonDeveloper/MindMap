---
title: "Prompt Registry with Feedback Hooks"
date: 2025-04-23
tags: [prompts, agents, devtools, feedback, yc-idea]
---

## Overview

The **Prompt Registry with Feedback Hooks** is version control for prompts. It enables teams and agents to store, share, and monitor prompt performance with metadata, user ratings, and real-world feedback loops. Think of it as GitHub for prompt engineering.

## Problem

Prompts are often:

- Stored in random files or environment variables
- Changed without tracking impact
- Hard to A/B test
- Lacking context around why they were written or updated

## Solution

Features:

- Prompt versioning with changelogs and commit messages
- Feedback hooks: capture success/failure signals from end-users or agents
- Tags and metadata for prompt discovery
- Performance dashboards (avg. tokens, response time, task completion)
- CI hooks for validating against test examples

## Technical Stack

- Supabase/Postgres for storage and analytics
- Web UI for prompt editing and reviews
- CLI + SDKs for agent/LLM integrations

## Use Cases

- Teams building multi-agent systems
- Enterprises managing LLM apps
- Open-source contributors sharing effective prompts

## Future Ideas

- Prompt marketplace
- Reputation scores for contributors
- Integration with Langchain/AutoGen agents directly
