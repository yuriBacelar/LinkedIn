# LinkedIn — Codex repository instructions

## Factory context discovery (when applicable)

1. Identify the active Git repository and read its root `context.yaml`, if present. Never infer customer, project or inheritance from a repository name alone.
2. When the manifest exists, use the reviewed `context-resolution` capability from Software Factory to resolve pinned parent commits through the central trust policy in `engineering-config/trust.yaml`. Respect access, commit pins and resolver failures; never bypass trust or substitute a local policy.
3. Discover relevant agents and skills at `.codex/agents/` and `.agents/skills/`, locally and in approved parents at their resolved revisions. Load or install them only through supported mechanisms. Neither `context.yaml` nor a Git URL automatically activates Codex capabilities.
4. Preserve applicable repository and nested `AGENTS.md` instructions; apply more specific approved decisions within their scopes and report conflicting requirements.
5. Keep work in its owning repository. Do not modify parents or central trust as a side effect, duplicate inherited components, or invent missing conventions. State unresolved access and validation gaps.

If the root `context.yaml` is absent, **no Software Factory inheritance is declared here**. Follow existing local instructions without assuming a parent. This `AGENTS.md` is a discovery entrypoint, not a context resolver.
