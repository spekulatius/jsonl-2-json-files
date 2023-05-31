# jsonl ➡️json files

## Install & Usage

Copy it somewhere.

## Usage

```bash
$ ./jsonl-2-json-files
Usage: ./jsonl-2-json-files <output_directory> [jq_selector] [input_file.jsonl]
```

With indexed files (`1.json`, `2.json`, ...):

```bash
cat input.jsonl | ./jsonl-2-json-files /tmp/json-files
```

With `id` extracted from the JSON for the json-file name:

```bash
cat input.jsonl | ./jsonl-2-json-files /tmp/json-files '.id'
```