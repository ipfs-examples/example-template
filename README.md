## Getting Started

This project is a template to be used to pull a given example from a folder/directory of another repository.

### Prerequisites

Check if exists a github action to perform the pull from another repository.

### Installation

Change the github action workflow, `sync` accordingly to your needs:

``` yaml
- name: Pull from another repository
  uses: ipfs-examples/actions-pull-directory-from-repo@main
  with:
    destination-repo: # mandatory, ex: 'ipfs-examples/examples-source'
    destination-folder-path: # mandatory, ex: 'examples/example2'
    destination-branch: # optional, can be omitted, defaults to: 'main'
    source-branch: # optional, can be omitted, defaults to: 'main'
    git-username: # optional, can be omitted, defaults to: 'github-actions'
    git-email: # optional, can be omitted, defaults to: 'github-actions@github.com'
```

_For more information, please refer to the [Documentation](https://github.com/ipfs-examples/actions-pull-directory-from-repo)_

## Usage

This repository will sync automatically based on the timer of the workflow, you can trigger manually:

- Go to the repository on Github
- Go to the `Actions` section
- Select the `Sync` workflow
- Run the workflow

_For more information, please refer to the [Documentation](https://docs.github.com/en/actions/managing-workflow-runs/manually-running-a-workflow)_
