<!--
PR title: Conventional Commits, imperative, no final period, e.g. "feat(engine): add the mule account rule"
Branch:   type/TICKET-short-description, e.g. feature/MAG-123-mule-rule, bugfix/MAG-130-postgres-port
Keep it small: ideally under 10 files and a few hundred lines. Open it as Draft while you work.
-->

## ✨ Context

<!-- What task this solves and why it is needed. -->

Related: <!-- Jira ticket (e.g. MAG-123), issue (e.g. Closes #12) or other PRs this depends on -->

## Type of change

<!-- Keep the ones that apply and delete the rest. -->

- [ ] ✨ New feature
- [ ] 🐛 Bug fix
- [ ] 💥 Breaking change
- [ ] 📝 Documentation
- [ ] 🔥 Refactor or improvement
- [ ] ✅ Tests
- [ ] 👷 CI, infrastructure or configuration

## 🛠 Before / After

**Before:** <!-- How it worked (or failed) before this change. -->

**After:** <!-- How it works now. -->

## 🧠 How and why

<!-- The main changes, file by file if it helps the reviewer, and why they were made this way (trade-offs, alternatives discarded). -->

## 🙈 Missing

<!-- Anything the task asked for that this PR does not cover yet. Write "Nothing" if complete. -->

## 🧪 How to test

<!--
Steps the reviewer can copy: where to run each command (repo, folder or service),
what has to be running first (e.g. docker compose up -d) and the expected result.
Example:
1. In SecurePay: `docker compose up -d`
2. In SecurePay: `uv run pytest services/decision_engine/tests/test_mule.py` → 12 passed
3. In securepay-generator: `uv run python -m securepay_generator` → `Listo: 1036 eventos`
-->

1.
2.

## Checklist

- [ ] Tests pass locally
- [ ] README and AGENTS.md updated if setup, commands or env vars changed
- [ ] Docusaurus updated if the documented behavior changed
- [ ] Code, comments and commit messages in English
- [ ] No secrets or `.env` values in the diff
- [ ] Reviewers assigned
