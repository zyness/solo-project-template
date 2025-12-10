# Solo Project Template & Framework

## 🎯 Purpose
This repository serves as a **foundation for one-person projects**. It provides a lightweight project management structure designed to help solo developers balance the roles of **Product Manager**, **Developer**, and **QA** without getting overwhelmed.

It is optimized for use with **GitHub Copilot Spaces**.

## 📂 What's Inside?
- **`docs/`**: A set of generic, "Copilot-ready" markdown files defining the project lifecycle (Initiation, Planning, Execution).
- **`.github/ISSUE_TEMPLATE/`**: Structured templates to ensure consistency when defining tasks.
- **`.gitignore`**: A polyglot configuration covering Node.js, Python, .NET, and standard IDE files.

## 🚀 How to Start a New Project

### 1. Instantiate
Click the green **"Use this template"** button to create a new repository for your specific project.

### 2. Configure Copilot Space
Go to [GitHub Copilot Spaces](https://github.com/copilot/spaces) and create a new Space for your new repository.
- **Source:** Select your new repository.
- **Instructions:**
  > "You are my assistant for this solo project. I act as PM, Dev, and QA. Your knowledge base is in the `docs/` folder. Always refer to `docs/roles-and-personas.md` to understand which 'Hat' I am currently wearing. Help me maintain a sustainable pace and strictly follow the 'Definition of Done'."

### 3. Define the Project (The "Initiation")
Open `docs/project-initiation.md` and fill out the **Project One-pager** section.
- Define the **Goal**.
- Define the **Tech Stack** (e.g., C#/.NET 8, Next.js, Python FastAPI).
- Define **Success Metrics**.

### 4. Generate the Project README
Once Step 3 is done, ask Copilot in your Space:
> "Based on the Tech Stack and Goals defined in `docs/project-initiation.md`, please generate a specific `README.md` for this project's root directory. It should replace this template README and include sections for 'Installation', 'Tech Stack', and 'Getting Started'."

### 5. Scaffold Code
Open your terminal and generate the project skeleton based on your chosen stack (e.g., `dotnet new`, `npx create-next-app`).

## 🎩 The Methodology (Wearing Hats)
This framework relies on consciously switching modes:
- **PM Mode:** Plan in the morning or start of a milestone. Don't code.
- **Dev Mode:** Execute the plan. Don't rethink features.
- **QA Mode:** Verify before marking "Done".

See `docs/roles-and-personas.md` for details.