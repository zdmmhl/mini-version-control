# Mini Version Control

A Python implementation of a limited snapshot-based version-control command set.

## Supported commands

`mygit-init`, `mygit-add`, `mygit-commit`, `mygit-log`, `mygit-show`, `mygit-rm`, `mygit-status`, `mygit-branch`, `mygit-checkout`.

Run commands with Python from a disposable working directory, for example `python /path/to/mygit-init`. They create and modify `.mygit` and working files.

Merge is not implemented. The historical marking log reports 28 passed and 6 failed tests, with missing `mygit-merge` affecting the failed cases. This log is not a fresh verification result and the test suite is not bundled.


## Provenance

Originated in UNSW COMP9044. The command implementations are included; original marking tests and standard answers are not. No complete Git compatibility is claimed.

## Verification status

A disposable-workspace smoke check passed on 8 October 2026: init/add/commit/show, branch creation and switching, a second commit and restoration of the first snapshot. Branch metadata is initialized lazily by `mygit-branch`, using `trunk` as the default. The original full marking suite was not rerun.
