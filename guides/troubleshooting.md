# Troubleshooting: tools

Problems with VS Code, Git, `gh`, or classroom50.org. For problems with the
day's Python code, use the **Help** page linked from your assignment.

| Problem | Fix |
| --- | --- |
| `gh` or `code` isn't recognized | Close and reopen VS Code. Still there? Tell your teacher. |
| `python` isn't recognized | Close and reopen VS Code. Still there? Tell your teacher. |
| `unknown command "student"` | Do [Order 1 of the setup](setup.md#order-1-install-the-classroom-50-extension). |
| `No module named pytest` | Do [Order 2 of the setup](setup.md#order-2-install-the-test-runner). |
| `gh student` says it's out of date | Run `gh extension upgrade gh-student`. |
| Signed in as the wrong person | Run `gh student logout`, then `gh student login`. |
| Git asks who you are | Do [Order 5 of the setup](setup.md#order-5-sign-your-work). |
| Push is rejected | Someone (maybe you, on GitHub) changed the repository first. Click **Sync Changes** again. |
| No scorecard, ✅, or ❌ yet | Grading takes a minute or two after you sync. Refresh the page. Only `main` is graded. |
| No **Codespaces** tab under the **Code** button | Tell your teacher. |
| Codespace stuck on "Setting up" | Wait two minutes, then reload the tab. Still stuck? Delete it (profile picture → **Your codespaces** → **⋯** → **Delete**) and create a new one. |
| Codespace won't start at all | You may be out of free hours. See [the quota](codespaces.md#mind-the-quota). |
| `No module named pytest` in a codespace | Paste `python -m pip install pytest`. |
| My change isn't here | You made it on the other computer. Click **Sync Changes** there, then **Sync Changes** here. |
| No laptop today | Use a [codespace](codespaces.md). |

Still stuck? Ask a crewmate, then your teacher.
