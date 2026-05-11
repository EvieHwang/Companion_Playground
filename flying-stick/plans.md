```markdown
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
```
