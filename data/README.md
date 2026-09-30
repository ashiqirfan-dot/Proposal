# data/ — confidential, not tracked by git

Everything in this folder is ignored by git (see `.gitignore`), so it never
leaves your machine.

| Folder     | Put here                                                        |
|------------|-----------------------------------------------------------------|
| `input/`   | Technical design PDFs (one per project)                          |
| `pricing/` | Product price list (Excel/CSV) and discount rules               |
| `output/`  | Generated commercial proposals                                  |

Before committing, run `git status` and confirm no file from this folder is listed.
