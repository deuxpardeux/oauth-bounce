# Agent instructions for oauth-bounce

## Code graph and workflow maps (Deux par Deux)

Before changing code or workflows, read the Archify map and query Graphify (graphify-latest).

Query Graphify via the
`code_catalog.jsonl` asset on the `graphify-latest` release in
`deuxpardeux/dpd-tools`, then open only the files it names:

```bash
gh release download graphify-latest --repo deuxpardeux/dpd-tools --pattern code_catalog.jsonl --dir /tmp/graphify --clobber
rg -i 'oauth-bounce/' /tmp/graphify/code_catalog.jsonl
```

See dpd-tools `.claude/skills/graphify-query/SKILL.md` and `bridge/GRAPHIFY.md`.
The catalog refreshes at 06:35 and 18:35 UTC; sibling rows use `repo` and
`repo/path` labels. The dependency graph itself covers dpd-tools only.
If the release is unavailable or a file is absent, use a scoped local file
index or GitHub path search. Do not install Graphify MCP on W10.
