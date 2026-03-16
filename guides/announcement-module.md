# Announcement Module

The Announcement Module lets you create reusable announcement presets for your divisions or units. Each preset has its own branding — headers, colors, footer, and ping roles — so posting a briefing only takes a few seconds.

---

### Setting Up Presets — /announcement wizard (Admin)

Before anyone can post announcements, an admin needs to create at least one preset.

Each preset includes:
- **Display Name** — The name of the division or unit this preset belongs to (e.g., "OSI Strike Team")
- **Accent Color** — Optional hex color to theme the announcement
- **Footer Image** — A static image shown at the bottom of every announcement using this preset
- **Headers** — Up to 5 header styles, each with a label (e.g., "New Briefing") and a banner image. The sender picks one when posting.
- **Ping Roles** — Up to 5 roles to mention when the announcement is sent, or an @everyone toggle

Presets can be edited or deleted at any time from the wizard.

---

### Posting an Announcement — /announcement send

Requires **Mention Everyone** permission.

1. Run `/announcement send`, pick a preset, and choose whether to ping roles
2. A form opens with:
   - **Title** (required)
   - **Content** (optional, markdown supported)
   - **Header Style** (if the preset has multiple headers, pick one)
   - **Custom Image** (optional upload, appears between the header and title)
3. Submit — the announcement posts to the current channel with your header image, content, role pings, footer image, and author credit

<img width="530" height="653" alt="image" src="https://github.com/user-attachments/assets/7085e397-499a-4c6b-b539-c2d3da0a2bcf" />
