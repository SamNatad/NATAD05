# PROJECT 3 — BuildHub

**Project:** BuildHub — PC Parts Ordering System (desktop)
**Language:** Java
**Repository:** `Natad05`
**Documentation:** https://www.facebook.com/share/v/1A3k5kKv9E/

**Main concept:** A desktop point-of-sale / ordering application for PC components, built with Java Swing. Customers register, verify their account with a one-time code, browse products by category, add items to a cart, and pay with change calculated live.

**Category:** Java / Object-Oriented Programming
**Level:** Beginner / Academic Project (BSIT capstone, team of 7)

> Verified by reading the 24 `.java` source files (5,900 lines). The Facebook link is
> documentation and certificate material only — the feature and OOP claims below come
> from the code, not the project name or the documentation.

---

## OOP concepts actually demonstrated

Counted from the source, not assumed:

| Concept | Evidence | Count |
|---|---|---|
| **Classes** | One public class per file | 24 classes |
| **Objects** | Instances created with `new` — `new Dashboard()`, `new BuildHubLogin()`, `new java.awt.event.ActionListener()` | 22 windows + 99 anonymous listeners |
| **Inheritance** | `extends javax.swing.JFrame` — each window class reuses JFrame's windowing, layout and event behaviour | 22 classes extend JFrame |
| **Encapsulation** | All Swing components declared `private`; behaviour exposed through public methods (`addtable`, `cal`, `actionPerformed`) | 387 private fields, only 2 public fields |
| **Polymorphism** | Anonymous `ActionListener` implementations dispatch on event; inherited JFrame methods called on JFrame-typed instances. `@Override` on `actionPerformed` | 99 anonymous inner classes |
| **Constructors** | One explicit no-arg constructor per window class, each calling `initComponents()` | 20 constructors |
| **Methods** | Public methods including 23 `main` entry points, 22 `initComponents()`, and the business logic below | 164 public methods |

### Concepts NOT demonstrated

Listed explicitly so the project isn't overstated:

- **Abstraction (custom) — not present.** The project contains **zero** interfaces and
  **zero** abstract classes of its own. It *consumes* a JDK abstraction
  (`java.awt.event.ActionListener`) but does not design one.
- **No method overloading, generics, enums, records, or interfaces authored.**
- **No inheritance between the project's own classes** — all inheritance comes from
  the Java library.

### Business logic worth pointing out

- `addtable(int id, String name, int qty, double price)` — cart line insertion
  (`CASE.java:25`, `Monitor.java:28`, `System.java:26`). Re-adding an existing item
  replaces the row so quantity updates rather than duplicating.
- `cal()` — recomputes the order total by summing the table's total column, formatted
  with `java.text.DecimalFormat`.
- Payment: `balance = paid - total`, with subtotal appended to a receipt `JTextArea`.
- OTP: a `javax.swing.Timer` runs a 60-second countdown, updating a button's label
  and rejecting non-numeric input (`OTP.java:161-185`).

---

## Screenshots

![BuildHub screenshot 1](img/buildhub-1.jpg)
![BuildHub screenshot 2](img/buildhub-2.jpg)
![BuildHub documentation / certificate](img/buildhub-certificate.jpg)

---

## Honest limitations

This was a beginner academic project, and these are real constraints a reviewer would
find:

- **Credentials are hardcoded in source** — `FORNEWPASSWORD.java` holds
  `public static String username = "user1234"` and compares them in plain text at
  `BuildHubLogin.java:191`. Not acceptable outside a classroom.
- **No database.** Everything is held in the running JVM, so all accounts, carts and
  orders are lost on exit.
- **Facebook and Gmail login are UI screens only** — no OAuth or network calls exist
  in the code.
- **Error handling is thin.** Most paths lack validation, try/catch, or input bounds.
- **Duplicated logic.** The cart methods are copy-pasted across `CASE`, `Monitor` and
  `System` rather than shared through a superclass — the obvious next refactor.

## What I'd do next

1. Move credentials to a database with hashed passwords.
2. Extract the duplicated `addtable`/`cal` logic into a shared `Cart` class — the
   first real inheritance/inheritance-hierarchy lesson in this project.
3. Add input validation and a proper error layer.
