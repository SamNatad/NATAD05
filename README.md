<div align="center">

# Sam Natad

**`$ whoami` → 2026 BSIT graduate · aspiring software engineer · continuous learner**

```diff
- looking for: senior / experienced developer
+ looking for: junior developer, internship, or a patient mentor
```

[Projects](#projects) · [Skills](#skills) · [Journey](#continuous-learning) · [Contact](#contact)

</div>

---

## About

I learn by building. Three desktop apps in **Java** and **C#** for school, plus a
portfolio site written from scratch in **HTML** and **CSS** — no frameworks, no
templates.

<details>
<summary><b>The longer version — what I have and haven't done</b></summary>

My practical experience came from team projects. Our seven-person capstone,
**BuildHub**, was a desktop app for ordering PC parts. It taught me more than the
syllabus did: how to read other people's code, agree on scope, and handle the parts
of a project nobody hands you in a textbook.

Being straight about the gaps:

- I'm a **beginner-to-early-intermediate programmer**
- I have **not** worked in a professional engineering team
- I have **not** shipped software to real users
- I have **not** maintained a production codebase

What I do have is the habit of finishing projects, asking questions early, and
picking up whatever the next task requires.

</details>

## Skills

**Languages & version control** — used in a project I completed

<div align="center">

![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![C#](https://img.shields.io/badge/C%23-9B4F96?style=flat-square&logo=dotnet&logoColor=white)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-2965F1?style=flat-square&logo=css3&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05033?style=flat-square&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white)

</div>

**Tools I use**

<div align="center">

![Visual Studio](https://img.shields.io/badge/Visual_Studio-5C2D91?style=flat-square&logo=visualstudio&logoColor=white)
![VS Code](https://img.shields.io/badge/VS_Code-007ACC?style=flat-square&logo=visualstudiocode&logoColor=white)
![NetBeans](https://img.shields.io/badge/NetBeans-5382A1?style=flat-square&logo=apachenetbeans&logoColor=white)
![JDK](https://img.shields.io/badge/JDK_22-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![.NET](https://img.shields.io/badge/.NET_10-512BD4?style=flat-square&logo=dotnet&logoColor=white)
![Windows](https://img.shields.io/badge/Windows-0078D4?style=flat-square&logo=windows&logoColor=white)
![Figma](https://img.shields.io/badge/Figma-A259FF?style=flat-square&logo=figma&logoColor=white)
![Canva](https://img.shields.io/badge/Canva-00C4CC?style=flat-square&logo=canva&logoColor=white)
![Microsoft Office](https://img.shields.io/badge/Microsoft_Office-D83B01?style=flat-square&logo=microsoft&logoColor=white)

</div>

**Currently learning** — early stage, no shipped project yet

<div align="center">

![SQL](https://img.shields.io/badge/SQL-learning-dashed-4A9ED8?style=flat-square)
![JavaScript](https://img.shields.io/badge/JavaScript-learning-dashed-F7DF1E?style=flat-square&logo=javascript&logoColor=black)

</div>

| Area | Details |
|---|---|
| **IDEs & editors** | Visual Studio, Visual Studio Code, NetBeans 22 |
| **Runtimes & platform** | JDK 22, .NET 10, Windows |
| **Version control** | Git, GitHub |
| **Design** | Figma, Canva |
| **Productivity** | Microsoft Office |
| **Desktop UI** | Java Swing, Windows Forms, NetBeans GUI Designer |
| **Concepts** | OOP, event-driven programming, data structures, algorithms, role-based access control, web accessibility |
| **Frontend** | Semantic HTML5, CSS Grid, Flexbox, responsive design, theming, a11y basics |

## Projects

### `01` BuildHub — PC Parts Ordering System

**Java · Swing · NetBeans 22 / JDK 22 · academic capstone · team of 7**

Desktop app for browsing and ordering PC parts. Customers register, verify their
account, build a cart, and pay with change calculated live.

<details>
<summary><b>What I built</b> — 8 features</summary>

- Account sign-up with **OTP verification** and password reset
- Login screens for account, Gmail, and Facebook sign-in
- Catalogue: monitors, keyboards, RAM, motherboards, GPUs, cases, prebuilt systems
- Cart on a `JTable` with live quantity and price calculation
- Payment flow computing subtotal, total, and balance due
- Receipt generation with a printable order summary
- Profile, settings, and log-out screens
- 24 Java classes across login, catalogue, cart, and checkout

</details>

> **Disclosure:** group project — seven of us, not solo work. Members: Talha A. Serad,
> Sam Natad, French V. Barrera, Jawie N. Chanda, Radjan H. Bidin, Nikko P. Butaya,
> Laurence Lad. Data is in-memory and not yet persisted to a database.

---

### `02` Student Records System

**C# · .NET 10 · Windows Forms · academic final project · team of 2**

Windows desktop app for managing student records. Opens on a role selector and
organises students by program.

<details>
<summary><b>What I built</b> — 7 features</summary>

- **Role-based login** for Student, Faculty, and Admin
- Tabbed interface covering **nine programs**: BSIT, BSBA, BSN, BSCE, BSEE, BSCJ, BSHM, BSED, SHS
- Record entry for ID, name, age, gender, address, email
- Edit/save flows with form validation and logout confirmation
- Roughly **2,500 lines** of C# across the form logic
- First real experience working inside a shared codebase

</details>

> **Disclosure:** two-person final project. Not yet database-backed.

---

### `03` Simple POS

**Java · Swing · practice project · beginner level**

A small fast-food POS mimicking a counter ordering screen. Built to get comfortable
with Swing events and table models.

<details>
<summary><b>What I built</b> — 6 features</summary>

- Nine menu items, each a button with its own product image
- Per-item quantity controls before adding to the order
- `JTable` order list that recalculates subtotals on every add
- Automatic total and change/balance computation
- Receipt text area for the finished order

</details>

> **Disclosure:** known unfinished — the entry point isn't wired up, so it won't
> launch from the main class as-is.

---

### `04` This Portfolio

**HTML · CSS · vanilla JavaScript · self-directed**

The site, and the `Natad.html` / `Sam.CSS` files in this repo. Built from an empty
file rather than a template.

<details>
<summary><b>What I built</b> — 7 features</summary>

- Semantic HTML5 with landmarks and labelled sections
- Custom CSS design system — variables, Grid, Flexbox, no preprocessor
- Mobile-first responsive layout down to small screens
- Light and dark themes, preference saved locally
- Keyboard navigation, skip link, visible focus states
- Respects `prefers-reduced-motion` and print preferences
- Inline SVG icon set — no icon fonts, no CDN, no build step

</details>

## Continuous Learning

| Stage | Focus |
|---|---|
| **Foundation** | BSIT year one — logic, OOP, data structures, theory |
| **Applied** | Java and Swing apps; event-driven programming clicked here |
| **Capstone** | BuildHub, team of 7 — scope, merging code, others' designs |
| **Expanded** | C# and .NET, testing whether concepts transferred |
| **Now** *(Oct 2026)* | HTML/CSS fundamentals, data structures & algorithms, cleaner code |
| **Next** | SQL, so my apps stop losing data — then rebuild BuildHub as a web app |

## Education

**BSIT — Bachelor of Science in Information Technology**, graduated 2026

Programming fundamentals, OOP, data structures, networking, and databases, with
practical team experience in Java. Academic work: a seven-member capstone in Java and
a final C#/.NET app with a classmate.

## Contact

- **GitHub** — [@SamNatad](https://github.com/SamNatad)
- **Email** — *(add your real address here)*

Open to junior developer roles, internships, and mentorship.

---

<div align="center">
  <sub>Hand-written HTML and CSS. · Updated October 2026</sub>
</div>
