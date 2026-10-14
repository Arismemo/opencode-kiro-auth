# opencode-kiro-auth (framed-system fork)

Fork of @magpie-community/opencode-kiro-auth (v0.1.11) with one change:
caller system messages are wrapped in a high-authority frame before being
demoted into Kiro's first user message, fixing the persona/identity leak
caused by Kiro's server-side agent harness prompt. See branch
kiro-framed-system of Arismemo/plugins for the monorepo commit.
