# opencode-kiro-auth (framed-system fork)

Fork of @magpie-community/opencode-kiro-auth (v0.1.11). Kiro's server puts
its own agent prompt ("Kiro", in kiro-cli) above every request; this fork
counters it:

- the caller's system prompt goes in a framed turn of its own that opens
  the conversation, answered once as Claude, and the message being
  answered ends with a short identity reminder;
- the harness and the frame (a fixed size per model) are deducted from the
  input usage reported, so relays bill callers for their own tokens only.

See branch kiro-framed-system of Arismemo/plugins for the monorepo commits.
