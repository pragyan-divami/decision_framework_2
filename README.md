# Port Talbot Decision Framework

The Port Talbot Decision Framework is an interactive, browser-based Multi-Criteria Decision Analysis (MCDA) application designed to simulate executive decision-making under various scenarios and emotional states.

## Overview

This tool models how different executive personas evaluate complex scenarios by applying different cognitive weights to key business dimensions (Schedule, Financial, Political, Commercial). It also demonstrates how emotional states (cautious, strategic, analytical, decisive) dynamically modify these weightings and influence the final recommended actions.

The application runs entirely in the browser using pure JavaScript and requires zero API calls for its core matrix functionality. It also features an optional AI Assistant powered by Groq.

## Key Features

- **Executive Personas**: Simulate decisions from the perspectives of key stakeholders including the CEO, Project Director, CFO, CHRO, and Commercial Director.
- **Dynamic Emotion Modifiers**: See how decisions shift when a persona adopts a *Cautious*, *Strategic*, *Analytical*, or *Decisive* emotional state.
- **Scenario Analysis**: Built-in scenarios such as contract disputes (VO-112), infrastructure delays, commercial commitments, financial renegotiations, and staffing crises.
- **Constraint Layer**: Hard constraints that eliminate specific options based on real-time Key Performance Indicators (KPIs).
- **Conflict Matrix**: A cross-persona view that highlights where leaders agree or conflict, and why.
- **AI Assistant**: Optional Groq-powered chat assistant to query decisions, perspectives, and risks (requires a free Groq API key).

## How to Run

A lightweight Python launcher is included to run the application locally and bypass any CORS issues when using the AI Assistant.

1. Ensure you have Python installed.
2. Run the launcher from your terminal:
   ```bash
   python3 launch.py
   ```
3. Your default web browser will automatically open the application.

## Project Structure

- `port_talbot_decision_framework.html`: The core application containing all UI components, styles, and the pure JavaScript MCDA engine.
- `launch.py`: A simple HTTP server script to serve the HTML file and configure CORS headers for the optional AI integration.