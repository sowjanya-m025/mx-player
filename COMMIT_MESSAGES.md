# Commit messages for mx_player

Run these inside the project folder. The first block makes sure your commits are
credited to the right GitHub account.

```sh
git init -b main
git config user.name "sowjanya-m025"
git config user.email "sowjanyamurgesh04@gmail.com"
```

## Commits

```sh
git add .gitignore .gitattributes
git commit -m "chore: add gitignore and line-ending rules"

git add .vscode lib
git commit -m "chore: add VS Code Java settings and lib folder for dependencies"

git add src
git commit -m "feat: add App entry point"

git add README.md COMMIT_MESSAGES.md
git commit -m "docs: add README and commit message guide"
```

## Push

Create an empty repo on GitHub first, then:

```sh
git remote add origin https://sowjanya-m025@github.com/sowjanya-m025/<repo-name>.git
git push -u origin main
```

Use a Personal Access Token as the password.
