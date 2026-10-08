# Storage model

The implementation stores an index and numbered commit snapshots under `.mygit`, records messages and branch references, and compares tracked working files during checkout.

It is a teaching model: storage is directory-based, merge is absent, and behaviour is not claimed to match real Git across all edge cases.
