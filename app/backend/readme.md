# Backend Application

This directory contains the backend application for the Azure Search OpenAI Demo.

## Overview

The backend is built using [Quart](https://quart.palletsprojects.com/), a Python framework for asynchronous web applications. It communicates with the frontend using the [AI Chat App HTTP Protocol](https://github.com/Azure-Samples/ai-chat-app-protocol).

## Directory Structure

- `approaches/`: Contains the classes powering the Chat and Ask tabs. Each class uses a different RAG (Retrieval Augmented Generation) approach.
- `auth/`: Contains the authentication logic for the application.
- `common/`: Contains common utilities and helper functions used across the application.
- `models/`: Contains the data models used in the application.
- `routes/`: Contains the route handlers for the application's API endpoints.

## Setup

To set up the backend for local development, follow these steps:

1. Install the required Python packages: `pip install -r requirements.txt`
2. Set the necessary environment variables.
3. Run the application: `python main.py`

## Customization

You can customize the backend to suit your needs. Typically, the primary backend code you'll want to customize is in the `approaches` folder. For more details, refer to the [customization guide](../docs/customization.md).

## Testing

To run the unit tests, use the following command: `pytest`

## Contributing

We welcome contributions! Please see [CONTRIBUTING.md](../CONTRIBUTING.md) for details on how to contribute.