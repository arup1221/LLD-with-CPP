<div align="center">

# 🏗️ Low-Level Design with C++

**Learn, practice and master Low-Level Design (LLD) — from OOP fundamentals to complete system designs — in modern C++.**

![C++](https://img.shields.io/badge/C%2B%2B-17-00599C?style=for-the-badge&logo=c%2B%2B&logoColor=white)
![License](https://img.shields.io/badge/License-All%20Rights%20Reserved-red?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-In%20Progress-orange?style=for-the-badge)

</div>

> 🚧 **Work in progress.** The OOP fundamentals module is complete — SOLID principles are up next.
> New topics are added regularly, and it will grow into a **complete LLD course in C++**. Star/watch the repo to follow along!

---

## 📖 About

This repository is a hands-on journey through **Low-Level Design** using C++. Every topic is explained with a
real-world analogy, heavily commented code, and a runnable `main()` so you can compile it and see the idea in action.

The goal is to cover the full LLD path:

1. **OOP fundamentals** – the building blocks
2. **SOLID principles** – writing maintainable code
3. **Design patterns** – proven solutions to recurring problems
4. **Complete system designs** – putting everything together in interview-style problems

---

## 🗺️ Roadmap

| # | Module | Topics | Status |
|---|--------|--------|:------:|
| 1 | [OOPS](OOPS/) | Abstraction, Encapsulation, Inheritance, Polymorphism (static & dynamic) | ✅ Done |
| 2 | SOLID Principles | SRP, OCP, LSP, ISP, DIP | ⏳ Planned |
| 3 | Creational Patterns | Singleton, Factory, Abstract Factory, Builder, Prototype | ⏳ Planned |
| 4 | Structural Patterns | Adapter, Decorator, Facade, Proxy, Composite | ⏳ Planned |
| 5 | Behavioral Patterns | Strategy, Observer, Command, State, Template Method | ⏳ Planned |
| 6 | Case Studies | Parking Lot, Elevator, Library Management, Vending Machine, BookMyShow, Splitwise, Chess, LRU Cache | ⏳ Planned |

Legend: ✅ Done · 🚧 In progress · ⏳ Planned

---

## 📂 Project Structure

```text
LLD with CPP/
├── OOPS/
│   ├── Abstraction.cpp                   # Abstract class (Car) vs concrete class (SportsCar)
│   ├── Encapsulation.cpp                 # Private state in SportsCar, accessed only via methods
│   ├── Inheritance.cpp                   # ManualCar & ElectricCar reuse common behaviour from Car
│   ├── StaticPolymorphism.cpp            # Compile-time: overloaded accelerate() in ManualCar
│   ├── DynamicPolymorphism.cpp           # Runtime: virtual overrides called through a Car* pointer
│   ├── StaticAndDynamicPolymorphism.cpp  # Overloading + overriding combined in one hierarchy
│   └── notes.txt                         # Abstraction vs Encapsulation comparison notes
├── .github/
│   └── CODEOWNERS
├── CLAUDE.md
├── LICENSE
└── README.md
```

> The structure grows as new modules are added (e.g. `SOLID/`, `DesignPatterns/`, `CaseStudies/`).

---

## 🧭 How to Use This Repo

1. Read the comments at the top of each file — they explain the concept with a real-world analogy.
2. Compile and run the code. Each file is a standalone program, for example:
   ```sh
   g++ -std=c++17 OOPS/Inheritance.cpp -o OOPS/Inheritance.exe
   ./OOPS/Inheritance.exe
   ```
3. Experiment locally on your own machine to understand how it works.
4. Move to the next topic in the roadmap.

---

## 📜 License

Copyright © 2026 Arup Gope. **All Rights Reserved.** You may read and run the code for personal learning, but modifying or redistributing it is not allowed without permission. See [`LICENSE`](LICENSE) for details.

---

<div align="center">

Made with ❤️ and C++ by **Arup Gope**

⭐ If this repo helps you, consider giving it a star!

</div>
