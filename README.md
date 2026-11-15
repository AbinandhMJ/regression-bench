# Regression Bench

Does a code review tool notice when a pull request quietly undoes a real bug fix?

This repository holds 33 real bug fixes from 11 open-source projects. For each one, `cases/<case>/` has the file as it was **before** the fix, then the fix itself as its own commit with the original message and author. Then two pull requests per case change the file again. Some undo the fix, some don't. Reviewers see the full history.

Built by [fixlock](https://abinandhmj.github.io/fixlock/regression-bench) (a product of Algotricz) to compare tools on the same cases. Method and results: https://abinandhmj.github.io/fixlock/regression-bench

Please don't merge the pull requests: they are the test cases.

## Sources and licenses

Each file is copied from its project at a pinned commit and remains under that project's license, included in `licenses/`. Changes: the files were moved under `cases/`, and the pull requests edit them as described above.

- **express**: https://github.com/expressjs/express at `43fca52` (license in `licenses/express/`)
- **ky**: https://github.com/sindresorhus/ky at `3541888` (license in `licenses/ky/`)
- **requests**: https://github.com/psf/requests at `3c7baaa` (license in `licenses/requests/`)
- **cobra**: https://github.com/spf13/cobra at `adbc881` (license in `licenses/cobra/`)
- **gson**: https://github.com/google/gson at `d938a10` (license in `licenses/gson/`)
- **okhttp**: https://github.com/square/okhttp at `b6e74e5` (license in `licenses/okhttp/`)
- **ripgrep**: https://github.com/BurntSushi/ripgrep at `178cc02` (license in `licenses/ripgrep/`)
- **rack**: https://github.com/rack/rack at `da90464` (license in `licenses/rack/`)
- **guzzle**: https://github.com/guzzle/guzzle at `f8aca40` (license in `licenses/guzzle/`)
- **Newtonsoft.Json**: https://github.com/JamesNK/Newtonsoft.Json at `52fa3ae` (license in `licenses/Newtonsoft.Json/`)
- **Alamofire**: https://github.com/Alamofire/Alamofire at `dea4bab` (license in `licenses/Alamofire/`)
