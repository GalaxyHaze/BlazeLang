# BlazeLang 🔥

**BlazeLang** is a lightweight, high-performance programming language built for the next generation of scalable and maintainable systems.

At its core, BlazeLang runs on a minimal virtual machine written in **C/C++**, explicitly designed for performance-critical applications. It leverages a **hybrid ECS (Entity-Component-System)** architecture that’s exposed to the developer—giving you full control of data layout and execution—but also blends in **Object-Oriented Programming (OOP)** features for ergonomic development.

---

## 🚀 Why BlazeLang?

Modern software increasingly demands **performance**, **modularity**, and **maintainability**. BlazeLang was created to answer that call:

- 🔧 **Explicit ECS Core** – Take full control of memory and behavior with a transparent Entity-Component-System model.
- 🌀 **Blended Paradigm** – Mix ECS with familiar OOP constructs to boost productivity without sacrificing speed.
- ⚡ **C/C++ VM** – Backed by a lightweight virtual machine focused on efficiency, designed to run close to the metal.
- 🔬 **Modular by Design** – Encourage separation of concerns and scalable architecture from the ground up.
- 🧠 **Designed with Systems Thinking** – Ideal for simulations, games, procedural generation, and real-time applications.

---

## 📦 Features (WIP)

- ✅ Lightweight VM runtime (written in C/C++)
- ✅ Explicit ECS architecture with performance in mind
- ✅ Hybrid OOP support layered over ECS
- ⏳ Macro-based syntactic sugar for future DSLs
- 🛠️ Tooling roadmap (parser, debugger, REPL)

---

## 💡 Example Snippet

```blaze
entity Player {
    Health,
    Position,
    Velocity
}

system Move {
    query: [Position, Velocity]
    update(entity) {
        entity.Position += entity.Velocity * deltaTime
    }
}
