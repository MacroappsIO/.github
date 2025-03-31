# MacroApps Architecture

**MacroApps** is an open-source, modular architecture built in TypeScript for developing enterprise-grade Node.js applications with clean, decoupled services.

Inspired by architectures like [Athenna](https://athenna.io), MacroApps provides a solid foundation for scalable backend applications, offering clear boundaries across modules such as `IoC`, `Core`, `Common`, and `CLI`.

> ✅ Built for developers, open to the community, and licensed under MIT.

---

## 🧱 Monorepo Structure

Each module is developed and maintained in isolation to encourage separation of concerns, scalability, and testability.

```
microapps/
├── ioc/           → Inversion of Control container (✅ completed)
├── core/          → Application lifecycle and service providers (🔜 planned)
├── common/        → Shared types, utilities, exceptions (🔜 planned)
├── cli/           → Command-line tooling for DX & scaffolding (🔜 planned)
```

All packages are ESM-first, written in TypeScript, and fully testable.

---

## 📦 Modules Overview

| Package     | Status    | Description                                  |
|-------------|-----------|----------------------------------------------|
| `@macroapps/ioc`     | ✅ Completed | Lightweight IoC container with decorators and scoped resolution |
| `@macroapps/core`    | 🔜 Planned   | App lifecycle, bootstrapping, and service providers              |
| `@macroapps/common`  | 🔜 Planned   | Shared helpers, domain errors, constants                         |
| `@macroapps/cli`     | 🔜 Planned   | Developer tooling and scaffolding CLI                            |

> ⚠️ Currently, only the `ioc` module is implemented. Other modules will be released gradually.

---

## 🚀 Quick Start (IOC Module)

If you want to explore or contribute to the IoC module:

```bash
git clone https://github.com/MacroappsIO/Ioc/
cd Ioc
npm install
npm run test
```

For full usage, see https://github.com/MacroappsIO/Ioc/blob/main/README.md.

---

## 📚 Technologies Used

- ✅ TypeScript (strict mode)
- ✅ ESM-only
- ✅ Japa + tsx for testing
- ✅ `reflect-metadata` for decorators
- ✅ Factory, value, and class providers
- ✅ Scoped resolution and lazy injection
- ✅ Support for module auto-loading via glob

---

## 🧩 Philosophy

> **Minimal, testable, extendable** — the core principles behind MacroApps.

This project is being built with a focus on maintainability and flexibility across large applications. It's structured in a way that lets developers adopt only the pieces they need, without being forced into a monolith.

---

## 👥 Community & Contributing

**MacroApps is open-source and built for the community.**

If you're a developer looking for a clean DI container, a contributor interested in modular architectures, or a team building scalable Node.js apps — you're welcome here!

Contributions are encouraged, and collaboration is open.

- PRs and issues are welcome.
- Please follow the code style and use the test suite to validate changes.

---

## 📌 Roadmap

- [x] `@macroapps/ioc`: IoC container
- [ ] `@macroapps/core`: Lifecycle, boot, providers
- [ ] `@macroapps/common`: Shared types, utilities
- [ ] `@macroapps/cli`: CLI tool for scaffolding
- [ ] Documentation website
- [ ] NPM release pipeline

---

## 📄 License

**MIT License**

Created and maintained by [R. Souza](https://github.com/RobsonTrasel)

> This project is open-source and free to use for both personal and commercial purposes.
