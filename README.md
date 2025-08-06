# Nanoagent OS

**The operating system for drop-in, language-agnostic micro-agents.**

---

## 🚀 What is Nanoagent OS?

Nanoagent OS is a new open standard for **running, orchestrating, and composing tiny, manifest-driven agents**—no matter what language they’re written in.

* **Plug-and-play:** Drop any agent folder (with a manifest) into `/agents/`—Nanoagent OS will auto-discover and run it.
* **Language-agnostic:** Python, Node.js, Go, Rust, Bash… if it can run from the shell, it can be a Nanoagent.
* **Manifest-first:** Every agent describes itself in a simple `manifest.json`—no global config or registry required.
* **Ultra-lightweight & local-first:** Designed for speed, privacy, and maximum hackability—runs on your laptop, server, or even embedded device.

---

## ✨ Why Nanoagent OS?

* **Modular:** Build your workflow from small, focused agents. Compose them like UNIX pipes—only smarter.
* **Extensible:** Add new capabilities via agents, not plugins or containers.
* **Transparent:** Audit everything. Every agent’s code and manifest are visible, auditable, and open.
* **Cross-platform:** Nanoagent OS is built to run anywhere.

---

## 🏗️ How does it work?

1. **Clone or download this repo.**
2. Drop agent folders (with `manifest.json` and code) into the `/agents/` directory.
3. Start Nanoagent OS:

   ```bash
   nanoagent run muse
   nanoagent run haiku
   nanoagent list
   ```
4. Nanoagent OS discovers all agents, registers them, and can launch, pipe, and orchestrate them on demand.

---

## 📦 Example Usage

* **List all agents:**

  ```bash
  nanoagent list
  ```
* **Run an agent:**

  ```bash
  nanoagent run muse
  ```
* **Chain agents (coming soon):**

  ```bash
  nanoagent run muse | nanoagent run haiku
  ```

---

## 🧬 Agent Structure

Each agent is a folder in `/agents/`:

```
agents/
  muse/
    manifest.json
    agent.py
  haiku/
    manifest.json
    agent.py
```

**Sample `manifest.json`:**

```json
{
  "name": "haiku",
  "description": "Prints a random haiku.",
  "entry": "python agent.py",
  "language": "python",
  "version": "1.0.0"
}
```

---

## 📖 Documentation

* See [nanoagent-examples](https://github.com/natha-nguyen/nanoagent-examples) for ready-to-use agent templates.
* Full protocol and API docs coming soon in the `/docs/` folder.

---

## 🛡️ License

Nanoagent OS is released under the [MIT License](LICENSE).

---

## 👥 Contributing

* Suggest features or open issues
* Submit PRs for core improvements, agent orchestration, or new runtime support
* Share your custom agents in [nanoagent-examples](https://github.com/natha-nguyen/nanoagent-examples)

---

## 💡 About

**Nanoagent OS** is built for developers, hackers, and anyone who wants local-first, composable, privacy-respecting automation and AI—without the bloat.

---

> **Nanoagent OS:** Tiny code. Massive potential.

---

*Questions, feedback, or want to help shape the OS? Open an issue or join the discussion!*

---

Let me know if you want a setup section, architecture diagram, or a "getting started" video blurb!
