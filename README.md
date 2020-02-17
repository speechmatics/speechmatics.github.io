# speechmatics.github.io

Source for https://speechmatics.github.io/

## How this works

This is a Jekyll project that reads the `_data/repos.yml` file and generates static webpages.
The format of `_data/repos.yml` entries is as follows:

    - `name` is used to generate the repo link, like `github.com/speechmatics/name`
    - `language` is used to display the primary language icon ([supported languages](https://konpa.github.io/devicon/))
    - `description` should be a short summary (up to 10 words) of what the repo is about
    - `pages` is a boolean indicating whether there is repo-specific [GitHub pages](https://guides.github.com/features/pages/). If set, the documentation link is generated like `speechmatics.github.io/name`

To list a new project, simply add an entry to `_data/repos.yml`.
