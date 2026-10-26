# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What this repo is

A teaching repository for Low-Level Design in C++ (targets C++17). It is meant to grow module by module, following the roadmap in `README.md`: OOPS → SOLID → Creational / Structural / Behavioral patterns → Case Studies (Parking Lot, Elevator, LRU Cache, etc.). New modules go in their own top-level folder (e.g. `SOLID/`, `DesignPatterns/`, `CaseStudies/`).

## Build & run

There is no build system, test suite, or linter. Each `.cpp` file is a standalone program with its own `main()`. The toolchain on this machine is MinGW `g++`:

```sh
g++ -std=c++17 OOPS/Inheritance.cpp -o OOPS/Inheritance.exe
./OOPS/Inheritance.exe
```

The compiled `.exe` sits next to its source file. Some `.exe` files are tracked in git.

## Conventions for example files

Every topic file uses the same layout. Match it when you add a new one:

- Only `#include <iostream>`, `#include <string>`, and `using namespace std;`. No headers outside the standard library, and no multi-file programs.
- A block comment at the top, or above each class, explains the concept with a real-world analogy. Most files build on the **car** analogy (`Car`, `ManualCar`, `SportsCar`, etc.).
- The comments are heavy and written for learners. Keep this teaching style.
- Each `main()` demonstrates the concept, often by creating objects with `new` and assigning them to base-class pointers, then calling `delete` at the end.
- Classes print what they do using the pattern `cout << brand << " " << model << " : <action>" << endl;`.

`OOPS/notes.txt` holds plain-text concept notes, such as Abstraction vs Encapsulation in a comparison table.

## When adding a topic

Update `README.md` as well. Its roadmap table has status markers (✅ / 🚧 / ⏳), and its "Project Structure" tree should list the new files.

## Licensing / ownership

The project is All Rights Reserved (see `LICENSE`). `.github/CODEOWNERS` assigns every file to the repo owner. Do not add any other license headers.
