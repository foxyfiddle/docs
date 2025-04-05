# How To Create a Vite Application

- Ensure [Node.js] is installed on your machine.
- A terminal or command prompt is required to run the installation command
- replace `<project-name> in the steps below with the desired name for your project directory

---

## Step 1: Create a New Vite Project

Open your terminal and run the following command to create your Vite project:
```bash
npm create vite@latest <project-name>
```

During the project creation, you will be prompted to:
- Select a framework: Choose between options like Vanilla, React, Vue, Svelte, etc.
- Choose a variant: Decide on JavaScript or typeScript for your project.

## Step 2: Navigate to the Project Directory

Once the project is created, move into your project folder:
```bash
cd <project-name>
```

## Step 3: Install Dependencies

install all the required dependencies by running:
```bash
npm install
```
This command downloads and sets up all packages mentioned in the project's `package.json` file.

## Step 4: Start the Development Server

Start the Vite development server with the following command:
```bash
npm run dev
```
The terminal will display a local development URL(typically `http://localhost.5173/`).
Open this URL in your browser to see your app in action.

---

Additional Commands:
- Build for Production:
  When you're ready to deploy your application, build it using:
  ```bash
  npm run build
  ```
- Preview the Production Build:
  To Preview the production build locally, run:
  ```bash
  npm run preview
  ```
