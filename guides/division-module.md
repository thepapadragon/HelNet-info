# Division Module

Divisions are groups within your server that members can join. Admins set them up and configure everything through the Division Wizard. Members interact with them through the Division Terminal.

---

### Division Terminal

The Division Terminal is a panel you deploy into a channel. Members use it to join and leave divisions on their own — no admin needed after setup.

When a member clicks **Division Selection**, they'll see buttons for each available division:
- **Green** = join
- **Red** = leave

Changes are staged and nothing happens until they click **Submit**. Once submitted, their roles update instantly.

If a member is in 2 or more divisions, a dropdown appears letting them choose which one is their **Primary Division** (shown with a ★). If the server allows more than one division, the Join button will grey out once they've hit the limit.

---

### Primary and Secondary Divisions

- **Primary** — A member's main division. They receive the primary member role, and optionally a default rank role if the admin has configured one.
- **Secondary** — Any additional divisions. They receive a secondary member role instead.

Members can change their primary at any time using the dropdown in the terminal. If a member leaves their primary division, the bot will automatically promote one of their remaining divisions to primary.

---

### Welcome Messages

When a member joins a division for the first time, a welcome message can be sent to a designated channel. The message can include:
- The division name and logo
- An optional banner image
- A custom message (use `{member}` to automatically ping the new member)
- A sign-off with the leader's name

Welcome messages are configured per division through the Division Wizard.

---

### /lookup

Look up division info for any member or division.

- `/lookup member:@someone` — See which divisions they're in and which is their primary (★)
- `/lookup division:name` — See a list of all primary and secondary members in that division

---

### /division wizard (Admin)

The wizard is the admin control panel for everything division-related. Open it with `/division wizard`.

<br>

**Divisions**
- **Create** — Set a name, whether it's joinable from the terminal, an accent color, and a logo. Then assign the leader role, primary member role, and optionally a secondary member role.
- **Edit** — Change any of the above for an existing division.
- **Delete** — Permanently removes the division and all member data for it. Requires typing `CONFIRM DELETE` to confirm.

<br>

**Welcome Messages**
- Set up, edit, or remove a welcome message for any division.
- Configure the destination channel, leader name, message text, and an optional image.

<br>

**Terminal Config**
- **Terminal Image** — Optional banner shown at the top of the terminal
- **Terminal Text** — Optional text shown below the image
- **Max Divisions** — How many divisions a member can be in at once (1–10, default is 1)
- **Default Rank Role** — An optional role automatically given when a member joins their first division. Different from a division role.
