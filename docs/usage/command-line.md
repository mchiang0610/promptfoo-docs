---
sidebar_position: 10
sidebar_label: Command line
---

# Command-line options

If you're looking to customize your usage, there are a wide set of `promptfoo eval` parameters at your disposal.

| Option                              | Description                                                                                                                                                                  |
| ----------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `-p, --prompts <paths...>`          | Paths to [prompt files](/docs/configuration/parameters#prompt-files), directory, or glob                                                                                     |
| `-r, --providers <name or path...>` | One of: openai:chat, openai:completion, openai:model-name, localai:chat:model-name, localai:completion:model-name. See [API providers](/docs/providers)        |
| `-o, --output <path>`               | Path to [output file](/docs/configuration/parameters#output-file) (csv, json, yaml, html)                                                                                    |
| `-t, --tests <path>`                | Path to [external test file](/docs/configuration/expected-outputs#load-an-external-tests-file)                                                                               |
| `-c, --config <path>`               | Path to [configuration file](/docs/configuration/guide). `promptfooconfig.js/json/yaml` is automatically loaded if present                                                   |
| `--grader`                          | [Provider](/docs/providers) that will conduct the evaluation, if you are [using LLM to grade your output](/docs/configuration/expected-outputs#llm-evaluation) |
| `--no-cache`                        | Disable cache                                                                                                                                                                |
| `--no-table`                        | Disable CLI table output                                                                                                                                                     |
| `--no-write`                        | Do not write the latest config to disk (used for web viewer and sharing)                                                                                                     |
| `--prompt-prefix <path>`            | This prefix is prepended to every prompt                                                                                                                                     |
| `--prompt-suffix <path>`            | This suffix is append to every prompt                                                                                                                                        |
| `--share`                           | Automatically create a share link                                                                                                                                            |
| `--table-cell-max-length <number>`  | Truncate console table cells to this length                                                                                                                                  |
| `--verbose`                         | Show debug logs                                                                                                                                                              |
| `--view`                            | Open local web viewer                                                                                                                                                        |
| `-j, --max-concurrency <number>`    | Maximum number of concurrent API calls                                                                                                                                       |
