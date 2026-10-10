<p align="center">
  <img src="https://raw.githubusercontent.com/pazalo/.github/main/assets/pazalo-logo.png" width="132" alt="Pazalo">
</p>

<h1 align="center">Pazalo</h1>

<p align="center">
  <em>The platform we build on — and the one we host for others.</em>
</p>

<p align="center">
  <a href="https://github.com/pazalo/cloud"><img src="https://img.shields.io/badge/cloud-control_plane-FFC24D?style=flat-square&logo=github&logoColor=black" alt="cloud"></a>
  <a href="https://github.com/pazalo/panel"><img src="https://img.shields.io/badge/panel-back_office-FFC24D?style=flat-square&logo=github&logoColor=black" alt="panel"></a>
  <a href="https://github.com/pazalo/storefront"><img src="https://img.shields.io/badge/storefront-site-F0522C?style=flat-square&logo=github&logoColor=white" alt="storefront"></a>
  <a href="https://github.com/pazalo/cli"><img src="https://img.shields.io/badge/cli-terminal-FFC24D?style=flat-square&logo=github&logoColor=black" alt="cli"></a>
  <a href="https://github.com/pazalo/docs"><img src="https://img.shields.io/badge/docs-reference-F0522C?style=flat-square&logo=github&logoColor=white" alt="docs"></a>
  <a href="https://github.com/pazalo/skills"><img src="https://img.shields.io/badge/skills-agent_skills-FFC24D?style=flat-square&logo=github&logoColor=black" alt="skills"></a>
</p>

---

**Pazalo is a website platform.** A site is the unit of everything here — it can
sell, publish, take bookings or simply exist — and what a site *can* do is decided
by the capabilities installed on it, not by a template someone picked at signup.

## How it works

**Every site is two containers and one database.** The storefront is what people
see; the panel is where the site is run — including its commerce engine, which
lives inside it at `/api/graphql`.

**Sites cannot see each other.** Each one owns its database, and PostgreSQL
decides what it may touch. No permission means a refusal, never an empty page.

**The API is checked in.** The schema is generated from what a site actually
has, written to `schema.graphql`, and verified in CI. If an operation exists, the
file says so.

---

## The repositories

| | Repository | What it is |
| --- | --- | --- |
| ☁️ | **[cloud](https://github.com/pazalo/cloud)** | The **control plane.** Provisions and operates the fleet: one platform client, one isolation guard, one rollback-capable saga. |
| 🧭 | **[panel](https://github.com/pazalo/panel)** | The **back office**, one per site — and the site's engine inside it. 38 capabilities across 4 roles. |
| 🛍️ | **[storefront](https://github.com/pazalo/storefront)** | What the **visitor sees.** Fast, accessible, and in Romanian by design rather than by translation. |
| ⌨️ | **[cli](https://github.com/pazalo/cli)** | The **terminal client** the browser is not there for: deploys, logs, environments, releases. Zero dependencies. |
| 📚 | **[docs](https://github.com/pazalo/docs)** | The **reference material**, including eleven offline mirrors of the third-party docs we actually run. |
| 🧠 | **[skills](https://github.com/pazalo/skills)** | The **decisions** shared by every repository, installed into every agent that works on this workspace. |

---

<p align="center">
  <sub>Built and hosted by <b>Pazal Group SRL</b> · Romania · All rights reserved</sub>
</p>
