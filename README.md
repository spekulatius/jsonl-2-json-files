# jsonl ➡️json files

## Install & Usage

Copy it somewhere.

## Usage

Basic usage:

```bash
$ ./jsonl-2-json-files
Usage: ./jsonl-2-json-files <output_directory> [jq_selector] [input_file.jsonl]
```

To generate indexed files (`1.json`, `2.json`, ...):

```bash
cat test.jsonl | ./jsonl-2-json-files /tmp/json-files
```

To use the `id` field from the JSON as the output filename:

```bash
cat test.jsonl | ./jsonl-2-json-files /tmp/json-files '.id'
```

The script automatically formats the JSON files for improved readability.

## Testing

You can test the script by executing the `./test` script:

```bash
./test

Test completed.

If there is no `git diff` resulting from running this command the scripts work as expected.
```