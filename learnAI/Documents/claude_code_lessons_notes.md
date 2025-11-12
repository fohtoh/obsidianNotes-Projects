# 6 Months of Claude Code Lessons in 27 Minutes

**Video by:** AI with Avthar
**Duration:** 26 minutes
**Upload Date:** September 3, 2025
**Video URL:** https://www.youtube.com/watch?v=rfDvkSkelhg

## Video Description

This comprehensive guide shares 36 specific lessons that transformed the creator from a Claude Code beginner to a power user. The lessons are organized into three clear levels: beginner, intermediate, and master. These are battle-tested techniques used daily to ship real projects faster than ever before.

---

## Table of Contents

1. [Level 1: Beginner (Foundations)](#level-1-beginner-foundations)
2. [Level 2: Intermediate (Workflow Enhancements)](#level-2-intermediate-workflow-enhancements)
3. [Level 3: Master (Advanced Techniques)](#level-3-master-advanced-techniques)
4. [Cost and Value](#cost-and-value)

---

## Level 1: Beginner (Foundations)

### Installation & Setup

**Tip 1: Local Installation**
- Install Claude Code on your local laptop/machine
- Go to Anthropic website and copy the command
- Quick and easy setup to begin coding right away

**Tip 2: Remote Server Installation**
- Great for back-end projects
- Install on AWS, Digital Ocean, or Hetzner
- Benefit: Code from anywhere (even from your phone using Termius app on iOS)

**Tip 3: Use Inside Other AI Coding Tools**
- Can use Claude Code inside Cursor, Windsurf, etc.
- Great if you're already familiar with those tools or getting comfortable with terminal
- Navigate to directory and type `claude` in terminal
- Use resume flag (`claude --resume`) to resume previous sessions

### Essential Concepts & Commands

**Tip 4: To-Do Lists**
- Favorite feature that made Claude Code stand out
- Automatically created for most tasks (can also explicitly prompt for it)
- Shows what's happening and what's coming next
- Enables Claude to work on big complex tasks without getting stuck in loops
- Checks off items as Claude works

**Tip 5: Bash Mode**
- Run bash commands inside Claude Code without exiting
- Claude can run bash commands itself:
  - Read and write files
  - Search
  - Handle git commands
- Example: Tell Claude to read all files in a folder for context

**Tip 6: Instant Documentation**
- Ask Claude to explore and explain app architecture
- Save output in files like `architecture.md`
- Great for:
  - Getting up to speed with new projects
  - Documenting key things for teammates
  - Reference for future Claude sessions

**Tip 7: (Not numbered in transcript)**

**Tip 8: Auto Accept Mode**
- Press Shift + Tab together to enable
- Lets Claude make changes without asking each time
- Use when you want to "let Claude take the wheel"

**Tip 9: Model Switching**
- Use `/model` command to choose which model to use
- **Opus**: Most powerful model for deeper analysis and toughest challenges
- **Sonnet**: For routine tasks, saves tokens, faster responses
- **Default mode**: Uses Opus until 50% of monthly usage limit
- **Recommended**: Opus plan mode (Opus for planning, Sonnet for implementation)

**Tip 10: Don't Be Afraid to Interrupt**
- Press Escape key once to interrupt Claude
- Press Escape twice to go back to previous prompt
- Better to redirect early than waste tokens

### Debugging with Claude Code

**Tip 11: Screenshot Method**
- Claude Code accepts images as input
- Take screenshots of UI issues or bugs
- Claude can see all context and pinpoint problems
- Also useful for: UI designs and diagrams

**Tip 12: Let Claude Write Tests**
- Simply ask Claude to write tests for features
- Example: "Write tests for the new onboarding flow"
- Focus on general end-to-end tests rather than implementation-specific ones

**Tip 13: Test-Driven Development (TDD)**
- Ask Claude to first write tests for a feature, then implement it
- Helps Claude catch issues early
- Provides structure for better outputs

### Project Configuration

**Tip 14: The claude.md File** (MOST IMPORTANT)
- Your project's memory
- Gets added to context every single time Claude works
- Contains information you want Claude to know about your project
- Should include:
  - Git workflows and best practices
  - Project and architecture overviews
  - Build commands
  - Testing and debugging best practices
  - Analytics and documentation how-tos
- Claude will follow these rules automatically
- **Pro tip**: Ask Claude to write it for you
- Update as you add features or discover preferences

**Tip 15: Message Queue**
- Game-changer feature
- Type messages while Claude is working
- Messages get added to queue
- Claude will act on them once current task is finished
- No need to wait for Claude to finish

**Tip 16: Markdown File Prompts**
- For long prompts, put prompt in a markdown file
- Reference file using @ symbol in Claude
- Much cleaner than typing everything in terminal
- Great for long prompts or when you want to think things through first

---

## Level 2: Intermediate (Workflow Enhancements)

### Planning & Thinking Features

**Tip 17: Planning Mode**
- Don't jump straight into writing code
- Use planning mode to plan and strategize first
- Press Tab + Shift until you see "plan only" mode
- Claude gives you a plan to review before writing code
- Use for:
  - Architecture decisions
  - Forcing Claude to think through bug fixes before action

**Tip 18: Opus Plan Mode (Hidden Setting)**
- Use Opus for planning
- Use Sonnet for implementation
- Select via `/model` command
- Good default for powerful planning + cost-efficient implementation

**Tip 19: Multiple Plans with Sub-Agents**
- Use sub-agents to create multiple plans for implementing features or fixing bugs
- Explore multiple solutions simultaneously
- Pick the best one yourself or let Claude pick
- (More details in Master section)

**Tip 20: Think Keywords**
- Control how much Claude thinks
- Three levels:
  - **think**: Basic thinking
  - **think hard**: Deeper analysis
  - **ultra think**: Maximum thinking power
- Include appropriate keyword in your prompt
- Uses more of Claude's thinking budget for tough problems

**Power Workflow Example:**
Combine think hard + planning mode + saving output to markdown file for future reference

### More Than Code

**Tip 21: Research with Claude Code**
- Web search and web fetch tools enable searching and reading websites
- Use for:
  - Small research: How to use Stripe API
  - Large research: Reports on best OAuth tools with pre-built login components
- Saves time and takes app context into account

**Tip 22: Claude Can Read PDFs**
- Combine PDF information with web searches
- Example: Feed Claude PDFs of ChatGPT deep research reports for reference during research phase

**Tip 23: Document Generation**
- Think like a product manager and give Claude all needed context
- Use Claude to generate:
  - Product Requirement Docs (PRDs)
  - User experience guides
  - API documentation
  - Technical design docs
- More useful than ChatGPT docs because they leverage actual app structure and project context

**Tip 24: Automatic Change Tracking**
- Create changelogs for Claude to reference later
- Document up-to-date features for website
- Make decision docs outlining why decisions were made
- Keep track of how project evolves over time
- Benefits future self and future Claude Code agents

### GitHub Integration

**Tip 25: GitHub Actions Integration**
- Deep integration with GitHub Actions
- Run `/install gh-actions` from Claude Code menu
- Tag Claude Code in issues and pull requests
- Claude runs using GitHub Actions and submits PR or fix
- Doesn't need to run on local or remote machine
- Claude can review PRs automatically as they come in

### Mindset for Success

**Tip 26: Think Like a Product Manager**
Two key aspects:
1. Give Claude lots of clear, relevant context and constraints
2. Let go of reviewing every line of code

**Key mindset shift:**
- Don't need to understand every line of code Claude outputs
- Verify at higher levels of abstraction:
  - Does the app experience match what you want?
  - Do the tests pass?
  - Does the app work as intended?
- Similar to managing smart technical people in real jobs

---

## Level 3: Master (Advanced Techniques)

### Working in Parallel

**Tip 27: Parallel Sub-Agents for Planning**
- Allows Claude to explore multiple solutions simultaneously
- Like having a team brainstorming session
- Ask Claude to "plan and use parallel sub-agents to explore solutions"
- Great for:
  - Exploring how to add complex features
  - Fixing gnarly bugs or problems
- You or Claude picks the best solution

**Tip 28: Multiple Claude Instances with Git Worktrees**
- Work on multiple features at the same time
- Git worktrees provide isolation without conflicts
- **Setup:**
  1. Create a hidden folder in your project (e.g., `trees`)
  2. Use `git add` commands to create worktree for each feature/thread
  3. Spin up terminal session for each worktree
  4. Run Claude Code in each terminal
- Results in clean git history
- When done, ask Claude to merge worktrees and fix conflicts
- Enables a week's worth of development in just a few minutes

### Advanced Customization

**Tip 29: Custom Commands**
- Prompting shortcuts for repetitive tasks
- Avoid typing same long prompts repeatedly
- **Setup (or ask Claude to do it):**
  1. Create `commands` folder in `.claude` folder
  2. Add markdown file with command name (e.g., `changelog.md`)
  3. File should include:
     - Description of what command does
     - List of allowed tools (bash, read, write, etc.)
     - Actual command prompts
- Command prompts can include:
  - Arguments for dynamic input
  - Bash commands
  - File references

**Tip 30: Personal vs Project Commands**
- Custom commands can be:
  - **Project-specific**: Only for current project
  - **Personal**: Apply to all Claude Code projects
- Note: Custom commands don't automatically get added to context
- For always-added context, use `claude.md` file instead

**Tip 31: Specialized Sub-Agents**
- Create custom sub-agents with custom prompts and tool permissions
- Handle specific tasks autonomously
- Can be project-specific or personal (all projects)
- **Examples:**
  - User experience design
  - API design
  - Security review
  - Running tests
  - Database administration
  - Other domain-specific tasks
- Each has specific accessible tools and domain-specific system prompt

**Tip 32: Creating Sub-Agents**
- Easiest way: Use `/agents` command in Claude Code
- Wizard walks through setting up new agent
- Claude does heavy lifting
- **Under the hood:** Each agent has markdown file specifying:
  - Agent type
  - Usage
  - Accessible tools
  - System prompts (overview of what agent does)
- View all created agents with `/agents` command

**Tip 33: Using Sub-Agents**
- Claude automatically knows about created sub-agents
- Understands usage based on description in agent markdown file
- Automatically delegates tasks to sub-agents when relevant
- Can explicitly ask for sub-agents in prompts
  - Example: "Use the test runner sub-agent to run these tests"
  - Example: "Use the database administration agent to make sure queries are correct"

### MCP Servers

**Tip 34: Model Context Protocol (MCP)**
- Extends Claude Code capabilities to third-party tools
- Actions in databases, Figma, Canva, etc.

**Tip 35: Popular MCP Servers**
- **Database MCPs**: Great for direct database work
  - MongoDB MCP
  - Postgres MCP
  - Supabase MCP
- **Playwright MCP**: Browser automation
  - Claude can visually see web UI
  - Great for testing and finding/fixing bugs
- **Figma MCP**: Going from design to code

**Tip 36: MCP Ecosystem**
- Many other MCP servers available
- Incredibly powerful capabilities
- Will become more powerful as ecosystem matures

---

## Cost and Value

### Pricing Options

**Option 1: Claude Paid Plans**
- **Pro Plan**: $20/month
  - Good to get started or play around
- **Max 5X Plan**: $100/month
  - 5x higher rate limits than Pro
  - Recommended when serious about building
- **Max 20X Plan**: $200/month
  - 20x higher rate limits
  - Creator's personal choice
  - Recommended if serious about AI coding tools

**Option 2: Anthropic API**
- Ridiculously expensive
- Only recommended if part of large company that will pay for API usage
- Otherwise, pick a Claude Pro or Max plan

### Important Notes

- No free version of Claude Code available
- Anthropic announced additional weekly rate limits for Claude Max users (end of August)
- Impact unclear but expected to be minimal
- Claude Code still considered good value for money

---

## Key Takeaways

1. **Foundation is Critical**: The `claude.md` file is the most important thing - it's your project's memory
2. **Think Like a PM**: Give context, verify at high level, don't review every line of code
3. **Use Planning Mode**: Don't jump straight to code - plan first
4. **Leverage Parallelization**: Multiple Claude instances with git worktrees = massive productivity
5. **Extend with MCP**: Integrate with databases and third-party tools for maximum power
6. **Customize Everything**: Custom commands and sub-agents for your specific workflows
7. **Use Todo Lists**: Essential for tracking complex tasks and preventing loops
8. **Documentation Matters**: Generate and maintain docs automatically with Claude

---

## Recommended Workflow

1. Set up `claude.md` file with project context, workflows, and best practices
2. Use planning mode for complex features (with think keywords if needed)
3. Leverage todo lists for tracking progress
4. Use git worktrees for parallel development on multiple features
5. Create custom commands for repetitive tasks
6. Set up specialized sub-agents for domain-specific work
7. Integrate MCP servers for database and third-party tool access
8. Think like a product manager - provide context and verify outcomes, not implementation

---

## Resources

- **YouTube Channel**: [AI with Avthar](https://www.youtube.com/@avtharai)
- **Twitter/X**: [@avthars](https://x.com/avthars)
- **TikTok**: [@vibecoder.com](https://www.tiktok.com/@vibecoder.com)

---

## Timestamps

- 00:00 - Claude Code: The New King of AI Coding?
- 02:14 - Level 1: Beginner
- 02:29 - Installation
- 03:37 - Todo lists
- 04:16 - Essential Commands
- 06:35 - Debugging with Claude Code
- 07:57 - Claude.md file
- 09:33 - Message Queue
- 09:57 - Markdown file prompts
- 10:33 - Level 2: Intermediate
- 10:51 - Planning Modes
- 12:10 - Thinking Modes
- 12:58 - More than Code: Research, Documents, Changelogs
- 15:16 - Github Actions Integration
- 15:59 - Mindset for Success with Claude Code
- 17:23 - Level 3: Master
- 17:48 - Parallel Subagents
- 18:16 - Multiple Claudes (multi-clauding) with Git worktrees
- 19:30 - Custom Slash Commands
- 20:50 - Custom Subagents
- 22:50 - MCP Server Usage
- 24:05 - Cost and Value for Money
- 25:56 - Conclusion: What's next?
