---
title: "Agent Technical Writer"
date: 2025-04-23
tags: [agents, documentation, devtools, productivity, yc-idea]
---

## Overview

The **Agent Technical Writer** is an LLM-powered documentation assistant that observes your development activity and autogenerates internal docs, onboarding guides, and changelogs in clean, readable Markdown. It sits alongside your codebase and dev tools, integrating seamlessly.

## Problem

Developers often skip writing docs. Teams rely on tribal knowledge. Docs are outdated or nonexistent. New hires struggle. Changelogs are spotty or copy-pasted from commit messages.

## Solution

The agent:

- Hooks into Git + PRs
- Watches your coding sessions or reviews
- Extracts intentions, APIs, and usage
- Generates:
  - README updates
  - Endpoint documentation
  - Component usage notes
  - Onboarding instructions
  - Changelogs with diff summaries

## Features

- Markdown or Notion export
- Editor preview + “accept edits” flow
- Supports frameworks: React, Next.js, Node.js, Django
- Optional voice notes to enrich context

## Audience

- Startups with fast-moving teams
- OSS maintainers
- Freelancers + consultants with handoff duties

## Extensions

- Multilingual doc generation
- Visual walkthroughs (Loom-style)
- Docs-as-code integrations (Docusaurus, Nextra)
