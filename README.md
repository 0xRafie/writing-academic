# writing-academic

An agent skill for writing, editing, and translating academic English. It works with Claude Code, Codex, Factory Droid, Grok CLI, and any other agent that reads `SKILL.md`.

## Contents

- `SKILL.md`: the rules most often broken, each with a correct and an incorrect example.
- `reference.md`: numbers (APA and IEEE side by side), abbreviations, punctuation, grammar and usage, clarity, spelling, and a table for translating Indonesian drafts into English.

## Sources

- American Psychological Association. *Publication Manual of the American Psychological Association* (7th ed.) and the APA Style website: https://apastyle.apa.org/style-grammar-guidelines
- IEEE. *IEEE Editorial Style Manual for Authors*. IEEE Author Center.
- Plain Language Action and Information Network. *Federal Plain Language Guidelines* (2011). https://digital.gov/guides/plain-language

## Installation

For Claude Code:

```bash
git clone https://github.com/0xRafie/writing-academic ~/.claude/skills/writing-academic
```

Other agents can symlink the same clone:

```bash
ln -s ~/.claude/skills/writing-academic ~/.agents/skills/writing-academic   # Codex
ln -s ~/.claude/skills/writing-academic ~/.factory/skills/writing-academic  # Factory Droid
ln -s ~/.claude/skills/writing-academic ~/.grok/skills/writing-academic     # Grok CLI
```

The skill activates when the agent writes or edits academic English. In Claude Code you can also call it with `/writing-academic`.

## Personal style

Put your own rules in `personal-style.md` inside the skill folder, for example "avoid 'we'; write 'this study' instead". The agent reads the file before writing, and its rules override the defaults. The file is listed in `.gitignore`, so it is never pushed.

## License

[MIT](LICENSE)
