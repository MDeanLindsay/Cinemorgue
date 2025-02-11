# Cinemorgue

A notebook parsing a wikimedia file from Cinemorgue to extract actor/actress names and movie titles.

## Description

Cinemorgue is an encyclopedia that is dedicated to documenting which actors or actresses "died" in which movie or TV show. Having started as a separate website, the documentation effort proved to be too big a job for one person, so the wiki was born where everyone is allowed to submit their additions and corrections directly.

So if you've ever wondered "Has so-and-so ever done a death scene?" or "What's that movie where what'sisname kills such-and-such?", then this index will strive to answer those questions.

This notebook will produce a csv from their .xml export, and only focuses on movies. It will contain actor name, movie title, year, and a cause of death. 

If you are just looking for the cleaned data, it's in the output folder!

### Prerequisites

Make sure you have UV installed. You can install it using pip:

```sh
pip install uv
```

The project requires Python 3.9. You have two options:

1. Using pyenv (recommended for managing Python versions):
```sh
# Install and set Python 3.9 as the project version
pyenv install 3.9
pyenv local 3.9
```

2. Without pyenv:
   - Manually install Python 3.9 from python.org
   - Ensure `python --version` shows 3.9.x before proceeding

### Installation

1. Download the "Current Pages" xml dump at the bottom of the page from https://cinemorgue.fandom.com/wiki/Special:Statistics. 
Add the file to the root of the directory.

2. Clone the repo
   ```sh
   git clone https://github.com/MDeanLindsay/Cinemorgue.git
   cd Cinemorgue
   ```

3. Create and activate virtual environment
   ```sh
   uv venv
   source .venv/bin/activate  # On Unix/MacOS
   # OR
   .\.venv\Scripts\activate   # On Windows
   ```

4. Install dependencies
   ```sh
   uv pip install -r requirements.lock
   ```

### Development

If you need to update dependencies:

1. Edit `requirements.txt` to add/remove packages
2. Generate new lock file:
   ```sh
   uv pip compile requirements.txt -o requirements.lock
   ```
3. Install from new lock file:
   ```sh
   uv pip install -r requirements.lock
   ```

### Running the Notebook

After installation, start Jupyter Lab:
```sh
jupyter lab
```

Open `Cinemorgue.ipynb` to get the party started.