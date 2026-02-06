# Git Commit Summarizer Skill

This is a specialized skill for the **Gemini CLI** designed to act as an expert **Technical Resume Writer** and **Senior Software Architect**.

## Purpose

The primary goal of this skill is to analyze raw git commit logs and transform them into high-impact, resume-worthy achievement statements. It helps developers translate their daily coding activities into professional narratives suitable for CVs and resumes.

## Features

*   **Author Discovery:** Automatically identifies contributors in the repository to help you filter by your specific handle.
*   **Smart Extraction:** Filters out merge commits and trivial style changes to focus on meaningful work.
*   **Resume Synthesis:**
    *   **Action-Oriented:** Starts bullet points with strong power verbs (e.g., *Architected*, *Deployed*, *Optimized*).
    *   **Problem-Solution-Impact:** Structures points to highlight the technical challenge, the solution implemented, and the resulting benefit.
    *   **Aggregation:** Combines multiple granular commits into substantial, cohesive narratives.
    *   **Technical Specificity:** explicitly mentions relevant languages, frameworks, and tools.

## Example

**Input (Raw Commits):**
> `refactor: update database schema for users`
> `feat: add index to user email`
> `perf: optimize user search query`

**Output (Generated Resume Bullet):**
> "Redesigned the user database schema and optimized search queries via indexing, resulting in a 40% reduction in query execution time."

## File Structure

*   `git-commit-summarizer.skill`: The packaged skill file for use with Gemini CLI.
*   `AGENT.md`: The system prompt defining the agent's persona and logic.

### Nice to pair.
[https://github.com/marketplace/actions/lazypr-ai-pr-summary](Lazy PR)
lazypr is an AI-powered GitHub Action that rescues your repository from "lazy" documentation and "updated auth" as a PR title. It automatically generates high-context Pull Request summaries, risk assessments, and change logs directly from your code diffs.
