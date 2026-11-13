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


 - **Gitea (codefloe - mirror)** | [Details](src/cb800a2c-4bf7-41c8-9360-cfe9d54cdf2b) | [Settings](src/cb800a2c-4bf7-41c8-9360-cfe9d54cdf2b/item.json)
 - **Gitea (github)** | [Details](src/c743c2b1-354a-4d21-acd6-5e14a13065ce) | [Settings](src/c743c2b1-354a-4d21-acd6-5e14a13065ce/item.json)
 - **Joomla Field Types (codefloe - mirror)** | [Details](src/bf4a1d77-e3a4-4aa8-a07f-2b01872bf7e9) | [Settings](src/bf4a1d77-e3a4-4aa8-a07f-2b01872bf7e9/item.json)
 - **Joomla Field Types (github)** | [Details](src/e10a2193-aa8b-4414-a57e-fa4bbedbf063) | [Settings](src/e10a2193-aa8b-4414-a57e-fa4bbedbf063/item.json)
 - **Joomla Packages (codefloe - mirror)** | [Details](src/b07f99f2-30be-4b29-a158-0fb98692cf89) | [Settings](src/b07f99f2-30be-4b29-a158-0fb98692cf89/item.json)
 - **Joomla Packages (github)** | [Details](src/ca50a886-0fd9-4fd8-803f-ba2cd9f43f55) | [Settings](src/ca50a886-0fd9-4fd8-803f-ba2cd9f43f55/item.json)
 - **Joomla Powers (codefloe - mirror)** | [Details](src/8ac595d4-0b1d-4877-ba3e-2b815c1c7e3c) | [Settings](src/8ac595d4-0b1d-4877-ba3e-2b815c1c7e3c/item.json)
 - **Joomla Powers (github)** | [Details](src/4088b8b0-e92c-4f59-b480-7da328e3d828) | [Settings](src/4088b8b0-e92c-4f59-b480-7da328e3d828/item.json)
 - **Minify (codefloe - mirror)** | [Details](src/1ea3f09b-b65c-4fc2-b850-7996ab81bf83) | [Settings](src/1ea3f09b-b65c-4fc2-b850-7996ab81bf83/item.json)
 - **Minify (github)** | [Details](src/8cacacde-03db-46e9-bfa2-84985d26e666) | [Settings](src/8cacacde-03db-46e9-bfa2-84985d26e666/item.json)
 - **Openai (codefloe - mirror)** | [Details](src/c625381a-7795-4b9f-8b4e-997c9291e3fc) | [Settings](src/c625381a-7795-4b9f-8b4e-997c9291e3fc/item.json)
 - **Openai (github)** | [Details](src/da402346-a3cb-49f1-9eae-b11026f48eaa) | [Settings](src/da402346-a3cb-49f1-9eae-b11026f48eaa/item.json)
 - **PHP Seclib (codefloe - mirror)** | [Details](src/64a84f86-391e-4e4b-be99-b2c7c41a6005) | [Settings](src/64a84f86-391e-4e4b-be99-b2c7c41a6005/item.json)
 - **PHP Seclib (github)** | [Details](src/8b4a4649-cffb-4cda-a695-b8162cbe8f99) | [Settings](src/8b4a4649-cffb-4cda-a695-b8162cbe8f99/item.json)
 - **PSR (codefloe - mirror)** | [Details](src/93af374c-f48f-47b7-8be1-870e814f3001) | [Settings](src/93af374c-f48f-47b7-8be1-870e814f3001/item.json)
 - **PSR (github)** | [Details](src/5ff9f972-960b-46ba-a0e8-ff737b13007c) | [Settings](src/5ff9f972-960b-46ba-a0e8-ff737b13007c/item.json)
 - **Packages (codefloe - mirror)** | [Details](src/11298fc6-11a4-4075-bdcb-622ef4f3054d) | [Settings](src/11298fc6-11a4-4075-bdcb-622ef4f3054d/item.json)
 - **Packages (github)** | [Details](src/562624ab-48bf-4979-9a14-6b10cf3635de) | [Settings](src/562624ab-48bf-4979-9a14-6b10cf3635de/item.json)
 - **Repositories (codefloe - mirror)** | [Details](src/a8701724-b77c-4e5a-9efc-61701341e8e5) | [Settings](src/a8701724-b77c-4e5a-9efc-61701341e8e5/item.json)
 - **Repositories (github)** | [Details](src/8f156882-f299-4be2-ad13-fdb2c40bb207) | [Settings](src/8f156882-f299-4be2-ad13-fdb2c40bb207/item.json)
 - **Search (codefloe - mirror)** | [Details](src/7d7b5688-6ac9-422a-8fba-b3ce7ece6ac4) | [Settings](src/7d7b5688-6ac9-422a-8fba-b3ce7ece6ac4/item.json)
 - **Search (github)** | [Details](src/dcc988f9-88b4-4acb-9a07-9ace866414ca) | [Settings](src/dcc988f9-88b4-4acb-9a07-9ace866414ca/item.json)
 - **Snippets (codefloe - mirror)** | [Details](src/70a9b44b-0802-4b94-9132-e5f360d0215e) | [Settings](src/70a9b44b-0802-4b94-9132-e5f360d0215e/item.json)
 - **Snippets (github)** | [Details](src/70e85588-bc28-4459-9b29-858f68faae8f) | [Settings](src/70e85588-bc28-4459-9b29-858f68faae8f/item.json)
 - **Super Powers (codefloe - mirror)** | [Details](src/8213b3a3-8618-4b29-92b3-15c9f26f019c) | [Settings](src/8213b3a3-8618-4b29-92b3-15c9f26f019c/item.json)
 - **Super Powers (github)** | [Details](src/183fac1f-bfee-4993-8e21-4dbdde4d7e3f) | [Settings](src/183fac1f-bfee-4993-8e21-4dbdde4d7e3f/item.json)

### All used in [Joomla Component Builder](https://www.joomlacomponentbuilder.com) - [Source](https://git.vdm.dev/joomla/Component-Builder) - [Mirror](https://github.com/vdm-io/Joomla-Component-Builder) - [Download](https://git.vdm.dev/joomla/pkg-component-builder/releases)

---
[![Joomla Volunteer Portal](https://img.shields.io/badge/-Joomla-gold?logo=joomla)](https://volunteers.joomla.org/joomlers/1396-llewellyn-van-der-merwe "Join Llewellyn on the Joomla Volunteer Portal: Shaping the Future Together!") [![GitHub](https://img.shields.io/badge/-Git-181717?logo=git)](https://github.com/joomengine "Build premium Joomla extensions with JoomEngine on GitHub: Help us raise Joomla extension standards!") [![Octoleo](https://img.shields.io/badge/-Octoleo-black?logo=linux)](https://git.vdm.dev/octoleo "--quiet") [![Llewellyn](https://img.shields.io/badge/-Llewellyn-ffffff?logo=gitea)](https://git.vdm.dev/Llewellyn "Collaborate and Innovate with Llewellyn on Git: Building a Better Code Future!") [![Telegram](https://img.shields.io/badge/-Telegram-blue?logo=telegram)](https://t.me/Joomla_component_builder "Join Llewellyn and the Community on Telegram: Building Joomla Components Together!") [![Mastodon](https://img.shields.io/badge/-Mastodon-9e9eec?logo=mastodon)](https://joomla.social/@llewellyn "Connect and Engage with Llewellyn on Joomla Social: Empowering Communities, One Post at a Time!") [![X (Twitter)](https://img.shields.io/badge/-X-black?logo=x)](https://x.com/llewellynvdm "Join the Conversation with Llewellyn on X: Where Ideas Take Flight!") [![GitHub](https://img.shields.io/badge/-GitHub-181717?logo=github)](https://github.com/Llewellynvdm "Build, Innovate, and Thrive with Llewellyn on GitHub: Turning Ideas into Impact!") [![YouTube](https://img.shields.io/badge/-YouTube-ff0000?logo=youtube)](https://www.youtube.com/@OctoYou "Explore, Learn, and Create with Llewellyn on YouTube: Your Gateway to Inspiration!") [![n8n](https://img.shields.io/badge/-n8n-black?logo=n8n)](https://n8n.io/creators/octoleo "Effortless Automation and Impactful Workflows with Llewellyn on n8n!") [![Docker Hub](https://img.shields.io/badge/-Docker-grey?logo=docker)](https://hub.docker.com/r/octoleo/joomengine "JoomEngine on Docker: Containerize Your Creativity!") [![Open Collective](https://img.shields.io/badge/-Donate-green?logo=opencollective)](https://opencollective.com/joomla-component-builder "Donate towards JCB: Help Llewellyn financially so he can continue developing this great tool!") [![GPG Key](https://img.shields.io/badge/-GPG-blue?logo=gnupg)](https://git.vdm.dev/Llewellyn/gpg "Unlock Trust and Security with Llewellyn's GPG Key: Your Gateway to Verified Connections!")