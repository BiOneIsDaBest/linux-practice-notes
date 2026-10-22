# Bandit — Concept Notes

Notes are organised **by concept**, not by level, so they stay useful after the game and do not spoil solutions.

---

## SSH — Remote login

```bash
ssh <user>@<host> -p <port>
```

| Part | Meaning |
|---|---|
| `<user>` | Account on the remote server |
| `<host>` | Server name or IP address |
| `-p <port>` | Port number (SSH default is 22, Bandit uses 2220) |

- First connection shows the server **fingerprint** → typing `yes` saves it in `~/.ssh/known_hosts`.
- If the fingerprint changes later, SSH warns me → possible **man-in-the-middle** or the server was rebuilt.
- Real-world use: admins and SOC analysts connect to Linux servers with SSH every day.

> SSH provides encrypted remote access to a system.

---

<!-- Add a new section each time I learn a new concept -->
