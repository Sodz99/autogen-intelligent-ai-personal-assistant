# Autogen Project to Build an Intelligent AI Personal Assistant

The primary aim of this project is to utilize AutoGen to build a Multi-Agent System for orchestrating specialized AI agents into a unified personal assistant system, enabling seamless task automation, service integration, and intelligent conversation handling.

## Overview
Modern digital life is filled with dozens of tools emails, calendars, weather apps, web browsers all designed to help us manage our day. Yet ironically, the constant switching between these tools often leads to fragmented workflows, wasted time, and decreased focus. The problem isn’t the tools themselves, but the lack of a unified system that can intelligently coordinate and automate tasks across them.

This project tackles that challenge by creating a centralized, intelligent automation layer that can manage daily workflows more efficiently. At its core is a multi-agent system that brings together diverse services like Gmail operations, Google Calendar scheduling, weather forecasting, and real-time web search into one cohesive interface. The goal is to replace manual effort and context-switching with smart, conversational automation.

## Approach
- Set Up the Environment ○ Install AutoGen AgentChat and required dependencies ○ Configure OpenAI API keys and environment variables ○ Set up project structure and virtual environment
- Tool Building and Service Integrations ○ Obtain Google API credentials and configure OAuth2 authentication flows ○ Set up Gmail API integration with LangChain toolkit for email operations ○ Configure Google Calendar API for scheduling and event management ○ Integrate Tavily Search API for web search and research capabilities ○ Implement Weather API connections for meteorological data ○ Create tool implementations with async capabilities for each service
- Agent Architecture Design

○ Create specialized agents for Email, Calendar, Weather, and Search functionalities ○ Design system prompts for optimal agent behavior and tool selection ○ Implement FunctionTool wrappers for seamless AutoGen integration ○ Configure agent descriptions and capabilities for intelligent task routing

- Multi-Agent Orchestration ○ Configure MagenticOneGroupChat for intelligent agent coordination ○ Implement termination conditions and conversation flow management ○ Set up logging and monitoring for agent interactions and performance ○ Create the main orchestrator class for managing the agent lifecycle
- Build Conversational Interface System ○ Implement context-aware conversation handling with agent selection logic ○ Design response formatting for optimal user experience across platforms ○ Configure final answer prompts for consistent response structure
- Platform Integration and Deployment ○ Create Slack app configuration with proper scopes and permissions ○ Implement FastAPI-based server with Slack SDK integration ○ Set up webhook endpoints for event handling ○ Configure threading and background task processing for responsive interactions

Modular code overview:

Once you unzip the code.zip file, you can find the following:

## Tech stack
➔ Language: Python 3.12 ➔ Libraries: autogen-agentchat, autogen-core, autogen-ext, fastapi, uvicorn, slack-sdk, httpx, pandas, pytz, Open AI ➔ Model: OpenAI GPT-4o ➔ APIs: Google Gmail API, Google Calendar API, OpenWeatherMap, Tavily Search API ➔ Platform Integrations: Slack SDK, FastAPI REST endpoints

## How to run
```bash
pip install -r code (1)/requirements.txt
```

## Project structure
```
.gitignore
README.md
code (1)/
  readme.md
  requirements.txt
  slack_app.py
  source/
    __init__.py
    calendar_tools.py
    configurations.py
    email_tools.py
    google_utils.py
    log_records.py
    personal_agents.py
    prompts.py
    search_tools.py
    weather_tools.py
```

## Credits
Based on a ProjectPro guided project.
