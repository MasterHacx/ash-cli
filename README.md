# Aisha CLI (ash-cli) v2.1

Aisha CLI is an interactive AI chat assistant designed for your command line.
It offers personalized conversations, remembers information, and provides a smooth, customizable, and flicker-free user experience.

## Features:
- Personalized conversational AI (Angel/Evil modes)
- Customizable user and bot names
- Dynamic system prompts for AI persona
- Memory management (remember/recall specific facts)
- Web search grounding for factual queries
- Command history (Up/Down arrows)
- Command auto-completion (Tab key)
- **Flicker-free display** for long responses, ensuring a smooth reading experience.
- Customizable configuration via `config.json` and `aisha_custom_settings.json`

## Installation

You can install Aisha CLI using pip:

```bash
pip install ash-cli
```

### Upgrading from a Previous Version

If you have an older version of `ash-cli` installed, you can upgrade to the latest version with:

```bash
pip install --upgrade ash-cli
```

## Usage

After installation, you can run Aisha from any terminal by simply typing `ash`:

```bash
ash
```

Type `help` or `h` for a list of all available commands and their short aliases.

## Configuration

Aisha uses two configuration files, which will be created in your current working directory when you run `ash` for the first time:

- `config.json`: Contains core settings like API keys and model preferences.
- `aisha_custom_settings.json`: Stores your personalized settings such as your name, Aisha's name, and custom AI personas. You can also manage these via the `set` and `reset settings` commands.

## Getting Started

1. **Install:** `pip install ash-cli`
2. **Run:** `ash`
3. **API Key:** On first run, you will be prompted to enter your Google Gemini API key. You can get one from [Google AI Studio](https://makersuite.google.com/app/apikey).
4. **Personalize:** Follow the prompts to set your name and Aisha's name. You can change these later with `set name <your_name>` and `set botname <new_name>`.

## Commands

Aisha supports a variety of commands, many with short aliases:

- `help` / `h`: Show available commands.
- `exit` / `quit` / `bye` / `x`: Exit the chat.
- `clear` / `c`: Clear the console screen.
- `angel`: Switch to Angel Mode.
- `evil`: Switch to Evil Mode.
- `remember <text>` / `rem <text>`: Store a memory. (e.g., `rem my_name: Raunak`)
- `recall <keyword>` / `rec <keyword>`: Find memories.
- `show memory` / `memory` / `mem`: Display all memories.
- `forget all` / `fmem`: Clear all memories.
- `history` / `hist`: Show chat history.
- `delete history` / `dh`: Clear chat history.
- `search on` / `son`: Enable web search groxunding.
- `search off` / `soff`: Disable web search grounding.
- `set name <your_name>`: Set your display name.
- `set botname <aisha_name>`: Set Aisha's display name.
- `set prompt angel <new_prompt>`: Customize Angel persona.
- `set prompt evil <new_prompt>`: Customize Evil persona.
- `reset settings` / `rs`: Reset custom names/prompts to default.

## License

This project is licensed under the MIT License - see the LICENSE file for details.
