# 📦 Monorepo Practice — Flutter Monorepo Example

![Flutter](https://img.shields.io/badge/Flutter-Framework-blue?logo=flutter)
![Dart](https://img.shields.io/badge/Dart-Language-blue?logo=dart)
![GitHub](https://img.shields.io/badge/GitHub-Monorepo_practice-black?logo=github)

This repository demonstrates a **Flutter monorepo structure** using a workspace setup.  
It allows organizing multiple apps and shared packages in a single repository while enabling code sharing, modularity, and scalable project organization.

This project was created as a **practice project** to explore monorepo architecture in Flutter.

---

## 🧠 What is a Monorepo?

A *monorepo* (monolithic repository) is a project structure where multiple related applications and packages reside in a single repository.  
In Flutter, this structure helps:

- Share **widgets, utilities, and packages** across multiple apps :contentReference[oaicite:0]{index=0}
- Centralize **dependency management** :contentReference[oaicite:1]{index=1}
- Simplify refactoring and reuse :contentReference[oaicite:2]{index=2}

Monorepos are often used with tools like **melos** to manage workspaces and dependencies.

---

## 🗂️ Repository Structure

```

Monorepo_practice/
├── apps/ # Flutter apps
│ ├── example_app/ # Example application
│ └── ... # Add more apps here
├── packages/ # Shared packages / modular libraries
│ └── ... # Add reusable package folders here
├── melos.yaml # Workspace configuration
├── pubspec.yaml # Root project config
└── README.md # This documentation
```

---

## 🚀 Getting Started

This repository uses **melos** (a Dart/Flutter workspace manager) to handle dependencies and linking between apps and packages.

### 1️⃣ Install Melos

If you don’t have melos installed:

```bash
dart pub global activate melos

Make sure ~/.pub-cache/bin is in your PATH.
```

### 2️⃣ Bootstrap the Workspace
```bash
Run the following to install dependencies and link packages:
melos bootstrap

This will:
Install all package and app dependencies
Link local packages into apps
```

### 3️⃣ Run an App
```bash
Navigate to one of the apps and run it like a regular Flutter project:

cd apps/example_app
flutter run

You can add more apps under apps/ and each app can use shared code from packages/.
```
---

### 📌 Why Use a Monorepo in Flutter?

A monorepo structure is useful when:
- You want to share widgets/utilities across multiple Flutter apps
- You are building a multi-app product suite
- You want to manage features and modules in an organized workspace 

Benefits include:
- Centralized dependencies
- Shared code without duplication
- Easier atomic changes across apps 

### 🧪 Testing in Monorepo

You can run tests across all apps and packages using melos:

```bash
melos run test
```

This command will find and run all tests inside your workspace (if tests are added).

---

### 🧩 Best Practices for Monorepo

- Split code into feature-based packages
- Avoid cyclic dependencies between packages
- Use melos for bootstrap, linking, and scripting
- Keep shared widgets and utilities in reusable packages 

---

### 📌 Notes

- This project is structured for practice and learning monorepo concepts
- You can expand it with your own apps and shared packages
- Add CI/CD workflows and automated testing for production-ready setups

---

## 👨‍💻 Author

**Chorus Rajbanshi** - Flutter Developer (Fresher)

🔗 https://github.com/Chorusraj
🔗 https://www.linkedin.com/in/chorus-rajbanshi-32ba7a330/

