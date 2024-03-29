# Cinemorgue

A notebook parsing a wikimedia file from Cinemorgue to extract actor/actress names and movie titles.

## Description

Cinemorgue is an encyclopedia that is dedicated to documenting which actors or actresses "died" in which movie or TV show. Having started as a separate website, the documentation effort proved to be too big a job for one person, so the wiki was born where everyone is allowed to submit their additions and corrections directly.

So if you've ever wondered "Has so-and-so ever done a death scene?" or "What's that movie where what'sisname kills such-and-such?", then this index will strive to answer those questions.

This dataset is parsed from their .xml export, and only focuses on movies. The dataset consists of two columns: the actor name and the title of a film they've died in. All other dates, death descriptors, and character names have been dropped due to reliability issues.

### Prerequisites

Make sure you have venv installed.

* venv
  ```py
  pip install venv
  ```

### Installation

1. Download the "Current Pages" xml dump at the bottom of the page from https://cinemorgue.fandom.com/wiki/Special:Statistics. Unzip the .7z however you see fit.

2. Clone the repo
   ```sh
   git clone https://github.com/MDeanLindsay/Cinemorgue.git
   ```
3. Create venv.
   ```sh
   python3 -m venv .venv
   ```
4. Initialize venv.
   ```sh
   .\.venv\Scripts\bin\activate
   ```
5. Install requirements.
   ```sh
   pip install -r requirements.txt
   ```
