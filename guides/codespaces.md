# Working in a codespace

A **codespace** is VS Code running in your browser on a GitHub computer, with
your repository already on it. Days 1 and 2 use one. After that, your school
laptop is home base, but a codespace works for every assignment when you don't
have your laptop (it's broken, at school, or you're on a family computer).

## Open one

1. Sign in to [github.com](https://github.com) with your school GitHub account
   and open your assignment repository (its link is on
   [classroom50.org](https://classroom50.org) under **My submission**).
2. Click the green **Code** button, choose the **Codespaces** tab, and click
   **Create codespace on main**. It takes about a minute to start.
Everything works the same as on a laptop: the steps, the tests, **Source
Control**, and **Sync Changes**. The test runner is installed for you.

If `python -m pytest -q` says `No module named pytest`, the setup didn't
finish. Paste this once:

```sh
python -m pip install pytest
```

## Mind the quota

Codespaces are free up to a limit, and the limit is **yours**, not the
school's: a free GitHub account gets **120 core-hours a month**. The smallest
codespace uses 2 cores, so that's about **60 hours of running time**. Stopped
codespaces still use some of your monthly storage.

- **Stop it when you're done.** Click the **Codespaces** menu in the bottom-left
  corner and choose **Stop Current Codespace**. (It also stops itself after 30
  minutes of inactivity, but don't count on that.)
- **Delete it when the assignment is done.** On github.com, click your profile
  picture → **Your codespaces** → **⋯** → **Delete**.
- **One codespace per assignment.** Reopen the same one instead of creating a
  new one.
- **Keep the default machine size.** A bigger machine burns the quota faster.
- **Check your usage** at github.com → profile picture → **Settings** →
  **Billing and licensing** → **Usage**.

If you run out, the codespace won't start until next month. Your work is safe
on GitHub as long as you clicked **Sync Changes**.

## Switching between laptop and codespace

Git only knows about work you've **synced**. Before you switch computers, click
**Sync Changes**. When you sit down at the other one, click **Sync Changes**
again before you edit anything.
