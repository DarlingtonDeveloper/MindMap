---
title: "Frontend SDK for Embedding Agents in Web Apps"
date: 2025-04-23
tags: [agents, frontend, sdk, webapps, ux, devtools, yc-idea]
---

## Overview

A **Frontend SDK** that enables developers to easily embed AI agents into web applications with first-class UX support. This toolkit provides plug-and-play components for chat, streaming actions, memory context, and tool invocation — ideal for SaaS, dashboards, and productivity tools.

## Problem

Embedding agents in apps today is custom work: WebSockets, token streaming, prompt history, memory management — all handcrafted per use case. Developers need a standard toolkit to:

- Render chat UIs with token-by-token streaming
- Manage memory/session/state via local-first storage
- Call tools/functions safely from UI with feedback

## Solution

The SDK includes:

- `<AgentChat />`: Embeddable, themeable chat UI
- `<MemoryStore />`: Manages session memory + user feedback
- `<ToolCall />`: Wraps function calling UX with input forms
- `<AgentConfigPanel />`: Live parameter tuning for devs or end-users

## Architecture

- Written in TypeScript + React
- Built-in support for OpenAI functions, Langchain tools, Supabase memory
- LocalStorage + Supabase dual persistence for agent memory

## Use Cases

- Custom CRMs with embedded AI assistants
- Knowledge bases and helpdesks with streaming GPT support
- Personal dashboards (health, finances, habits) with interactive agents

## Future

- Vue + Svelte versions
- PWA compatibility + offline fallback
- Plugins for voice input, camera input, and screen recording
