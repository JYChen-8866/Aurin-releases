# Aurin Releases

This public repository builds and publishes Aurin desktop installers.

It contains only release automation and public release artifacts. Aurin source
code and development history remain in a separate private repository and are
not mirrored here.

Release builds are started manually by the maintainer. The workflow reads one
explicit private source ref through a repository-scoped, read-only deploy key.
Only the packaged DMG, macOS in-app update ZIP, Windows portable EXE, Windows
setup EXE, and checksum manifests are uploaded. The setup EXE registers Aurin
in Windows' Markdown "Open with" application list without replacing the
user's current default. Aurin verifies the combined checksum manifest before
an in-app update is made available for installation.
