# One-time setup

Do this **once** on your laptop, then never again. When you're done, use your
browser's **Back** button to return to your assignment.

## Meet the terminal

Open VS Code. In the menu bar, choose **Terminal → New Terminal**. A panel
opens at the bottom. That's the **terminal**: a text chat with your computer.
You type an order, press `Enter`, and the computer answers.

- **You can paste orders.** Real pirates don't hand-copy maps. Paste with
  `Ctrl+V`.
- **Red text doesn't mean you broke something.** It's the computer saying
  "I didn't understand." Read it, then check
  [Troubleshooting](troubleshooting.md).
- **Nothing on this page can hurt your computer.**

Give the orders below **one box at a time**. Wait for each one to finish (the
blinking cursor comes back) before pasting the next.

## Order 1: install the Classroom 50 extension

The GitHub CLI (`gh`) can learn new tricks from **extensions**. This one,
`gh student`, connects you to your classroom on
[classroom50.org](https://classroom50.org):

```sh
gh extension install foundation50/gh-student
```

Check it worked:

```sh
gh student --version
```

You should see `gh-student version` and a number.

## Order 2: install the test runner

```sh
python -m pip install pytest
```

## Order 3: make sure nobody else is signed in

```sh
gh student whoami
```

If it shows **someone else's** username, run `gh student logout`. If it shows
yours, skip Order 4.

## Order 4: sign in to GitHub

```sh
gh student login
```

It asks a few questions. **Press `Enter` for every one.** It shows a code like
`ABCD-1234`: press `Enter`, a browser opens, paste the code, and click
**Authorize**.

## Order 5: sign your work

Git puts your name on every snapshot you save. This sets it to your GitHub
username:

```sh
git config --global user.name "$(gh api user -q .login)"
git config --global user.email "$(gh api user --template '{{.id}}+{{.login}}@users.noreply.github.com')"
```

✅ **Checkpoint:** `python -m pytest --version` prints `pytest` and a version
number. You're ready to sail!

---

Curious what `gh student` can do? See the
[Classroom 50 CLI Student Guide](https://github.com/foundation50/classroom50/blob/main/wiki/CLI-Student-Guide.md).
