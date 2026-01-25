# Configuring Remotion for CLI Agents

This guide provides a structured setup for integrating Remotion with CLI-based agents like Open Code and Claude Code to create motion graphics, videos, and animations.

## Prerequisites
Ensure you have the following installed:
- Node.js (v18 or later)
- Bun (v1.0 or later)
- A project directory where you want to integrate Remotion

## Step-by-Step Setup

### 1. Install Remotion Skills
Install the Remotion skills package to enable agent interaction:

```bash
npx skills add remotion-dev/skills
```

**During installation:**
- Select the desired CLI tool (e.g., Open Code, Claude Code).
- Follow the prompts to complete the setup.

This step initializes the necessary configurations and dependencies for Remotion to work with your agent.

### 2. Initialize a Remotion Project
Create a new Remotion project using the Bun CLI to generate a structured project directory:

```bash
bun create video
```

**This command:**
- Sets up a project directory with a template.
- Creates a `skills` folder for agent interaction.
- Configures the project for Remotion-based video and motion graphics production.

### 3. Interact with the Agent
After initializing the project:
- Navigate into the newly created directory:
  ```bash
  cd <project-directory>
  ```

- **Interact with the agent** in this directory. The agent will utilize the `skills` folder to execute Remotion commands and generate motion graphics, videos, and animations.

## Key Notes
- The `skills` folder created by `bun create video` is essential for seamless agent interaction.
- Ensure the agent has access to this folder to dynamically control Remotion compositions, assets, and exports.
- Use the `skills` folder to parametrize compositions with Zod schemas for dynamic agent input.

## Best Practices

- **Use Zod schemas** for parametrizable compositions to allow dynamic agent input.
- **Optimize assets** (images, videos, fonts) for performance and compatibility.
- **Leverage Remotion’s composition structure** for modular and reusable animations.
- **Implement proper metadata handling** to ensure accurate video dimensions and durations.
- **Utilize TailwindCSS or CSS-in-JS** for styling animations and compositions.

This setup ensures your Remotion project is ready for integration with CLI agents, enabling efficient and scalable motion graphics production.



