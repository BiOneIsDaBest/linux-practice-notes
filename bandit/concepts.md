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

## Listing files and reading permissions

```bash
ls -la
```

- `-l` = long format (permissions, owner, group, size, date)
- `-a` = show **hidden files** (names starting with `.`)

```text
-rw-r-----  1 bandit1 bandit0  438  readme
```

| Part | Meaning |
|---|---|
| `-` | Regular file (`d` = directory) |
| `rw-` | Owner can read and write |
| `r--` | Group can read |
| `---` | Others have no access |

- I can read a file if I am the owner, **or in the group**, or if "others" has read permission.
- Security use: wrong permissions on sensitive files are a common misconfiguration and a path to privilege escalation.

> Linux file permissions control who can read, write or execute a file.

---

<!-- Add a new section each time I learn a new concept -->
