# Development hooks

Install Lefthook 2.2.1 or newer (`brew install lefthook` on macOS), then run
`make install-git-hooks` once per clone. The configuration is `lefthook.yml`.

The pre-commit hook checks staged Python with `python3 -m py_compile`, owned
JavaScript with `node --check`, shell scripts with `bash -n`, and staged
whitespace. Have Python 3, Node.js, and Bash on your development PATH.
Vendored and obsolete JavaScript is excluded.

These syntax checks do not start Flask, access a database, or run the test
suite. Use the commands in `tests/README.md` for application tests.
