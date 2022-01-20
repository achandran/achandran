# Software Engineering Toolkit

## Languages:
[Python](https://www.python.org/) when possible. Often performance limitations
can be handled via _good algorithm selection_, and careful _use of the standard
library_/other _libraries that use C_ under the hood. If not possible to reach
needed performance via Python, look at Go or C.

Domains where alternative languages might be a better choice:
- __Web Frontends__ (SPAs) via Javascript (though see tools like HTMX to add
  reactivity without much JS)
- __Mobile Apps__ (Swift for iOS, Java for Android).

## Python:
- [poetry](https://github.com/python-poetry/poetry) to install dependencies and handle virtual environments.
- [pyenv](https://github.com/pyenv/pyenv) to manage different versions of python, and avoid using the system python.
- [pipx](https://github.com/pypa/pipx) to install and run standalone python cli applications.

### Python Libraries:
- [Django](https://github.com/django/django) for full-featured backends.
- [Django Ninja](https://github.com/vitalik/django-ninja) for adding APIs to Django.
- [FastAPI](https://github.com/tiangolo/fastapi) for standalone/simple APIs.
- [Pydantic](https://github.com/samuelcolvin/pydantic) for data validation.
- [HTTPX](https://github.com/encode/httpx) for making HTTP requests.
- [Pytest](https://github.com/pytest-dev/pytest) for testing.
- [htmx](https://htmx.org/) for reactive web UIs without javascript single-page apps.
- [Hypothesis](https://github.com/HypothesisWorks/hypothesis) for property-based testing/fuzzing.
- [Boto3](https://github.com/boto/boto3) for interacting with AWS.
- [Pandas](https://github.com/pandas-dev/pandas) for data analysis/manipulation.
- [Numpy](https://github.com/numpy/numpy) for scientific computing.
- [Dash](https://github.com/plotly/dash) for data visualization via web apps.
- [Datasette](https://github.com/simonw/datasette) for data exploration/publishing.
- [Scrapy](https://github.com/scrapy/scrapy) for web crawling/scraping.
- [BeautifulSoup](https://pypi.org/project/beautifulsoup4/) for HTML parsing.
- [Pillow](https://github.com/python-pillow/Pillow) for image manipulation.
- [Pygame](https://github.com/pygame/pygame) for 2d games.
- [Rich](https://github.com/willmcgugan/rich) for rich text formatting in terminals.
- [Textual](https://github.com/willmcgugan/textual) for TUIs (text-based user interfaces).
- [Ortools](https://github.com/google/or-tools) for combinatorial optimization algorithms.
- [ScikitLearn](https://github.com/scikit-learn/scikit-learn) for machine learning.
- [PyTorch](https://github.com/pytorch/pytorch) for deep learning.

## Data:
- [PostgreSQL](https://github.com/postgres/postgres) as default option.
- [sqlite](https://github.com/mackyle/sqlite) for simpler projects.
- [redis](https://github.com/redis/redis) as cache layer if needed.
- JSON as interchange format.

## Tools:
- [Pycharm](https://www.jetbrains.com/pycharm/) as primary editor.
- [neovim](https://github.com/neovim/neovim) for quick edits.
- [git](https://github.com/git/git) for source control.
- unix tools combined with pipes (`|`) to process text generally (`awk`, `sed`, `wc`, `grep`, `tr`, `diff`, `uniq`,
  `sort`, `cut`, `cat`, `head`, `tail`)
- [ripgrep](https://github.com/BurntSushi/ripgrep) as an improvement to `grep`.
- [fd](https://github.com/sharkdp/fd) as an improvement to `find`.
- [jq](https://github.com/stedolan/jq) to parse and process JSON.
- [iterm](https://iterm2.com/) terminal emulator.
- [zsh](https://www.zsh.org/) shell.

## Problem Solving:
- Chunk functionality together, as our working memories can handle roughly [seven](https://en.wikipedia.org/wiki/The_Magical_Number_Seven,_Plus_or_Minus_Two) items.
- Solve a related, but simpler problem.
- State the problem clearly, and then develop incrementally.
- Repeat tasks manually until patterns emerge and functions discover themselves.
- Build classes independently and let inheritance discover itself.
- Consider data structures programming as a graph-traversal problem, traveling from one "island" to another to use
  appropriate functionality. (strings -> lists -> dictionaries etc.)
- Separate ETL (extract-transform-load) from analysis. Separate analysis from presentation.
- Verify type and size of the data. View and test a subset of the data.
- Humans should never gaze upon unsorted data.

 *Adapted from The Mental Game of Python Talk given by Raymond Hettinger
  at PyBay2019*
