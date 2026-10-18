# Git and GitHub the Safe Way

The practice repository for [Git and GitHub the Safe Way](https://www.t0ul.com/blog/introducing-git-and-github-the-safe-way/), a short free book on git, GitHub, and the four habits that keep a repository from hurting you: no leaked secret, no lost work, no surprise change to `main`, nobody acting as you.

Everything the book's chapters quote lives here, in the form the book recommends:

- `.githooks/pre-commit`: the TruffleHog scan that refuses a commit holding a live credential (chapter 4). After cloning, run `git config core.hooksPath .githooks` once.
- `.github/workflows/ci.yml`: the check that must pass before anything merges to `main` (chapter 6).
- `.github/CODEOWNERS`: who reviews what (chapter 6).
- `.env.example` and `.gitignore`: the ignore-and-example pattern (chapter 4).
- `recipes/pancakes.md`: the file the examples edit. Make your own changes to it; it is here to be practised on.
- `CONTRIBUTORS.md`: add your name as your first pull request (chapter 5).

`main` is protected by a ruleset exactly as chapter 6 describes: changes arrive by pull request, the check must pass, force pushes and deletions are blocked. Fork the repository, make a branch, open a pull request, and watch it all happen.

The book's text is on t0ul.com. The files here are MIT-licensed; copy them into your own projects.
