# Release notes

## New in git-machete 2.5.5

- fixed: behavior of `discover` in a repository where no local branches exist (e.g. a newly-created one)

## New in git-machete 2.5.4

- improved: fetching the list of local branches

## New in git-machete 2.5.3

- fixed: upstream inference crashing for branches whose reflog is empty (due to e.g. expiry)

## New in git-machete 2.5.2

- added: link to the new blog post in README.md

## New in git-machete 2.5.1

- fixed: various issues with `help` subcommand, esp. when run for an alias

## New in git-machete 2.5.0

- added: `discover` is the new name for `infer` subcommand
- added: `l` is an alias for `log`
- deprecated: `infer` subcommand (retained for backward compatibility)
- improved: README

## New in git-machete 2.4.6

- improved: `infer` now works faster for large repositories

## New in git-machete 2.4.5

- fixed: corner cases in algorithm for computing fork point of a given branch

## New in git-machete 2.4.4

- fixed: `prune-branches` crashing when deleting a branch merged to HEAD but not to its remote tracking branch

## New in git-machete 2.4.3

- improved: `status` now works faster for large repositories

## New in git-machete 2.4.2

- updated: repository url in README.md
- removed: unused install.sh script

## New in git-machete 2.4.1

- fixed: use apostrophes instead of backticks in user-facing messages to comply with git's conventions

## New in git-machete 2.4.0

- improved: `show up`, `go up` and `update` use inferred parent branch if the current branch isn't managed

## New in git-machete 2.3.0

- added: `log` subcommand

## New in git-machete 2.2.0

- added: `first` and `last` params to `go` and `show` subcommands

## New in git-machete 2.1.2

- fixed: some initial `git` commands were skipped from logs when `--verbose` flag was passed
- fixed: faster validation of branches included in the definition file

## New in git-machete 2.1.1

- fixed: Makefile commands for install/uninstall

## New in git-machete 2.1.0

- added: `anno` subcommand

## New in git-machete 2.0.1

- fixed: `prune-branches` crashing when the currently checked-out branch was unmanaged

## New in git-machete 2.0.0

- added: `infer` subcommand
- added: `show` subcommand
- added: `list` subcommand has new category `slidable-after`
- improved: `add` subcommand behavior, including inference of desired upstream when possible
- improved: remote sync-ness information displayed by `status` (now corresponds to how git tracks remote counterparts)
- removed: `down`/`next`/`prev`/`root`/`up` subcommands
- removed: `-r`/`--remote` option to `status` and `traverse` subcommands

## New in git-machete 1.5.0

- improved: branch name completion in shell
- added: `list` subcommand (mostly for internal use of branch name completion)

## New in git-machete 1.4.0

- added: `traverse` subcommand that semi-automatically syncs the entire branch dependency tree

## New in git-machete 1.3.1

- added: extra checks for indent errors in the definition file 

## New in git-machete 1.3.0

- added: custom annotations (e.g. PR number) allowed next to branch name in the definition file

## New in git-machete 1.2.0

- changed: allow to specify multiple branches when doing a `slide-out`

## New in git-machete 1.1.0

- changed: loosen requirements for `diff`, `fork-point` and `reapply` commands

## New in git-machete 1.0.2

- fixed: some `git machete` subcommands crashing when run from within a submodule

## New in git-machete 1.0.1

- fixed: some `git machete` subcommands crashing when run during an ongoing merge or rebase

