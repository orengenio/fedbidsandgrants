# FedBidsAndGrants

This repository contains example n8n workflows for automating government bid tracking and grant proposal generation. These workflows are designed as starting points for integrating large language models and GoHighLevel CRM to streamline your pipeline.

## Overview

The included workflows demonstrate how to:

1. Fetch opportunities from a data source.
2. Analyze and summarize them with AI services.
3. Generate proposal drafts using multiple LLM providers (OpenAI, Claude, etc.).
4. Add leads and send messages through GoHighLevel.

Each workflow uses placeholder URLs and API parameters. Replace them with your specific endpoints and authentication details before deploying.

## Workflows

- **`workflows/main_workflow.json`** – orchestrates the daily process of retrieving opportunities, summarizing them with OpenAI, and updating the CRM.
- **`workflows/proposal_generator.json`** – takes opportunity data and produces a refined proposal using both Claude and OpenAI models.
- **`workflows/relationship_manager.json`** – simple example for adding contacts to GoHighLevel and sending a welcome message.

Import these JSON files into your n8n instance to explore and modify the flows. They are intentionally minimal and may require additional nodes (e.g., authentication, error handling, routing) depending on your needs.

## Customization

1. **Set up credentials** for each API (OpenAI, Claude, GoHighLevel, etc.) in your n8n installation.
2. **Replace URLs and parameters** in the HTTP Request nodes with your actual endpoints.
3. **Extend the flows** with conditional logic, additional LLM calls, or database steps to fit your full pipeline.
4. **Schedule** the main workflow according to how often you want to scan for new opportunities.

These examples should help you build a more robust system for bidding and grant proposals. Modify and expand them to create a production‑ready automation pipeline.
