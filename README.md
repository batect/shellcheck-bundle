# shellcheck-bundle

[![Build Status](https://img.shields.io/github/workflow/status/batect/shellcheck-bundle/Pipeline/master)](https://github.com/batect/shellcheck-bundle/actions?query=workflow%3APipeline+branch%3Amaster)
[![License](https://img.shields.io/github/license/batect/shellcheck-bundle.svg)](https://opensource.org/licenses/Apache-2.0)

A bundle for [batect](https://batect.dev) that provides a task to lint shell scripts with [ShellCheck](https://github.com/koalaman/shellcheck).

## Usage

### Setup

Add the following to your `batect.yml`:

```yaml
include:
  - type: git
    repo: https://github.com/batect/shellcheck-bundle.git
    ref: XXX # Replace with latest version from https://github.com/batect/shellcheck-bundle/releases
```

### Tasks

### `lint:shell`

Runs [ShellCheck](https://github.com/koalaman/shellcheck) on all shell scripts in the project directory.

Recursively searches for any files ending in `.sh`.

Exits with a non-zero status code if any issues are found.

## Development

Run `./batect --list-tasks` to see a list of available tasks for this project.
