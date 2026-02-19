# Verify Squashed Commits Action

This composite action ensures that Pull Requests maintain a clean history by verifying the 
number of commits before merging. 

## Usage

```
yaml
jobs:
  check-squash:
    runs-on: ubuntu-latest
    steps:
      - name: Verify PR is squashed
        uses: ./ci_squash
        with:
          max-commits: 1
```
## Inputs

* **max-commits**: Maximum number of commits allowed in the PR. (Default: `1`)

