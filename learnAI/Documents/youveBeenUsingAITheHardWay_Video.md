# Summary of "You've Been Using AI the Hard Way (Use This Instead)"

**Video URL:** https://www.youtube.com/watch?v=MsQACpcuTkU

# Detailed Summary of "You've Been Using AI the Hard Way (Use This Instead)"

This document provides a detailed, section-by-section summary of the YouTube video by NetworkChuck, which advocates for using AI in the terminal for a more efficient and powerful workflow.

## 1. Introduction: The Problem with Browser-Based AI

*   **Inefficiency:** The video starts by highlighting the inefficiencies of using AI in a web browser, such as losing context across multiple chats, the need to copy and paste information, and the lack of control over the project's data.
*   **The Terminal as a Solution:** The speaker proposes that using AI in the terminal is a "superpower" that allows for greater speed, control, and functionality.

## 2. Gemini CLI: Your First Step into Terminal AI

*   **Installation:** The video provides a simple one-command installation for the Gemini CLI, with instructions for Mac, Windows (with WSL), and Linux.
*   **First Steps:** The user is guided through logging into their Google account and asking their first question.
*   **Superpowers:** The Gemini CLI offers several advantages over the browser version:
    *   It shows the context window size.
    *   It can read and write files directly to your computer.
    *   It can execute bash and Python scripts.
*   **Project Context with `gemini.md`:** A key feature highlighted is the ability to create a `gemini.md` file. This file provides context to the AI about the project, so you don't have to re-explain everything in a new session.

## 3. Claude Code: The Daily Driver

*   **Installation:** Similar to Gemini, Claude Code (Claude in the terminal) is installed with a single command.
*   **Context File:** Claude Code also uses a context file, `claude.md`, which works similarly to Gemini's context file.
*   **Agents: The Game-Changing Feature:** The video introduces "agents" in Claude Code, which are like sub-AIs that can be delegated tasks. This has several benefits:
    *   **Preserves Context:** Delegating tasks to agents doesn't bloat the main conversation's context window.
    *   **Fresh Perspective:** Each agent starts with a fresh context, avoiding biases from the main conversation.
    *   **Parallel Processing:** Multiple agents can work on different tasks simultaneously.
*   **Customization:** The video demonstrates how to create custom agents for specific tasks, such as a "brutal critic" agent to review work.

## 4. The Multi-AI Workflow

*   **Using Multiple Tools:** The speaker reveals that he uses Gemini, Claude Code, and Codex (ChatGPT's terminal tool) all at the same time on the same project.
*   **Synced Context:** The key to this workflow is to have all the AI tools working in the same directory and to keep their context files (`gemini.md`, `claude.md`, and `agents.md` for Codex) synchronized.
*   **Division of Labor:** The speaker assigns different roles to each AI:
    *   **Gemini and Claude:** For deep work and content generation.
    *   **Codex (ChatGPT):** For high-level analysis and review.

## 5. Open Code: The Open-Source Alternative

*   **Installation:** Open Code is an open-source tool that can be installed with a single command.
*   **Flexibility:** It allows you to use various models, including:
    *   Grok (free for a limited time).
    *   Local models (e.g., Llama 3.2).
    *   Claude (by logging in with your Claude Pro subscription).
*   **Features:** Open Code also supports sessions, sharing sessions via URL, and a timeline feature to go back in time.

## 6. The Philosophy: Owning Your Context

*   **Data Ownership:** The main takeaway from the video is that by using AI in the terminal, you own your data and your context. Your project is not locked into a specific vendor's platform.
*   **Future-Proof:** If a new, better AI comes out, you can easily switch to it because all your project files are on your local machine.
*   **Personalization:** The speaker encourages viewers to build their own personalized AI-powered workflows tailored to their specific needs.

## 7. Practical Workflow and Automation

*   **Syncing Context Files:** The speaker uses an agent in Claude to automatically summarize the work done and update the context files for all the AI tools.
*   **Version Control with Git:** He treats his projects like code, using Git to commit changes and keep a history of his work. This allows him to track progress and revert to previous versions if needed.
*   **Critique and Improvement:** The speaker emphasizes the importance of using AI to critique his own work, using custom agents to provide harsh but valuable feedback.
