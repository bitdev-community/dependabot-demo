# Dependabot Demo
A demo of using Dependabot to install newer versions of Bit Component dependencies.

- [Dependabot Config](https://github.com/bitdev-community/dependabot-demo/blob/main/.github/dependabot.yml)
- [Dependabot Results](https://github.com/bitdev-community/dependabot-demo/network/updates)

## Configuring Dependabot for Bit

```
version: 2
updates:
  - package-ecosystem: "npm"
    directory: "/"
    schedule:
      interval: "daily"
    groups:
      showoff-scope-dependencies:
         patterns:
           - "@showoff*"
```

In the above configuration, dependabot is only checking the Bit scope @showoff for new version updates.
