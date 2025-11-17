# AI Chat Agent – Cogitator

<a href="https://cogitator.karthikeyansura.workers.dev">
  <img src="https://deploy.workers.cloudflare.com/button" alt="Live Deployment"/>
</a>

A full-stack AI chat agent built on the Cloudflare Agents platform. This project extends the official `cloudflare/agents-starter` template and is configured to run on **Cloudflare Workers AI (Llama 3)**.

## Overview

Cogitator provides a lightweight, fully serverless chat system with tool execution, persistent state, and real-time streaming. It integrates Cloudflare’s Agent runtime, Durable Objects, and Workers AI to deliver a self-contained AI assistant that runs entirely on Cloudflare’s edge.

## Technology Stack

- **LLM**: Llama 3 via Cloudflare Workers AI
- **Agent Runtime**: Cloudflare Agents (backed by Durable Objects)
- **Frontend**: React, served as static assets
- **State & Memory**: SQLite-backed storage (configured via `wrangler.jsonc` migrations)

## Features

- Interactive chat interface
- Tooling with human-in-the-loop confirmation
- One-time, delayed, and cron-based task scheduling
- Real-time streaming responses
- Persistent chat history and agent state

## Live Demo

The deployed application is available at:  
https://cogitator.karthikeyansura.workers.dev

## Running Locally

1. Clone the repository:
   ```bash
   git clone https://github.com/karthikeyansura/cf_ai_cogitator.git
   cd cf_ai_cogitator
