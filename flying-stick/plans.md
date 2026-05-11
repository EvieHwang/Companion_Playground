# Tiered Agentic Build Framework — Next Steps

## Immediate

- [ ] Fix template repo spec (dag.md and state.md paths, 
      remove docs/ root folder, updated research and verify 
      skills, t3-feature-declaration command, state file 
      format in constitution, features/README.md)
- [ ] Set up template repo with corrected structure
- [ ] Confirm hook implementation — settings.json 
      vs embedded in t3-generate-dag

## Road test — Tier 2

Target: Python script that takes CSV input and produces 
a weekly analysis, replacing a manual employee workflow.

- [ ] Run t2-intent, t2-plan, t2-verify, t2-build
- [ ] Note what the documents missed
- [ ] Note where the build needed context that 
      wasn't in the documents
- [ ] Update constitution and command files accordingly

## Carry forward from testing

- [ ] Feature-name parameter handling in commands
- [ ] Sub-agent invocation mechanism in t3-build
- [ ] Adversarial review as isolated sub-agents
- [ ] Single vs two pre-build sessions in practice

## Road test — Tier 3

Target: MCP Gateway rebuild on Eviebot.
Hold until Tier 2 road test is complete and 
framework is stable.


# Companion Playground — Personal Agent / Thinking Partner
Design largely settled in conversation. Not yet built.
Architecture: Claude Code + GitHub repo. Eviebot is the 
natural host.

## Design decisions made
- Repo as persistent memory layer; CLAUDE.md auto-loads 
  context at session start
- Three focus areas: job search, WA Commission, Flying Stick
- Session reset is user-initiated ("when I've lost the thread"), 
  not on a schedule
- Wrap-up command: agent surfaces potential file updates, 
  Evie decides what gets committed
- Dispatch explored as phone interface — promising given 
  always-on Eviebot, but single-thread constraint conflicts 
  with session reset model; revisit when more stable

## Repo structure (designed, not created)
- CLAUDE.md — orientation + behavior
- plans/job-search.md
- plans/commission.md
- plans/flying-stick.md
- inbox.md

## Next steps
- [ ] Create repo
- [ ] Draft CLAUDE.md (skeleton drafted in conversation)
- [ ] Populate three plan files manually
- [ ] Run first session and note what's missing
