# gh-codeql-db
A very basic gh extension to list and download CodeQL databases.

## Installation

```bash
gh extension install rvermeulen/gh-codeql-db
```


## Usage

### Listing CodeQL Databases

To list available CodeQL databases for a repository, run:

```bash
gh codeql-db list <owner/repo> [language]
```

**Example:**

```bash
gh codeql-db list spring-projects/spring-framework
gh codeql-db list spring-projects/spring-framework java
```

If you omit the language parameter, you'll receive the all the available databases.

### Downloading a CodeQL Database

To download a CodeQL database for a specific repository and language, run:

```bash
gh codeql-db download <owner/repo> <language>
```

**Example:**

```bash
gh codeql-db download spring-projects/spring-framework java
```

## Requirements

- [gh CLI](https://cli.github.com/)
- [jq](https://stedolan.github.io/jq/)

Ensure you are authenticated with the `gh` CLI before using this extension.
