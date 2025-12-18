# Gemini CLI Git Commit Extension

This extension for [Gemini CLI](https://github.com/google-gemini/gemini-cli) automates the generation of Git
commit messages. By analyzing the changes in your staging area, it creates a professional title and a
descriptive body to keep your project history clear and concise.

## Features

- **Automated Analysis:** Inspects your Git staging area to understand code changes.
- **Smart Generation:** Produces an AI-generated title and description based on the context of your work.
- **Seamless Integration:** Adds a custom command directly into your Gemini CLI workflow.

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

- **Troubleshooting:** If you encounter issues with the CLI, visit the [Troubleshooting Guide](https://github.com/google-gemini/gemini-cli/blob/main/docs/troubleshooting.md).
- **FAQ:** Check the [Gemini CLI FAQ](https://github.com/google-gemini/gemini-cli/blob/main/docs/faq.md) for common questions.

## License

This project is licensed under the **Apache License 2.0**. For more details, see the [LICENSE](https://github.com/samucodesh/geminicli-gitcommit/blob/main/LICENSE) file.
