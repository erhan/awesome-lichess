# Maintaining Awesome Lichess

## Growing the list

The first pass contains four topic categories and nine resources. Keep additions focused on useful resources with a clear Lichess connection. Add categories only when there are entries to populate them, and keep `Contents` synchronized with the resource headings.

## Checks

From the repository root, with Node.js 20 or newer and Git installed, run:

```sh
npx --yes awesome-lint@2.3.0 README.md
git diff --check
```

The first command downloads the pinned linter version if needed. Version 2.3.0 allows a missing table of contents and does not enable its repository-age rule, so a passing result does not mean the list meets the upstream submission checklist. Review the output and fix findings; do not disable rules to make an unfinished list appear ready. CI can be added as the list grows.

Verify resource links and descriptions manually as well; linting does not establish resource quality or fair-play compliance.

## Before submitting to the Awesome directory

Re-read the current [Awesome manifesto](https://github.com/sindresorhus/awesome/blob/main/awesome.md), [creation instructions](https://github.com/sindresorhus/awesome/blob/main/create-list.md), and [submission checklist](https://github.com/sindresorhus/awesome/blob/main/pull_request_template.md). The upstream requirements may change.

- Build a useful, personally evaluated list. The upstream checklist requires that the list is not AI-generated; scaffolding and a successful lint run do not establish eligibility.
- Confirm that this list offers a distinct scope from existing lists and submissions.
- Add populated topic categories and a matching `Contents` section. Exclude `Contributing` and `Footnotes` from the contents links.
- Keep the title, Awesome badge, succinct explanation of Lichess, and contribution guidelines. Keep licensing in the root `LICENSE` file, without adding a license section or license name to the README.
- Keep obsolete or archived resources out of the main list. Consider a relevant illustration if useful.
- Set the GitHub topics `awesome` and `awesome-list`, along with relevant topics such as `lichess` and `chess`.
- Wait at least 30 days from the first real commit or public release, whichever is later.
- Pass `awesome-lint` and verify links and descriptions.
- Complete the upstream submission requirements, including meaningful reviews of at least four other open pull requests, before submitting a finished proposal.

The Awesome badge can be used before directory inclusion; it does not mean the list has been accepted.
