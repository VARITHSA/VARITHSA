<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/banner-dark.svg">
  <img alt="Srivathsa B S — Software Engineer · HPC & Heterogeneous Computing · Quantum" src="assets/banner-light.svg" width="100%">
</picture>

<a href="https://github.com/VARITHSA">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=500&size=17&duration=2600&pause=900&color=2986FF&center=true&vCenter=true&width=640&lines=Deciding+when+code+should+run+on+the+CPU+vs+the+GPU;Writing+quantum+circuits+with+Qiskit;Shipping+client+products+at+LYPTRON;Open+to+SDE+roles+%E2%80%94+say+hi+below" alt="What I'm working on">
</a>

<br>

<a href="https://linkedin.com/in/srivathsa-b-s-185a03237"><img src="https://img.shields.io/badge/LinkedIn-0B0B0C?style=for-the-badge&logo=linkedin&logoColor=2986FF" alt="LinkedIn"></a>
<a href="mailto:bssrivathsa2003@gmail.com"><img src="https://img.shields.io/badge/Email-0B0B0C?style=for-the-badge&logo=gmail&logoColor=FDAE2B" alt="Email"></a>
<a href="https://medium.com/@bssrivathsa2003"><img src="https://img.shields.io/badge/Medium-0B0B0C?style=for-the-badge&logo=medium&logoColor=white" alt="Medium"></a>
<a href="https://lyptron.com"><img src="https://img.shields.io/badge/LYPTRON-0B0B0C?style=for-the-badge&logo=data:image/svg%2bxml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI+PGNpcmNsZSBjeD0iMTIiIGN5PSIxMiIgcj0iOCIgZmlsbD0iI0ZEQUUyQiIvPjwvc3ZnPg==" alt="LYPTRON"></a>

</div>

---

### `$ cat about.md`

I'm an M.Tech CSE student at **Manipal Institute of Technology, Bengaluru**, working where software meets hardware: figuring out *where* a workload should run, CPU or GPU, and *how* to run it there fast. On the side I'm learning quantum computing the hands-on way, with Qiskit.

I also run **[LYPTRON](https://lyptron.com)**, a design and technology studio, where I've shipped production apps for real clients, from a desktop music-notation editor to a Flutter field-operations app.

<table>
<tr>
<td width="33%" valign="top">

**🔭 Researching**<br>
Intelligent CPU–GPU execution strategy selection for ML workloads

</td>
<td width="33%" valign="top">

**⚛️ Learning**<br>
Quantum algorithms (Bernstein–Vazirani, oracles, circuit design)

</td>
<td width="33%" valign="top">

**🛠️ Building**<br>
Client products and agentic workflows at LYPTRON

</td>
</tr>
</table>

---

### `$ ls ~/work` <sub>· click a project to open it</sub>

<details>
<summary><b>⚡ AutoHetero</b> · a zero-config runtime that dispatches Python workloads to CPU or GPU</summary>
<br>

A self-adaptive runtime layer that sits under ordinary Python code, profiles each workload, and dispatches it to the CPU or the GPU, so developers get heterogeneous execution without rewriting anything.

```mermaid
flowchart LR
    A[Python call] --> B{Profiler}
    B -->|features: size, ops, memory| C[Dispatch policy]
    C -->|small / branchy| D[CPU]
    C -->|large / data-parallel| E[GPU]
    D --> F[Result]
    E --> F
    F -.->|runtime feedback| C
```

`Python` `CUDA` `profiling` `HPC`
</details>

<details>
<summary><b>🧠 Intelligent Execution Strategy Selection</b> · M.Tech research: choose device and GPU concurrency for ML models</summary>
<br>

My M.Tech HPC project. Given an ML workload, it picks the execution strategy: which device it runs on and how much GPU concurrency to use. The aim is a decider students can use before they run their models. It builds on what AutoHetero showed in practice.

`Python` `CUDA` `ML systems` `research`
</details>

<details>
<summary><b>⚛️ ClusterDoc</b> · finds failing servers in a cluster with the Bernstein–Vazirani algorithm</summary>
<br>

Each server's health becomes one bit of a hidden string. A parity health-check oracle encodes the cluster, and one Bernstein–Vazirani query recovers which servers are failing. A classical approach needs *n* checks for the same answer.

```mermaid
flowchart LR
    A["|0⟩ⁿ |1⟩"] --> B["H⊗ⁿ"]
    B --> C["U_f<br/>parity health-check oracle"]
    C --> D["H⊗ⁿ"]
    D --> E["Measure → failing-server bitmap"]
```

`Qiskit` `Python` `quantum algorithms`
</details>

<details>
<summary><b>🛰️ EGAQ</b> · entropy-guided adaptive quadtree for multi-resolution satellite image retrieval</summary>
<br>

Splits satellite imagery into a quadtree that subdivides only where image entropy is high, so detailed regions get fine tiles and flat regions stay coarse. Retrieval works across resolutions without indexing every pixel at full detail.

`Python` `computer vision` `spatial indexing`
</details>

<details>
<summary><b>💼 Client work at LYPTRON</b> · production apps, end to end</summary>
<br>

- **Music-notation desktop app**: offline score editor with playback, tala-aware layout, and PDF export, shipped as a Windows installer
- **Field-operations app** (Flutter): attendance, materials and reporting for construction sites, designed for non-technical users
- Client websites and landing pages, from design system to deployment

Code is private under client agreements; happy to walk through the architecture.
</details>

---

### `$ stack --list`

<table>
<tr><td><b>Languages</b></td><td><img src="https://skillicons.dev/icons?i=python,cpp,c,java,dart&theme=dark" height="40" alt="Python, C++, C, Java, Dart"></td></tr>
<tr><td><b>HPC &amp; Quantum</b></td><td>
<img src="https://img.shields.io/badge/CUDA-0B0B0C?style=flat-square&logo=nvidia&logoColor=76B900" alt="CUDA">
<img src="https://img.shields.io/badge/MPI-0B0B0C?style=flat-square&logoColor=white" alt="MPI">
<img src="https://img.shields.io/badge/OpenMP-0B0B0C?style=flat-square" alt="OpenMP">
<img src="https://img.shields.io/badge/Qiskit-0B0B0C?style=flat-square&logo=qiskit&logoColor=6929C4" alt="Qiskit">
</td></tr>
<tr><td><b>System Design</b></td><td>
<img src="https://img.shields.io/badge/Low--Level_Design-0B0B0C?style=flat-square" alt="Low-Level Design">
<img src="https://img.shields.io/badge/System_Flow_Architecture-0B0B0C?style=flat-square" alt="System Flow Architecture">
<img src="https://img.shields.io/badge/Design_Patterns-0B0B0C?style=flat-square" alt="Design Patterns">
</td></tr>
<tr><td><b>Agentic AI &amp; Automation</b></td><td>
<img src="https://img.shields.io/badge/Agentic_AI-0B0B0C?style=flat-square" alt="Agentic AI">
<img src="https://img.shields.io/badge/MCP-0B0B0C?style=flat-square&logo=modelcontextprotocol&logoColor=white" alt="MCP">
<img src="https://img.shields.io/badge/Claude-0B0B0C?style=flat-square&logo=claude&logoColor=D97757" alt="Claude">
<img src="https://img.shields.io/badge/Workflow_Automation-0B0B0C?style=flat-square" alt="Workflow Automation">
</td></tr>
<tr><td><b>Backend &amp; Apps</b></td><td><img src="https://skillicons.dev/icons?i=fastapi,flutter,firebase&theme=dark" height="40" alt="FastAPI, Flutter, Firebase"></td></tr>
<tr><td><b>Tools</b></td><td><img src="https://skillicons.dev/icons?i=git,linux,docker,vscode,figma&theme=dark" height="40" alt="Git, Linux, Docker, VS Code, Figma"></td></tr>
</table>

---

### `$ git log --graph`

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/VARITHSA/VARITHSA/output/snake-dark.svg">
  <img alt="Contribution graph being eaten by a snake" src="https://raw.githubusercontent.com/VARITHSA/VARITHSA/output/snake.svg" width="100%">
</picture>

---

### `$ ./visitor.sh` <sub>· pick your path</sub>

<details>
<summary>🧑‍💼 <b>I'm hiring</b></summary>
<br>

I'm looking for **SDE roles** where systems thinking matters: backend, infrastructure, performance, ML systems, or agentic AI. I bring:

- Low-level performance work (CUDA, MPI, OpenMP) **and** end-to-end product delivery
- Experience owning projects with real clients, from scoping and contracts to design and shipping
- Steady DSA practice

📫 [Email me](mailto:bssrivathsa2003@gmail.com) or [connect on LinkedIn](https://linkedin.com/in/srivathsa-b-s-185a03237).
</details>

<details>
<summary>🔬 <b>I want to collaborate on research</b></summary>
<br>

I'm interested in heterogeneous scheduling, GPU performance modelling, energy-aware execution, and practical quantum algorithms. If you're working on any of these, [open a discussion](https://github.com/VARITHSA/VARITHSA/issues/new?title=Research%20collab%3A%20&body=Hi%20Srivathsa%2C%20I%27m%20working%20on%20...) and tell me about it.
</details>

<details>
<summary>🏢 <b>I need something built</b></summary>
<br>

That's what [LYPTRON](https://lyptron.com) does: apps, websites, and design systems, built with care.<br>
*Building trust, one partnership at a time.*
</details>

<br>

<div align="center">

<a href="https://github.com/VARITHSA/VARITHSA/issues/new?title=%F0%9F%91%8B%20Hi%20from%20&body=Name%3A%0AWhere%20I%20found%20you%3A%0AMessage%3A%0A"><img src="https://img.shields.io/badge/👋_Sign_the_guestbook-2986FF?style=for-the-badge" alt="Sign the guestbook"></a>
<a href="https://github.com/VARITHSA/VARITHSA/issues/new?title=%E2%9D%93%20Question%3A%20&body=Ask%20me%20anything%20about%20HPC%2C%20quantum%2C%20Flutter%2C%20or%20running%20a%20studio%20as%20a%20student."><img src="https://img.shields.io/badge/❓_Ask_me_anything-0B0B0C?style=for-the-badge" alt="Ask me anything"></a>

<sub>Both buttons open a pre-filled GitHub issue. I read every one.</sub>

</div>
