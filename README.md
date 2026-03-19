# <img src="favicon.png" alt="logo" width="25" height="25"/> CtrlV
### Copy & Paste Blurbs fast!
 
CtrlV is a free, single-file browser tool that lets you store and instantly copy frequently used messages, scripts, and templates — built for anyone who types the same things over and over.
 
[![Live Demo](https://img.shields.io/badge/Live%20Demo-GitHub%20Pages-blue?style=flat-square)](https://404neil.github.io/CtrlV/)
![GitHub Repo stars](https://img.shields.io/github/stars/404neil/CtrlV?style=flat-square)
![GitHub forks](https://img.shields.io/github/forks/404neil/CtrlV?style=flat-square)
![GitHub License](https://img.shields.io/github/license/404neil/CtrlV?style=flat-square)


 
---
 
## Why This Project Exists 📋
 
While working as a customer support chat executive, I noticed that many customer questions were repeated throughout the day. Rewriting the same responses — or scrolling through a document to find the right one — slowed down response time and reduced efficiency during active conversations.
 
To solve this, I built CtrlV: a simple HTML page that acts as a quick-response dashboard. Store your most-used scripts, click Copy, paste into chat. That's it.
 
What started as a personal tool has grown into something much bigger — with profiles, a Knowledge Hub, multilingual support, keyboard shortcuts, team sharing, and more — while staying true to the original idea: **no install, no account, no friction, just open it and go.**
 
---
 
## How It Works ⚙️

 <img src="/Screenshots/copy.gif"/>

1. Open CtrlV in a browser tab alongside your CRM or chat window
2. Organise your scripts into tabs and sections
3. Click the **📋 Copy** button next to any script
4. Paste directly into your customer chat
 
That's the core of it. Everything else is built around making that workflow faster and more organised.
 
---
 
## Key Features 💪
 
**Scripts & Organisation**
- One-click copy for any blurb
- Tabs and collapsible sections to organise scripts by category, topic, or workflow
- Colour coding for tabs and sections — find what you need at a glance
- Drag and drop to reorder tabs, sections, and blurbs
- Labels for each blurb so you can scan quickly
- Placeholder detection — blurbs with `{customer_name}` style fields turn the copy button red and warn you to fill them in before sending
 
**Profiles**
- Multiple profiles for different roles or clients (e.g. 🎧 Customer Service, 🛠 Technical Support)
- Each profile has its own tabs, scripts, colours, shortcuts, language, dark mode, and Knowledge Hub
- Switch profiles instantly from the footer button
- Export and import profiles as `.json` to share with your team
 
**Knowledge Hub**
- A built-in reference panel for SOPs, FAQs, and product guides — right next to your scripts
- Supports Markdown: headings, bold, italic, lists, blockquotes, links, code blocks
- Paste a YouTube or Vimeo URL on its own line to embed a video player
- Paste an image URL on its own line to embed an image
- Live search across all content
 
**Keyboard Shortcuts**
- Assign any `Ctrl`, `Alt`, or `Shift` + key combo to any blurb
- Press the combo anywhere on the CtrlV page to copy instantly
- Works with Bluetooth and USB keyboards on mobile too
 
**Global Search**
- Press `Ctrl+K` to search across every blurb in every tab in real time
 
**Languages**
- Built-in: English, Español, Français, Deutsch, हिन्दी, বাংলা
- Export any language file, translate it, import it back — add any language you need
- Language setting saved per profile
 
**Everything else**
- Usage counter — see how many times each blurb has been copied; export as CSV
- Dark mode
- Mobile-friendly layout with collapsible sidebar
- Works completely offline
- Works on locked-down corporate machines — if there's a browser, CtrlV works
- White-label support — customise the footer text, link, and favicon for your organisation
- Save Location — point CtrlV at any folder and it auto-saves your scripts there
 
---
 
## Team Sync 🤝
 
CtrlV has no sync server. This is a deliberate choice — your data stays on your devices, and you never depend on anyone else's infrastructure.
 
Instead, CtrlV uses the **KeepassXC model**: it reads and writes a plain `ctrlv_blurbs.json` file from a folder you choose. If that folder is synced by Dropbox, Google Drive, OneDrive, or a shared network drive — you get team sync for free, with no accounts and no backend involved.
 
**Quick setup:**
1. Manager points CtrlV at a shared Dropbox/Drive folder via **Settings → Save Location**
2. Each agent does the same — points their CtrlV at the same shared folder
3. When the manager updates scripts, agents go to **Settings → Import JSON** to load the latest version
 
The import step is intentional — in a customer service context, you want agents to consciously load an update rather than have scripts change silently mid-shift.
 
No shared drive? Just email the export file. It takes 10 seconds.
 
---
 
## Profiles Guide 👤
 
Profiles are useful if you handle multiple queues, multiple clients, or multiple brands in a single shift.
 
1. Click the emoji button in the footer (defaults to 👤)
2. Click **➕ New Profile**, pick an emoji, give it a name
3. Customise that profile's tabs, scripts, and settings independently
4. Switch between profiles instantly — everything changes, including language and Knowledge Hub content
 
Export a profile to share it with a colleague. Import a profile to load someone else's setup without overwriting your own.
 
---
 
## Knowledge Hub Guide 📚
 
The Knowledge Hub is a reference panel for things your team needs to *read*, not copy — SOPs, product guides, FAQs, escalation paths.
 
- Click **📚** in the footer to open it
- Edit content in **⚙️ Settings → Knowledge Hub** using Markdown
- Use the search bar to find anything instantly
- Each profile has its own Knowledge Hub content
 
Paste a YouTube or Vimeo link on its own line in the editor and it embeds as a video. Paste an image URL and it embeds as an image.
 
---
 
## Use Cases 😊
 
- Customer support chat agents
- Call centre teams
- Community moderators and social media managers
- Helpdesk and technical support teams
- Receptionists and admin staff
- Teachers giving written feedback
- Recruiters sending screening messages
- Anyone who types the same things every day
 
---
 
## Tech Stack 🧰
 
- HTML, CSS, JavaScript
- Zero dependencies
- Zero build tools
- One file
 
---
 
## Contributing 🙌
 
Contributions are very welcome.
 
**Adding a language:**
1. Go to **⚙️ Settings → Language → ⬆ Export Language File**
2. Translate the string values in the downloaded `.json` (leave the keys unchanged)
3. Add `"_name": "Your Language Name"` so it shows in the dropdown
4. Submit a pull request or open an issue and attach the file
 
**Reporting bugs:**
Open an issue with what happened, which browser you were using, and whether it was on the hosted version or a local file.
 
**Code contributions:**
CtrlV is a single `index.html` file — no build step, no node_modules. Open it in any text editor and you can see everything. Pull requests welcome.
 

---
 
## Roadmap 🛠️
 
Things that started as "future improvements" and are now done ✅ — and what's coming next:
 
- [x] Search through saved responses
- [x] Categorise responses with tabs and sections
- [x] Save responses in local storage
- [x] Keyboard shortcuts
- [x] Improved UI/UX
- [x] Template export/import
- [x] Dark mode
- [x] Mobile layout
- [x] Profiles
- [x] Knowledge Hub
- [x] Multilingual UI
- [x] Drag and drop reordering
- [x] Usage analytics
- [x] Team sharing
- [x] White-label support
- [ ] Chrome extension with inline auto-expansion
- [ ] Desktop app (Windows & Linux)
- [ ] Android app via GooglePlay Store
- [ ] More languages
 
---
 
## Project Status 🟢
 
Actively maintained. Started as a personal tool used in a real support workflow — now a full-featured productivity platform that still fits in a single HTML file.

---
 
## Support the Project ⭐
 
CtrlV is free forever. If it saves you time, you can help by starring the repo ⭐, sharing it with your team, or contributing a translation.
 
