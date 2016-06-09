# Plugin repo updater

----

A script to update plugin repos with dir names matching one or more substring patterns

### Installation:

- Download the `updater` file.
- Place it in the parent directory of where your repos are located.
- Customize as needed
- For permissions issues, run `chmod +x updater`


----

#### AffiliateWP usage:

- Download the `updater` file here, and place it in `/plugins`
- Script currently checks for any plugin starting with `affiliate-wp` or `affiliatewp`
- Follow prompts.

----

#### TODO:

- [x] Make sure there are no unstaged changes before attempting an update. Bail if not. (Using `git diff --quiet`)
- [ ] Ability to update custom branches per repo
- [ ] Save settings in a `.config` file _(or something)_
- [ ] Completion of updating the current `HEAD` via `git rev-parse --abbrev-ref HEAD`
