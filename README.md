# Plugin repo updater

----

A script to update all plugin repos within the `plugins` parent dir.

This version will only update plugins with dir names matching one or more substring patterns.

Presently, these patterns are: `affiliatewp` and `affiliate-wp`.

----

### Installation:

- `cd` into your `plugins` dir (or the parent directory of wherever your repos are located).
- Download the `updater` file:
    `curl -O https://raw.githubusercontent.com/ramiabraham/plugin-repo-updater/master/updater`
- Customize as needed (you'll need to change the match patterns, as it presently is set to check `affiliatewp` and `affiliate-wp` folder name prefixes only.
- For permissions issues, run `chmod +x updater`.

#### Usage

- Run the updater with `./updater`
- Follow the prompts (see TODO below for in-progress stuff).

----

#### AffiliateWP usage:

- `cd` into your `plugins` dir.
- Download the `updater` file:
    `curl -O https://raw.githubusercontent.com/ramiabraham/plugin-repo-updater/master/updater`
- Script currently checks for any plugin starting with `affiliate-wp` or `affiliatewp`
- Follow prompts.

----

#### TODO:

- [x] Make sure there are no unstaged changes before attempting an update. Bail if not. (Using `git diff --quiet`)
- [ ] Ability to update custom branches per repo
- [ ] Save settings in a `.config` file _(or something)_
- [ ] Completion of feature to update the current `HEAD` via `git rev-parse --abbrev-ref HEAD`
- [ ] Abstract to a general-use script once saved settings are implemented, allowing for easier use by people that are _not_ my coworkers :)
