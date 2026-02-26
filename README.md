Custom Question Answering Bot using Azure Language Service
Overview

This project demonstrates how to build and deploy a custom Question Answering knowledge base using Microsoft Azure Language Service, and integrate it with an Azure Web App Bot for automated customer support.

The system allows users to ask natural language questions and receive intelligent answers sourced from a structured FAQ document.

Problem Statement

Customer support systems often struggle with repetitive FAQs, leading to increased operational costs and delayed responses.

This project solves that by:

Creating a searchable knowledge base from structured documents

Enabling natural language query interpretation

Deploying a chatbot that provides automated responses via web interface

Architecture

User → Web App Bot → Azure Language Service → Knowledge Base → Response

Core components:

Azure Language Service (Custom Question Answering)

Azure Cognitive Search

Azure Web App Bot

FAQ document as structured data source

Features

Knowledge base creation from external document (FAQ)

Custom question–answer pair addition

Alternate phrase recognition (e.g., “Hi” → “Hello”)

Intelligent short answer extraction

Full answer passage retrieval

HTTP deployment for external access

Bot integration for real-time interaction

Tech Stack

Microsoft Azure Language Service

Azure Cognitive Search

Azure Bot Service

Web App Bot (C# or Node.js SDK)

Natural Language Processing (NLP)

Knowledge Base Configuration

Project Name: MargiesTravel
Source Language: English
Default Fallback Response: "No answer found"

Data Source:
FAQ document imported from GitHub (Microsoft Learning AI-900 dataset)

Custom Additions:

Question: Hello

Alternate phrase: Hi

Answer: Hello

Testing

Example Queries:

User Input	Expected Behavior
Hi	Returns "Hello"
I want to book a flight	Returns relevant FAQ answer
How can I cancel a reservation?	Returns cancellation policy
Random unrelated query	Returns fallback response

The system supports:

Extracted short answers

Full contextual answer passages

Deployment

The knowledge base is deployed via Azure Language Studio.

A Web App Bot is configured with:

Language resource key

Project name

Endpoint hostname

Managed identity authentication

The bot is tested using the Azure Web Chat interface.

Limitations

Performance depends on quality of training data

Limited contextual memory (not a conversational LLM)

Requires manual updates for new FAQs

Future Improvements

Integrate with a live website

Expand FAQ dataset

Add multilingual support

Add telemetry and analytics tracking

Improve intent handling with Azure Conversational Language Understanding

Learning Outcomes

Through this project, I gained hands-on experience with:

Azure resource provisioning

Knowledge base design

NLP-powered search systems

Bot deployment and configuration

Cloud-based AI integration
