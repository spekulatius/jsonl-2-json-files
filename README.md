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
cat test.jsonl | ./jsonl-2-json-files /tmp/json-files
```

With `id` extracted from the JSON for the json-file name:

```bash
cat test.jsonl | ./jsonl-2-json-files /tmp/json-files '.id'
```

## Testing

You can test this script by running the `./test` script:

```bash
./test

Test completed.

If there is no `git diff` resulting from running this command the scripts work as expected.
```