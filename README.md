# Keyless submodule checkout

A demonstration of checking out submodules without deploy keys, by leveraging GitHub App.

## HOWTO

1.  Edit `.circleci/config.yml` to specify the location of the submodule (`path`) and its remote URL (`origin-http`). **The remote URL needs to be based on HTTP(S)**; the access credentials from GitHub App can be used only for HTTP(S)-based calls.

2.  Set up a CircleCI project for this repository and integrate it using GitHub App.
