# jira-title-check-action

An Action to ensure that PR's and Commits have a Jira ticket associated with it.

## Usage

```yaml
- step:
    name: check-jira-title
    use: Epallet/jira-title-check-action@V1
```

It requires that the Head Commit message of a push or the title of a Pull Request start with an identifier formatted following  the regex: `\[?[A-Z]+-[0-9]+\]?` with a maximum length of 10 characters.

Examples:

* `ABC-1235`
* `[ABC-1235]`
