# Gemini CLI Git Commit Extension

This extension for [Gemini CLI](https://github.com/google-gemini/gemini-cli) automates the generation of Git
commit messages. By analyzing the changes in your staging area, it creates a professional title and a
descriptive body to keep your project history clear and concise.

## Features

- **Conventional Commits:** Automatically generates messages following the industry-standard [Conventional Commits](https://www.conventionalcommits.org/) specification.
- **Safety First (No Backticks):** Guarantees output without backticks (`), preventing the Gemini CLI from incorrectly identifying messages as bash commands.
- **Context Awareness:** Automatically activates when you ask to "commit this," "write a commit message," or similar requests.
- **Automated Analysis:** Inspects your Git staging area to understand code changes and provide meaningful context.
- **Seamless Integration:** Adds both an Agent Skill and a custom command directly into your Gemini CLI workflow.

## Installation

To install the extension, run the following command:

```bash
gemini extension install https://github.com/samucodesh/geminicli-gitcommit
```

## Usage

Once installed, you can trigger the extension within Gemini CLI using the custom command:

```bash
/git:commit
```

> [!NOTE]
> You must have changes staged in Git (`git add`) for the extension to analyze them.

## Uninstallation

To remove the extension from your system, use the following command:

```bash
gemini extension uninstall https://github.com/samucodesh/geminicli-gitcommit
```

## Resources

- **Troubleshooting:** If you encounter issues with the Gemini CLI, visit the [Troubleshooting Guide](https://github.com/google-gemini/gemini-cli/blob/main/docs/troubleshooting.md).
- **FAQ:** Check the [Gemini CLI FAQ](https://github.com/google-gemini/gemini-cli/blob/main/docs/faq.md) for common questions.

## License

This project is licensed under the **Apache License 2.0**. For more details, see the [LICENSE](https://github.com/samucodesh/geminicli-gitcommit/blob/main/LICENSE) file.
