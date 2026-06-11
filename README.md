# Sacral Business OS

An AI-native workspace that combines personalized memory, knowledge retrieval, and contextual guidance to help entrepreneurs implement ideas and make decisions over time.

Built as an exploration of long-term personalization, AI orchestration, and implementation-focused user experiences.

## Overview

I built Sacral Business OS to explore how AI can move beyond simple chat interactions and become a personalized workspace that helps users make decisions, organize information, and implement ideas. The platform combines persistent user memory, retrieval-augmented knowledge systems, and AI-powered guidance to deliver contextual recommendations based on each user's Human Design chart, goals, experiences, and evolving needs.

## System Architecture

The platform combines persistent user context, retrieval-based knowledge systems, and AI-powered guidance to help users make decisions, prioritize actions, and implement ideas over time.

```mermaid
flowchart TD

    U[User]

    UC[User Context<br/>Human Design • Memory • Goals • Insights]

    KB[Knowledge Base<br/>Human Design • Business Methodologies]

    U --> UC
    U --> KB

    UC --> CE[Context Engine]
    KB --> CE

    CE --> AM[AuraMate Assistant]

    AM --> PG[Personalized Guidance]

    PG --> D[Decisions]
    PG --> P[Priorities]
    PG --> E[Execution]
```
## Product Screenshots

### Main chat interface
<img src="https://drive.google.com/uc?export=view&id=1IaUkXx7ZJmh90ov7hLL3TnOyuKrU1TUS" width="900" alt="Sacral Business OS architecture diagram" />

### Energy data gathering feature

<img src="https://drive.google.com/uc?export=view&id=17qBzwKSspxVPwzSFeZ0PHzisfIB-PH2p" width="900" alt="Sacral Business OS main workspace" />

### Module to kick-start conversation
<img src="https://drive.google.com/uc?export=view&id=1W-Njap2zPsLEPw8NtgoAGKFrUneJ8_2t" width="900" alt="AuraMate chat interface" />

### Work insights based on energy data + Early time tracking API integration
<img src="https://drive.google.com/uc?export=view&id=1SdL5n1ZB4cHfbCm7osM_e0kSgpX5bI2D" width="900" alt="Personalized memory interface" />

### Human Design chart information modal
<img src="https://drive.google.com/uc?export=view&id=1FeSk0cqY0YagbQYQ4brAy0kaFwiWTKkv" width="900" alt="Human Design chart view" />

### Human design chart API integration
<img src="https://drive.google.com/uc?export=view&id=15tmz2sTmR_P0wlZ6rgNpvDnvNXI6SXP-" width="900" alt="Knowledge base and retrieval system" />

### User Memory/data modal
<img src="https://drive.google.com/uc?export=view&id=1SQsGaDEoR2re0dONIh3I0itbYAC-l2l5" width="900" alt="Saved insights interface" />

## What I built

I designed and built the platform end-to-end, including:

- Product strategy
- UX and workflow design
- Prompt architecture
- AI orchestration
- Knowledge retrieval systems
- Memory systems
- Frontend implementation
- Database design
- User onboarding

## What Makes This Different

Most AI applications treat each conversation as a new interaction, or only answer questions.

Sacral Business OS was designed around the idea that meaningful guidance requires long-term context.

The platform combines:

- Persistent user memory
- Human Design profile data
- Retrieval-based knowledge systems
- Conversation history
- User goals and preferences

to generate recommendations that become more personalized over time.

The goal was to create something that does more than answer questions by creating an implementation system that helps users apply Human Design and business methodologies in their everyday work.

The platform continuously incorporates new information as users interact with it. Users can connect time-tracking tools, log how energizing or draining different activities feel, save insights, and build a growing body of context that informs future guidance.

Rather than delivering generic advice, the system is designed to help users make decisions, prioritize work, identify patterns, and take action based on their unique goals, experiences, and Human Design chart.

## Technology Stack

- Next.js
- TypeScript
- Supabase
- Clerk
- OpenAI
- Gemini
- Vercel

## Case Study

https://www.sacralos.ai/case-study

## Personalized Memory

The platform maintains a structured user profile that combines Human Design data, onboarding responses, user-provided context, preferences, goals, and insights generated through prior interactions. Rather than treating each conversation as a blank slate, the system selectively retrieves relevant information to create continuity across sessions and enable increasingly personalized guidance over time.

## Knowledge Retrieval

Sacral Business OS uses a retrieval-based knowledge system containing Human Design education, business frameworks, implementation guidance, deconditioning concepts, and proprietary methodologies. Relevant content is dynamically selected based on the user's question, profile, and current context, allowing responses to be grounded in a curated knowledge base rather than relying solely on model training data.

## Context Assembly

Before generating a response, the system assembles multiple sources of context into a single prompt. This may include user memory, Human Design chart information, retrieved knowledge documents, tool-specific instructions, conversation history, and current user goals. This orchestration layer allows the AI to deliver recommendations that are both personalized and contextually relevant while minimizing unnecessary token usage.

## AI Response Generation

The assembled context is provided to the language model along with tool-specific behavioral instructions. Different AI tools within the platform can use different prompts, knowledge sources, and workflows while sharing the same personalization layer. Responses are generated in real time and designed to support decision-making, implementation, reflection, and ongoing behavior change rather than providing generic advice.

## Lessons Learned

### What Worked

- Persistent memory significantly improved perceived personalization and reduced repetitive onboarding conversations.
- Grounding responses in curated knowledge produced more consistent outputs than relying solely on model reasoning.
- Users responded positively when AI guidance felt contextual and implementation-focused rather than purely informational.
- Human Design provided a useful personalization framework that allowed guidance to feel highly individualized while remaining structured.

### What Didn't

- Early versions relied too heavily on large prompts, resulting in increased token usage and slower response times.
- Generic memory retrieval occasionally surfaced information that was technically relevant but not useful to the current conversation.
- Large knowledge bases require thoughtful organization and retrieval strategies to avoid overwhelming the model with unnecessary context.
- Prompt-only approaches became difficult to maintain as the product expanded into multiple tools and workflows.

### How I Measure Adoption

- User engagement with individual tools and workflows.
- Repeat usage across multiple sessions.
- Growth in saved memories, insights, and user-generated context.
- Qualitative feedback regarding relevance, usefulness, and personalization.
- Ongoing observation of which features users returned to most frequently.

### Tradeoffs I Made

- Chose retrieval-based knowledge over loading entire knowledge bases into prompts to reduce token consumption and improve scalability.
- Prioritized personalization and contextual relevance over complete transparency of internal AI workflows.
- Accepted increased system complexity in exchange for more adaptive and user-specific guidance.
- Focused on implementation support and decision-making rather than building a general-purpose AI assistant.
- Prioritized response quality over feature expansion. I focused on making the AI feel genuinely personalized and context-aware (uncanny!) before investing in additional workspace features, believing that trust and relevance were more important to adoption than feature count.

- ## Technical Stack

- Next.js
- TypeScript
- Tailwind CSS
- Supabase
- Clerk
- OpenAI
- Gemini
- Vercel

## Note

This repository serves as a project case study and architecture overview. The production application is under active development.

