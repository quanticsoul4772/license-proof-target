# Contributing to license-proof-target

Thank you for your interest in contributing! This repository is intentionally
small — at the moment it contains only a `LICENSE` file and a `README.md` —
so contributing is straightforward. This guide walks you through the whole
process, from forking the repository to opening a pull request.

## 1. Fork and clone the repository

1. Visit the repository on GitHub:
   `https://github.com/quanticsoul4772/license-proof-target`
2. Click the **Fork** button (top right) to create your own copy under your
   GitHub account.
3. Clone your fork to your machine:

   ```sh
   git clone https://github.com/<your-username>/license-proof-target.git
   cd license-proof-target
   ```

4. (Recommended) Add the original repository as the `upstream` remote so you
   can keep your fork up to date:

   ```sh
   git remote add upstream https://github.com/quanticsoul4772/license-proof-target.git
   git fetch upstream
   ```

## 2. Create a topic branch

Never work directly on `main`. Create a short-lived topic branch named after
the change you intend to make:

```sh
git checkout main
git pull upstream main   # make sure you start from the latest default branch
git checkout -b <topic-branch-name>
```

Use a descriptive branch name, e.g. `fix-readme-typo` or
`clarify-license-note`.

## 3. Make your edits

Edit the files with any text editor. Since the repository currently consists
of documentation and a license file, most contributions will be text changes:

- Keep changes focused: one topic branch should address one logical change.
- Match the style and tone of the existing files.
- Preview Markdown changes (e.g. in your editor or on GitHub) to make sure
  formatting renders as intended.
- Do **not** modify the terms of the `LICENSE` file.

## 4. No build or install step (today)

There is currently **no build, install, or test step** in this repository:
there is no package manifest (such as `package.json`, `pyproject.toml`, or
similar), no dependency list, no test suite, and no CI pipeline. You can
verify your changes simply by reading the edited files.

If a package manifest or build configuration is added to the repository in
the future, check that file (and any updated README instructions) for the
then-current setup and verification steps before submitting changes.

## 5. Commit message expectations

Write commit messages that make the history easy to read:

- Use a short, imperative summary line (roughly 50 characters or fewer),
  e.g. `Fix typo in README` — not `fixed stuff` or `updates`.
- If the change needs explanation, add a blank line after the summary and
  then a body describing *what* changed and *why*.
- Keep each commit to one logical change; avoid mixing unrelated edits in a
  single commit.

Example:

```
Clarify repository purpose in README

The opening paragraph did not explain what the proof exercise covers.
Expand it so first-time readers understand the repository's role.
```

## 6. Open a pull request

1. Push your topic branch to your fork:

   ```sh
   git push origin <topic-branch-name>
   ```

2. On GitHub, open a pull request from your branch against the **`main`**
   branch (the default branch) of
   `quanticsoul4772/license-proof-target`.
3. Give the pull request a clear title and a description that explains what
   the change does and why it is needed.

### What reviewers will look for

- **Clarity** — the change is easy to understand, well written, and the pull
  request description explains its purpose.
- **Adherence to the existing LICENSE terms** — the contribution is
  compatible with the repository's MIT license and does not alter or
  conflict with it.
- **No unrelated changes** — the diff contains only what the pull request
  says it does; drive-by edits belong in separate pull requests.

## Licensing of contributions

By submitting a contribution, you agree that it is provided under the terms
of the repository's existing [`LICENSE`](LICENSE) (the MIT License). No
separate contributor agreement is required.
