# rhuss' Claude Code Plugin Marketplace

This repository contains custom Claude Code plugins for security, development, and automation workflows.

## Available Plugins

### 🔒 threat-model-assessment

Turn security requirements into actionable code assessments. Provide a threat description and your code repositories, and the plugin analyzes your implementation to identify what's in place and what's missing.

**How it works:**
1. Paste a security requirement from your threat model
2. Specify your code repositories (local or Git URLs)
3. AI analyzes the code to assess current security controls
4. Receive detailed findings with file references and gap analysis
5. Optionally auto-generate JIRA tickets for remediation work

**Perfect for:**
- Architects validating security designs against actual implementation
- Developers ensuring security requirements are properly coded
- Security teams conducting compliance assessments
- Anyone who needs to verify code matches security requirements

[→ View Plugin Documentation](https://github.com/rhuss/cc-threat-model-assessment)

### 📋 spex

Specification-Driven Development with Process Discipline for Claude Code. Refine rough ideas into executable specifications through collaborative brainstorming, then implement with structured workflows, quality gates, and spec compliance verification.

**How it works:**
1. Brainstorm and refine ideas into executable specifications
2. Review specs for soundness, completeness, and implementability
3. Plan implementation with coverage validation and red flag scanning
4. Implement in isolated worktrees with spec guardian review
5. Verify spec compliance and evolve specs when code diverges

**Perfect for:**
- Teams practicing specification-driven development
- Projects requiring formal specification documentation
- Developers who want structured, spec-first workflows
- Organizations implementing quality gates and compliance checks

[→ View Plugin Documentation](https://github.com/rhuss/cc-spex)

### ✍️ prose

Write natural, human-sounding prose with AI pattern detection, voice profiles, and style enforcement. Catches and removes 24 categories of AI writing indicators to produce authentic content.

**How it works:**
1. Initialize style configuration with /prose:init
2. Create or extract voice profiles from writing samples
3. Generate new content with style enforcement and voice consistency
4. Validate content against AI pattern checklist before publishing
5. Rewrite existing text to remove AI-generated artifacts

**Perfect for:**
- Technical writers who want natural-sounding documentation
- Blog authors maintaining a consistent personal voice
- Content creators who need AI assistance without AI fingerprints
- Anyone reviewing text for unintentional AI patterns

[→ View Plugin Documentation](https://github.com/rhuss/cc-prose)

### 🎯 slidev

Create developer-focused technical presentations using Slidev with enforced evidence-based design guardrails. Complete workflow from brainstorming to LaTeX handouts.

**How it works:**
1. Initialize presentation with /slidev:init
2. Interactive brainstorming with web research
3. Auto-generate structured outline
4. Create modular slides with enforced quality (≤6 elements, <50 words)
5. Add multi-platform diagrams (Mermaid, PlantUML, Excalidraw)
6. Generate presenter notes and LaTeX handouts
7. Export to PDF/PPTX

**Perfect for:**
- Conference talks and tech meetups
- Internal technical demos and architecture reviews
- Developer training and workshops
- Open source presentations with Git collaboration

[→ View Plugin Documentation](https://github.com/rhuss/cc-slidev)

## Installation

**Step 1:** Add this marketplace to Claude Code:

```
/plugin marketplace add rhuss/cc-rhuss-marketplace
```

**Step 2:** Install any plugin from the marketplace:

```
/plugin install <plugin-name>@cc-rhuss-marketplace
```

**Step 3:** Invoke the plugin using its slash command:

```
/<plugin-name>
```

**Example** (installing threat-model-assessment):
```
/plugin install threat-model-assessment@cc-rhuss-marketplace
/threat-model-assessment
```

## Contributing

This is a personal plugin marketplace, but suggestions and improvements are welcome!

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

## License

MIT License - see individual plugin directories for specific licensing.

## Author

Roland Huß (@rhuss)

## Resources

- [Claude Code Documentation](https://docs.claude.com/claude-code)
- [Plugin Development Guide](https://docs.claude.com/claude-code/plugins)
- [Skill Framework Reference](https://docs.claude.com/claude-code/skills)
