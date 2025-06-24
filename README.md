# JCB! Repositories

### What Are JCB Repositories?
JCB Repositories define where Joomla Component Builder (JCB) pushes or pulls content from  
during INIT, RESET, and PUSH operations.

They act as the Git configuration layer for managing remote syncing of the following entity types:
- 🧩 Snippets
- ⚡ Super Powers
- 🧬 Field Types
- 🔧 Joomla Powers
- 📦 JCB Packages

Each repository configuration defines how and where content is versioned - using GitHub, Gitea, or similar Git platforms.

---
### What Do Repositories Do?
A JCB Repository specifies:

- Which Git platform (e.g., GitHub or Gitea)
- Which organization/repo to use
- What branches to read from and write to
- How authentication should be handled (token, user, URL)
- Whether to use **Global Config** credentials or **Override** credentials locally
- Author name/email for Git commits

Each repository becomes a "target" used by JCB to push and pull data between your local builder and remote Git Repo.

Repositories themselves do not contain the data - they provide the link for transferring it.

---
### Access & Authentication
You can define two authentication modes:

- `Global`: Pull credentials from the global configuration of your JCB Component.
- `Override`: Manually provide your own Git credentials within this repository setup.

This provides fine-grained control for contributors, CI/CD automation, or organization-level collaboration.

Depending on the selected Git type:
- GitHub requires token, organization, and repo
- Gitea requires base URL, token, and organization

---
### Repository Targets
Each Repository can be assigned as the sync target for:

- Snippets
- Super Powers
- Field Types
- Joomla Powers
- JCB Packages

When INIT or RESET is triggered in those respective areas, JCB uses the matching repository settings to:
- Clone content from the repository into JCB
- Push updated content from JCB into Git

Multiple repositories can exist for different content types or development environments.

> Repositories define where things go — they are the communication bridge between your structured data in JCB and your remote Git Repositories.

### Index of JCB Repositories


 - **Gitea (codeberg - mirror)** | [Details](src/cb800a2c-4bf7-41c8-9360-cfe9d54cdf2b) | [Settings](src/cb800a2c-4bf7-41c8-9360-cfe9d54cdf2b/item.json)
 - **Joomla Field Types (codeberg - mirror)** | [Details](src/bf4a1d77-e3a4-4aa8-a07f-2b01872bf7e9) | [Settings](src/bf4a1d77-e3a4-4aa8-a07f-2b01872bf7e9/item.json)
 - **Joomla Powers (codeberg - mirror)** | [Details](src/8ac595d4-0b1d-4877-ba3e-2b815c1c7e3c) | [Settings](src/8ac595d4-0b1d-4877-ba3e-2b815c1c7e3c/item.json)
 - **Openai (codeberg - mirror)** | [Details](src/c625381a-7795-4b9f-8b4e-997c9291e3fc) | [Settings](src/c625381a-7795-4b9f-8b4e-997c9291e3fc/item.json)
 - **PHP Seclib (codeberg - mirror)** | [Details](src/64a84f86-391e-4e4b-be99-b2c7c41a6005) | [Settings](src/64a84f86-391e-4e4b-be99-b2c7c41a6005/item.json)
 - **Packages (codeberg - mirror)** | [Details](src/11298fc6-11a4-4075-bdcb-622ef4f3054d) | [Settings](src/11298fc6-11a4-4075-bdcb-622ef4f3054d/item.json)
 - **Packages (github - mirror)** | [Details](src/562624ab-48bf-4979-9a14-6b10cf3635de) | [Settings](src/562624ab-48bf-4979-9a14-6b10cf3635de/item.json)
 - **Repositories (codeberg - mirror)** | [Details](src/a8701724-b77c-4e5a-9efc-61701341e8e5) | [Settings](src/a8701724-b77c-4e5a-9efc-61701341e8e5/item.json)
 - **Repositories (github - mirror)** | [Details](src/8f156882-f299-4be2-ad13-fdb2c40bb207) | [Settings](src/8f156882-f299-4be2-ad13-fdb2c40bb207/item.json)
 - **Snippets (codeberg - mirror)** | [Details](src/70a9b44b-0802-4b94-9132-e5f360d0215e) | [Settings](src/70a9b44b-0802-4b94-9132-e5f360d0215e/item.json)
 - **Snippets (github - mirror)** | [Details](src/70e85588-bc28-4459-9b29-858f68faae8f) | [Settings](src/70e85588-bc28-4459-9b29-858f68faae8f/item.json)
 - **Super Powers (codeberg - mirror)** | [Details](src/8213b3a3-8618-4b29-92b3-15c9f26f019c) | [Settings](src/8213b3a3-8618-4b29-92b3-15c9f26f019c/item.json)

### All used in [Joomla Component Builder](https://www.joomlacomponentbuilder.com) - [Source](https://git.vdm.dev/joomla/Component-Builder) - [Mirror](https://github.com/vdm-io/Joomla-Component-Builder) - [Download](https://git.vdm.dev/joomla/pkg-component-builder/releases)

---
[![Joomla Volunteer Portal](https://img.shields.io/badge/-Joomla-gold?logo=joomla)](https://volunteers.joomla.org/joomlers/1396-llewellyn-van-der-merwe "Join Llewellyn on the Joomla Volunteer Portal: Shaping the Future Together!") [![Octoleo](https://img.shields.io/badge/-Octoleo-black?logo=linux)](https://git.vdm.dev/octoleo "--quiet") [![Llewellyn](https://img.shields.io/badge/-Llewellyn-ffffff?logo=gitea)](https://git.vdm.dev/Llewellyn "Collaborate and Innovate with Llewellyn on Git: Building a Better Code Future!") [![Telegram](https://img.shields.io/badge/-Telegram-blue?logo=telegram)](https://t.me/Joomla_component_builder "Join Llewellyn and the Community on Telegram: Building Joomla Components Together!") [![Mastodon](https://img.shields.io/badge/-Mastodon-9e9eec?logo=mastodon)](https://joomla.social/@llewellyn "Connect and Engage with Llewellyn on Joomla Social: Empowering Communities, One Post at a Time!") [![X (Twitter)](https://img.shields.io/badge/-X-black?logo=x)](https://x.com/llewellynvdm "Join the Conversation with Llewellyn on X: Where Ideas Take Flight!") [![GitHub](https://img.shields.io/badge/-GitHub-181717?logo=github)](https://github.com/Llewellynvdm "Build, Innovate, and Thrive with Llewellyn on GitHub: Turning Ideas into Impact!") [![YouTube](https://img.shields.io/badge/-YouTube-ff0000?logo=youtube)](https://www.youtube.com/@OctoYou "Explore, Learn, and Create with Llewellyn on YouTube: Your Gateway to Inspiration!") [![n8n](https://img.shields.io/badge/-n8n-black?logo=n8n)](https://n8n.io/creators/octoleo "Effortless Automation and Impactful Workflows with Llewellyn on n8n!") [![Docker Hub](https://img.shields.io/badge/-Docker-grey?logo=docker)](https://hub.docker.com/u/llewellyn "Llewellyn on Docker: Containerize Your Creativity!") [![Open Collective](https://img.shields.io/badge/-Donate-green?logo=opencollective)](https://opencollective.com/joomla-component-builder "Donate towards JCB: Help Llewellyn financially so he can continue developing this great tool!") [![GPG Key](https://img.shields.io/badge/-GPG-blue?logo=gnupg)](https://git.vdm.dev/Llewellyn/gpg "Unlock Trust and Security with Llewellyn's GPG Key: Your Gateway to Verified Connections!")