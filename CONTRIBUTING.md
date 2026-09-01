# Contributing

Contributions are welcome. A useful entry tells readers not only that a dataset exists, but whether they can retrieve, combine, and redistribute it.

## Before opening a pull request

- Search the README and existing pull requests for duplicates.
- Link to a stable landing page or DOI, not a temporary download URL.
- Verify that the source is a dataset or machine-readable database. Put educational resources and software in an explicitly labeled related-resources section.
- Check the access method and license at the source. Write `license not stated` or `proprietary` when applicable; do not infer a license from free access.
- Prefer current facts over record counts that will immediately become stale. If a count is important, include the release or date.
- Check spelling, grammar, and links, and remove trailing whitespace.

## Entry format

Use this compact format:

```markdown
- [Dataset name](https://stable-landing-page.example/): Scope and data type. Access: bulk/API/files. Identifiers: InChIKey, DOI, etc. License: SPDX name or "not stated".
```

Not every field will be available, but access and license information are especially valuable. Mention important constraints such as registration, API keys, non-commercial terms, mixed per-record licensing, or predicted rather than experimental values.

For additions to [Dataset opportunities](OPPORTUNITIES.md), describe the proposed product, join keys, why the sources are complementary, the largest scientific caveat, and the relevant licenses.
  

## Creating a pull request

1. [Fork](https://docs.github.com/en/get-started/quickstart/fork-a-repo) the repository.
2. [Create a branch](https://git-scm.com/book/en/v2/Git-Branching-Basic-Branching-and-Merging) for your addition.
3. Open a pull request with a short explanation of what the dataset enables and how you verified its access and license information.

## Credits

This contribution guide is based on the one from [awesome-materials-informatics](https://github.com/tilde-lab/awesome-materials-informatics).
