# Awesome Claude Code Workflows with stars

> Curated workflow recipes that combine hooks, MCP servers, skills, agents, and CLAUDE.md to automate real development tasks in Claude Code.

A workflow is more than a single tool — it's a **recipe** that chains multiple Claude Code primitives together. Think of this as a cookbook, not a tool catalog.

Looking for individual components? See [awesome-claude-code](https://github.com/hesreallyhim/awesome-claude-code) ⭐ 53,149 | 🐛 945 | 🌐 Python | 📅 2026-08-29 for tools, [awesome-claude-skills](https://github.com/ComposioHQ/awesome-claude-skills) ⭐ 73,828 | 🐛 1,346 | 🌐 Python | 📅 2026-08-10 for skills, and [awesome-claude-code-hooks](https://github.com/ithiria894/awesome-claude-code-hooks) ⭐ 23 | 🐛 1 | 📅 2026-03-24 for hooks.

## Contents

* [Virtual Engineering Teams](#virtual-engineering-teams)
* [Plan-Build-Review Pipelines](#plan-build-review-pipelines)
* [Multi-Agent Orchestration](#multi-agent-orchestration)
* [Context and Memory Management](#context-and-memory-management)
* [TDD and Code Quality](#tdd-and-code-quality)
* [Git and PR Automation](#git-and-pr-automation)
* [Ship and Deploy](#ship-and-deploy)
* [Cross-LLM Collaboration](#cross-llm-collaboration)
* [Research and Discovery](#research-and-discovery)
* [Browser and Testing](#browser-and-testing)
* [Marketing and Content](#marketing-and-content)
* [Business Operating Systems](#business-operating-systems)
* [Autonomous Loops](#autonomous-loops)
* [Scope and Config Management](#scope-and-config-management)
* [Monitoring and Dashboards](#monitoring-and-dashboards)
* [Comprehensive Frameworks](#comprehensive-frameworks)

***

## Virtual Engineering Teams

Workflow systems that simulate an entire engineering team with specialized agents.

* [Superpowers](https://github.com/obra/superpowers) ⭐ 279,109 | 🐛 332 | 🌐 Shell | 📅 2026-08-29 - Composable plugin with auto-triggering skills for TDD, brainstorming, plan-then-execute, subagent-driven development, parallel agent dispatch, and code review loops. Includes hooks for session-start and verification gates. 20K stars.
* [gstack](https://github.com/garrytan/gstack) ⭐ 130,236 | 🐛 810 | 🌐 TypeScript | 📅 2026-08-28 - Virtual engineering team with 25 skills — CEO review, design review, eng review, QA, ship, canary deploy, freeze/guard safety hooks, and browser-based testing. The gold standard for "skills + hooks + CLAUDE.md as a startup engineering org."
* [OneRedOak/claude-code-workflows](https://github.com/OneRedOak/claude-code-workflows) ⭐ 3,888 | 🐛 9 | 📅 2025-09-14 - Battle-tested workflows from an AI-native startup's heavy daily Claude Code usage since launch. 3,734 stars.
* [claude-forge](https://github.com/sangrokjung/claude-forge) ⭐ 820 | 🐛 31 | 🌐 Shell | 📅 2026-08-29 - oh-my-zsh-inspired plugin framework with 11 AI agents, 36 commands, 15 skills, and 6-layer security hooks. 593 stars.
* [Solopreneur Plugin](https://github.com/pcatattacks/solopreneur-plugin) ⭐ 14 | 🐛 1 | 🌐 Shell | 📅 2026-05-04 - Turns Claude into a virtual company with 6 agents, 16 skills, 1 hooks.json, 2 .mcp.json configs, and a CLAUDE.md. Full product lifecycle: discover → spec → backlog → design → build → review → ship. Includes decision journal and observer protocol. Codex-verified counts.

## Plan-Build-Review Pipelines

Workflows that structure the development cycle into distinct planning, building, and review phases.

* [Superpowers plan-execute](https://github.com/obra/superpowers) ⭐ 279,109 | 🐛 332 | 🌐 Shell | 📅 2026-08-29 - Two-phase workflow: `/write-plan` creates a structured plan, `/execute-plan` implements it step by step with verification gates between steps.
* [gstack autoplan](https://github.com/garrytan/gstack) ⭐ 130,236 | 🐛 810 | 🌐 TypeScript | 📅 2026-08-28 - Auto-chains CEO review → design review → eng review into a single pipeline. Each review phase has its own checklist and acceptance criteria. Found in `/autoplan/SKILL.md`.
* [gmickel-claude-marketplace](https://github.com/gmickel/gmickel-claude-marketplace) ⭐ 689 | 🐛 6 | 🌐 Python | 📅 2026-08-29 - Plan-first workflows (Flow-Next), Ralph autonomous mode for overnight coding, multi-model review gates, re-anchoring to prevent drift, receipt-based gating. 548 stars.
* [shinpr/claude-code-workflows](https://github.com/shinpr/claude-code-workflows) ⭐ 673 | 🐛 0 | 🌐 JavaScript | 📅 2026-08-28 - Production-ready dev workflows with specialized AI agents. Includes frontend plugin with React-specific agents (component architecture, Testing Library, TypeScript-first quality checks) and UI Spec generation.
* [Spec-Flow](https://github.com/marcusgoll/Spec-Flow) ⭐ 91 | 🐛 1 | 🌐 Shell | 📅 2026-04-23 - Turn product ideas into production launches with spec-driven development, repeatable workflows with quality gates, token budgets, and auditable artifacts. 73 stars.
* [Solopreneur sprint](https://github.com/pcatattacks/solopreneur-plugin) ⭐ 14 | 🐛 1 | 🌐 Shell | 📅 2026-05-04 - Parallel feature building with isolated git branches per feature, auto git checkpointing after every skill completion, and agent team kickoff meetings where agents debate approach.

## Multi-Agent Orchestration

Workflows that coordinate multiple AI agents working in parallel or sequence.

* [Superpowers parallel dispatch](https://github.com/obra/superpowers) ⭐ 279,109 | 🐛 332 | 🌐 Shell | 📅 2026-08-29 - Dispatch multiple subagents in parallel, each working on independent subtasks. Includes patterns for collecting results and merging.
* [Everything Claude Code orchestrate](https://github.com/affaan-m/everything-claude-code) ⭐ 244,001 | 🐛 146 | 🌐 JavaScript | 📅 2026-08-29 - Multi-agent orchestration command that coordinates agents across different roles. Found in `commands/orchestrate.md`.
* [ruflo](https://github.com/ruvnet/ruflo) ⭐ 69,661 | 🐛 859 | 🌐 TypeScript | 📅 2026-08-28 - Agent orchestration platform for deploying multi-agent swarms with distributed intelligence, RAG integration, and native Claude Code/Codex integration. 22,810 stars.
* [wshobson/agents](https://github.com/wshobson/agents) ⭐ 39,232 | 🐛 5 | 🌐 Python | 📅 2026-08-26 - Intelligent automation and multi-agent orchestration for Claude Code with specialized agent roles and coordinated task execution.
* [catlog22/Claude-Code-Workflow](https://github.com/catlog22/Claude-Code-Workflow) ⚠️ Archived - JSON-driven multi-agent cadence-team development framework with intelligent CLI orchestration (Gemini/Qwen/Codex), context-first architecture. 1,555 stars.
* [multi-agent-shogun](https://github.com/yohey-w/multi-agent-shogun) ⭐ 1,419 | 🐛 7 | 🌐 Shell | 📅 2026-08-06 - Samurai-inspired multi-agent system orchestrating parallel AI tasks via tmux with shogun → karo → ashigaru hierarchy. 1,096 stars.
* [agent-council](https://github.com/team-attention/agent-council) ⭐ 139 | 🐛 3 | 🌐 JavaScript | 📅 2025-12-24 - Multi-agent collaboration plugin orchestrating multiple AI agents (Codex CLI, Gemini CLI) for diverse perspectives on the same task. 118 stars.
* [Founder OS queue system](https://github.com/cloudrepo-io/founder-os) ⭐ 19 | 🐛 1 | 📅 2026-02-05 - Queue-based task processing where agents pick up work items autonomously: `/queue:add` → `/queue:work` → `/founder:review`. Includes dependency management and blocked\_by ordering.
* [Solopreneur kickoff](https://github.com/pcatattacks/solopreneur-plugin) ⭐ 14 | 🐛 1 | 🌐 Shell | 📅 2026-05-04 - Agent team meetings where 6 specialist agents debate approach before building.

## Context and Memory Management

Workflows for managing Claude Code's context window, memory persistence, and session continuity.

* [claude-mem](https://github.com/thedotmack/claude-mem) ⭐ 92,526 | 🐛 263 | 🌐 JavaScript | 📅 2026-08-29 - Plugin that auto-captures everything Claude does, compresses it with AI via Agent SDK, and injects relevant context back into future sessions. 39,615 stars.
* [Continuous Claude v3](https://github.com/parcadei/Continuous-Claude-v3) ⭐ 3,932 | 🐛 46 | 🌐 Python | 📅 2026-01-26 - Context management via hooks that maintain state through ledgers and handoffs. MCP execution without context pollution. Agent orchestration with isolated context windows. 3,619 stars.
* [arscontexta](https://github.com/agenticnotetaking/arscontexta) ⭐ 3,482 | 🐛 34 | 🌐 Shell | 📅 2026-02-24 - Plugin that generates individualized knowledge systems from conversation — you describe how you think, and get a complete second brain as markdown files. 2,824 stars.
* [Claude Code Development Kit](https://github.com/peterkrueck/Claude-Code-Development-Kit) ⭐ 1,381 | 🐛 3 | 🌐 Shell | 📅 2026-07-22 - Handle context at scale with custom workflows combining hooks, MCP, and sub-agents working together. 1,330 stars.
* [runesleo/claude-code-workflow](https://github.com/runesleo/claude-code-workflow) ⭐ 711 | 🐛 0 | 🌐 Shell | 📅 2026-08-28 - Battle-tested template for memory management, context engineering, and task routing from 3 months of daily usage. 521 stars.
* [cartographer](https://github.com/kingbootoshi/cartographer) ⭐ 650 | 🐛 5 | 🌐 TypeScript | 📅 2026-05-13 - Plugin that maps and documents codebases of any size using parallel AI subagents. 522 stars.
* [vinicius91carvalho/.claude](https://github.com/vinicius91carvalho/.claude) - Portable workflow system with hooks, agents, skills, and enforcement. Drop-in `.claude/` directory that brings structured context management to any project.

## TDD and Code Quality

Workflows that enforce test-driven development and automated code quality checks.

* [Superpowers TDD](https://github.com/obra/superpowers) ⭐ 279,109 | 🐛 332 | 🌐 Shell | 📅 2026-08-29 - Full red-green-refactor loop: write failing test → implement → verify → refactor. Auto-triggers verification before marking any task complete.
* [Superpowers code review loop](https://github.com/obra/superpowers) ⭐ 279,109 | 🐛 332 | 🌐 Shell | 📅 2026-08-29 - Two-skill combo: `/requesting-code-review` prepares the request, `/receiving-code-review` processes feedback. Uses a dedicated code-reviewer agent.
* [Everything Claude Code TDD](https://github.com/affaan-m/everything-claude-code) ⭐ 244,001 | 🐛 146 | 🌐 JavaScript | 📅 2026-08-29 - TDD workflow with autonomous loop support — agent keeps running test cycles until all pass.
* [gstack QA](https://github.com/garrytan/gstack) ⭐ 130,236 | 🐛 810 | 🌐 TypeScript | 📅 2026-08-28 - Browser-based QA that opens real pages with Playwright, takes screenshots, and validates against acceptance criteria.
* [glebis/claude-skills TDD](https://github.com/glebis/claude-skills) ⭐ 364 | 🐛 9 | 🌐 JavaScript | 📅 2026-08-19 - Multi-agent TDD orchestration with architecturally enforced context isolation via Claude Code's Task tool. Interactive mode pauses at each RED checkpoint; autonomous mode runs all slices end-to-end.
* [claude-pipeline](https://github.com/aaddrick/claude-pipeline) ⭐ 126 | 🐛 3 | 🌐 Shell | 📅 2026-02-25 - Portable multi-agent pipeline with skills, agents, hooks, orchestration scripts, and quality gates. 97 stars.

## Git and PR Automation

Workflows that automate git operations, branching strategies, and pull request management.

* [Superpowers git worktrees](https://github.com/obra/superpowers) ⭐ 279,109 | 🐛 332 | 🌐 Shell | 📅 2026-08-29 - Run parallel workstreams using git worktrees — each agent works in its own isolated copy of the repo.
* [gstack ship pipeline](https://github.com/garrytan/gstack) ⭐ 130,236 | 🐛 810 | 🌐 TypeScript | 📅 2026-08-28 - Full deploy pipeline: merge PR → deploy → post-deploy monitoring loop. Chains `/ship` → `/land-and-deploy` → `/canary` skills.
* [Autoresearch branch-per-run](https://github.com/karpathy/autoresearch) ⭐ 94,874 | 🐛 194 | 🌐 Python | 📅 2026-03-26 - Creates a new git branch for each autonomous experiment run, tracks results in `results.tsv`, keeps or discards based on evaluation.

## Ship and Deploy

Workflows for publishing packages, deploying applications, and monitoring releases.

* [gstack canary deploy](https://github.com/garrytan/gstack) ⭐ 130,236 | 🐛 810 | 🌐 TypeScript | 📅 2026-08-28 - Post-deploy monitoring loop that watches for errors after canary release. Chains deploy → monitor → rollback-if-needed.

## Cross-LLM Collaboration

Workflows that combine Claude Code with other AI models for multi-perspective development.

* [gstack codex second opinion](https://github.com/garrytan/gstack) ⭐ 130,236 | 🐛 810 | 🌐 TypeScript | 📅 2026-08-28 - Multi-AI second opinion via OpenAI Codex during code review. Found in `skills/codex/`.
* [claude-review-loop](https://github.com/hamelsmu/claude-review-loop) ⭐ 726 | 🐛 3 | 🌐 Shell | 📅 2026-03-15 - Plugin implementing automated code review loop with Codex as the reviewer — Claude codes, Codex reviews, iterate until approved. 603 stars.
* [codex-orchestrator](https://github.com/kingbootoshi/codex-orchestrator) ⭐ 349 | 🐛 3 | 🌐 TypeScript | 📅 2026-05-28 - Delegate tasks to OpenAI Codex agents via tmux sessions, designed for Claude Code orchestration. 249 stars.
* [agent-council](https://github.com/team-attention/agent-council) ⭐ 139 | 🐛 3 | 🌐 JavaScript | 📅 2025-12-24 - Multi-agent collaboration orchestrating Claude, Codex CLI, and Gemini CLI for diverse perspectives on the same task. 118 stars.

## Research and Discovery

Workflows for market research, codebase exploration, and knowledge gathering.

* [Everything Claude Code search-first](https://github.com/affaan-m/everything-claude-code) ⭐ 244,001 | 🐛 146 | 🌐 JavaScript | 📅 2026-08-29 - Research before coding — agent searches codebase, docs, and web before writing any code.
* [Everything Claude Code continuous learning](https://github.com/affaan-m/everything-claude-code) ⭐ 244,001 | 🐛 146 | 🌐 JavaScript | 📅 2026-08-29 - Auto-extracts patterns from coding sessions into reusable skills. The agent learns from its own work.
* [Autoresearch autonomous loop](https://github.com/karpathy/autoresearch) ⭐ 94,874 | 🐛 194 | 🌐 Python | 📅 2026-03-26 - Karpathy's autonomous AI research agent: modify code → train for 5 min → evaluate → keep/discard → repeat. Only 10 files — intentionally minimal. program.md is 114 lines of substantive instructions. Codex-verified.
* [glebis/claude-skills deep-research](https://github.com/glebis/claude-skills) ⭐ 364 | 🐛 9 | 🌐 JavaScript | 📅 2026-08-19 - Multi-tool research orchestration combining OpenAI, Firecrawl, and web scraping with structured output. Includes insight-extractor that parses Claude Code's `/insights` into actionable markdown files.

## Browser and Testing

Workflows that combine browser automation with Claude Code for testing and data gathering.

* [gstack browser QA](https://github.com/garrytan/gstack) ⭐ 130,236 | 🐛 810 | 🌐 TypeScript | 📅 2026-08-28 - Opens real web pages via Playwright, takes screenshots, validates UI against acceptance criteria.
* [Pagecast demo recording](https://github.com/mcpware/pagecast) ⭐ 42 | 🐛 0 | 🌐 JavaScript | 📅 2026-03-27 - AI-powered product demo creation. After shipping a feature, AI reads your codebase (README, components, routes) to understand what the product does, then writes a demo script — you can review and adjust the plan before recording. It opens a browser, performs the interactions, and records with tooltip zoom overlays that auto-magnify each click and keystroke so viewers can see exactly what's happening. Exports to GIF/MP4 for README, plus formats optimized for IG Reels, YouTube Shorts, and TikTok. Full MCP workflow: `record_page` → `interact_page` → `stop_recording` → `smart_export` (tooltip mode) or `cinematic_export` (crop-pan mode).
* [UI Annotator + Claude Code](https://github.com/mcpware/ui-annotator-mcp) ⭐ 16 | 🐛 1 | 🌐 JavaScript | 📅 2026-03-24 - Dramatically improves AI-driven UI design and iteration. The pain: telling AI "move that button next to the search bar" never works because the AI can't see your page. UI Annotator fixes this — hover over any element and its component name appears as a label. Now you say "move `SearchButton` below `NavBar`" and Claude edits the right component instantly. No browser extensions, works with any framework. The workflow becomes: open page → hover to identify elements → describe changes using real component names → Claude edits → refresh and repeat. Turns a frustrating back-and-forth into a fluid design loop.

## Marketing and Content

Workflows for content creation, social media posting, and distribution.

* [Everything Claude Code content engine](https://github.com/affaan-m/everything-claude-code) ⭐ 244,001 | 🐛 146 | 🌐 JavaScript | 📅 2026-08-29 - Skills for article writing, market research, and investor materials.
* [Agency Agents marketing suite](https://github.com/msitarzewski/agency-agents) ⭐ 148,658 | 🐛 142 | 🌐 Shell | 📅 2026-08-26 - 156 agent persona files across 13 categories including marketing, engineering, design, sales, and more. Install script converts to Claude Code, Cursor, or Copilot format. By Michael Sitarzewski. Codex-verified counts. 15K stars.
* [OPC Skills solopreneur marketing](https://github.com/ReScienceLab/opc-skills) ⭐ 1,701 | 🐛 11 | 🌐 Python | 📅 2026-08-28 - 10 standalone skills for solopreneurs: SEO/GEO optimization, Reddit research, Product Hunt search, domain hunting, logo creation, banner creation. 612 stars.

## Business Operating Systems

Complete systems that use Claude Code as the operating layer for running a business.

* [Founder OS](https://github.com/cloudrepo-io/founder-os) ⭐ 19 | 🐛 1 | 📅 2026-02-05 - Queue-based markdown OS: autonomous task processing, research pipelines, institutional memory, context budgeting, goal-backward verification. Everything is markdown files — zero infrastructure.
* [BOS-AI](https://github.com/TheWayWithin/BOS-AI) ⭐ 7 | 🐛 1 | 🌐 Shell | 📅 2026-08-23 - Business Operating System with 42 agents, 17 commands, 183 missions across business domains, 3 CLAUDE.md files, and the Business Chassis formula. By Jamie (TheWayWithin). Codex-verified counts.
* [ABF (Agentic Business Framework)](https://github.com/alexclowe/abf) ⭐ 0 | 🐛 10 | 🌐 TypeScript | 📅 2026-08-09 - Full TypeScript runtime for agent-as-employee companies. Seed-to-company pipeline: upload business plan → LLM generates agent team + workflows. YAML workflow definitions, approval queues, behavioral bounds.

## Autonomous Loops

Workflows where Claude Code runs continuously without human intervention.

* [Everything Claude Code autonomous loops](https://github.com/affaan-m/everything-claude-code) ⭐ 244,001 | 🐛 146 | 🌐 JavaScript | 📅 2026-08-29 - Start and manage autonomous agent loops that keep running until a goal is met. Commands: `/loop-start`, `/loop-status`.
* [Autoresearch experiment loop](https://github.com/karpathy/autoresearch) ⭐ 94,874 | 🐛 194 | 🌐 Python | 📅 2026-03-26 - Agent autonomously modifies code, runs 5-minute experiments, evaluates results, and repeats. No human in the loop during runs.

## Scope and Config Management

Workflows for managing Claude Code's own configuration across scopes.

* [gstack freeze/guard/unfreeze](https://github.com/garrytan/gstack) ⭐ 130,236 | 🐛 810 | 🌐 TypeScript | 📅 2026-08-28 - File protection system using `PreToolUse` hook definitions in SKILL.md frontmatter with real shell scripts. Note: enforcement only works in Claude Code — Codex/non-Claude versions are advisory prose only. No hooks.json file exists.
* [agent-skill-manager (asm)](https://github.com/luongnv89/asm) ⭐ 901 | 🐛 22 | 🌐 TypeScript | 📅 2026-08-28 - Universal CLI/TUI for managing AI agent skills across 17 providers (Claude Code, Codex, Cursor, Windsurf, and more). Install from GitHub, security scan before install, detect duplicates, and audit skills across all agents from one tool. Online catalog with 2,800+ searchable skills.
* [claude-code-skill-factory](https://github.com/alirezarezvani/claude-code-skill-factory) ⭐ 854 | 🐛 27 | 🌐 Python | 📅 2025-11-12 - Toolkit for building and deploying production-ready Claude Skills, agents, slash commands, and LLM prompts at scale. Generates structured skill templates with 7 hook event types and safety validation.
* [Claude Code Organizer](https://github.com/mcpware/claude-code-organizer) ⭐ 376 | 🐛 12 | 🌐 JavaScript | 📅 2026-06-07 - Web dashboard + MCP server that scans `~/.claude/`, shows scope hierarchy (Global → Workspace → Project), and lets you drag-and-drop config between scopes. 4 MCP tools for programmatic scope management.

## Monitoring and Dashboards

Workflows for tracking Claude Code activity and visualizing progress.

* [claude-hud](https://github.com/jarrodwatts/claude-hud) ⭐ 27,715 | 🐛 1 | 🌐 JavaScript | 📅 2026-08-28 - Plugin that shows real-time context usage, active tools, running agents, and todo progress as a dashboard overlay. 11,537 stars.
* [ccproxy](https://github.com/starbaser/ccproxy) ⭐ 345 | 🐛 9 | 🌐 Python | 📅 2026-08-10 - Proxy that hooks into Claude Code requests for intelligent model routing, request/response modification, and LangFuse tracking. 189 stars.
* [cc-context-stats](https://github.com/luongnv89/cc-context-stats) ⭐ 115 | 🐛 1 | 🌐 Python | 📅 2026-08-26 - Real-time Model Intelligence (MI) score in your status bar — calibrated from Anthropic's MRCR benchmark per model (Opus/Sonnet/Haiku). Live ASCII dashboard tracks context growth, MI degradation, and token I/O. Five color-coded zones tell you when to plan, when to code-only, and when to start fresh. Python, Node.js, and Bash implementations.

## Comprehensive Frameworks

All-in-one frameworks that bundle skills, hooks, agents, and commands into a single installable package.

* [Everything Claude Code](https://github.com/affaan-m/everything-claude-code) ⭐ 244,001 | 🐛 146 | 🌐 JavaScript | 📅 2026-08-29 - 28 agents, 59 commands, 116 skills, 26 hook entries across 7 event groups with 27 hook scripts, language-specific rules for 13 languages, and autonomous loop management. By Affaan Mustafa (Anthropic hackathon winner). 17K stars.
* [shanraisshan/claude-code-best-practice](https://github.com/shanraisshan/claude-code-best-practice) ⭐ 65,312 | 🐛 45 | 🌐 HTML | 📅 2026-08-29 - Trending on GitHub March 2026. Interactive examples of Command → Agent → Skill orchestration pattern. Shows how to chain commands into multi-step workflows with reports and verification gates.
* [luongnv89/claude-howto](https://github.com/luongnv89/claude-howto) ⭐ 41,250 | 🐛 29 | 🌐 Python | 📅 2026-08-26 - Visual 10-module guide showing how to combine slash commands + hooks + skills + subagents + MCP into end-to-end workflows. Copy-paste templates for automated code review, CI/CD automation, and security audit pipelines.
* [claude-code-infrastructure-showcase](https://github.com/diet103/claude-code-infrastructure-showcase) ⭐ 10,013 | 🐛 18 | 🌐 TypeScript | 📅 2026-07-13 - Full showcase of Claude Code infrastructure with skill auto-activation, hooks, and agents working together as an integrated system. 9,315 stars.
* [ChrisWiles/claude-code-showcase](https://github.com/ChrisWiles/claude-code-showcase) ⭐ 6,032 | 🐛 12 | 🌐 JavaScript | 📅 2026-01-06 - Comprehensive project config combining hooks, skills, agents, commands, and GitHub Actions workflows. 5,571 stars.
* [claude-code-plugins-plus-skills](https://github.com/jeremylongshore/claude-code-plugins-plus-skills) ⭐ 2,686 | 🐛 46 | 🌐 Python | 📅 2026-08-29 - 340 plugins + 1,367 agent skills with CCPI package manager, interactive tutorials, and production orchestration patterns. 1,689 stars.
* [CloudAI-X/claude-workflow-v2](https://github.com/CloudAI-X/claude-workflow-v2) ⭐ 1,410 | 🐛 12 | 🌐 Python | 📅 2026-08-25 - Universal Claude Code workflow plugin with agents, skills, hooks, and commands combined into one installable package. 1,301 stars.

***

## Related Awesome Lists

* [awesome-mcp-servers](https://github.com/punkpeye/awesome-mcp-servers) ⭐ 93,010 | 🐛 3,712 | 📅 2026-08-27 - The definitive list of MCP servers. 83K stars.
* [awesome-claude-skills](https://github.com/ComposioHQ/awesome-claude-skills) ⭐ 73,828 | 🐛 1,346 | 🌐 Python | 📅 2026-08-10 - Claude Code skills collection. 47K stars.
* [awesome-claude-code](https://github.com/hesreallyhim/awesome-claude-code) ⭐ 53,149 | 🐛 945 | 🌐 Python | 📅 2026-08-29 - Comprehensive catalog of Claude Code tools, skills, hooks, agents, and plugins. 30K stars.
* [awesome-claude-skills (travisvn)](https://github.com/travisvn/awesome-claude-skills) ⭐ 14,873 | 🐛 773 | 📅 2026-04-28 - Another curated Claude Code skills list with different curation focus.
* [awesome-vibe-coding](https://github.com/filipecalegario/awesome-vibe-coding) ⭐ 5,180 | 🐛 156 | 📅 2026-04-16 - Vibe coding tools and resources. 3.6K stars.
* [awesome-claude-code-hooks](https://github.com/ithiria894/awesome-claude-code-hooks) ⭐ 23 | 🐛 1 | 📅 2026-03-24 - Curated collection of Claude Code hooks for event-driven automation.

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines. We curate, not collect — not every submission will be accepted.

***

> _Enhansomed by [enhansome](https://github.com/enhansome) on 2026-08-29._
