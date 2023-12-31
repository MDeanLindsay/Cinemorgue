# Cinemorgue

A notebook parsing a wikimedia file from Cinemorgue to extract actor/actress names and movie titles.

## Description

Cinemorgue is an encyclopedia that is dedicated to documenting which actors or actresses "died" in which movie or TV show. Having started as a separate website, the documentation effort proved to be too big a job for one person, so the wiki was born where everyone is allowed to submit their additions and corrections directly.

So if you've ever wondered "Has so-and-so ever done a death scene?" or "What's that movie where what'sisname kills such-and-such?", then this index will strive to answer those questions.

This dataset is parsed from their .xml export, and only focuses on movies. The dataset consists of two columns: the actor name and the title of a film they've died in. All other dates, death descriptors, and character names have been dropped due to reliability issues.

## Getting Started

### Dependencies

* py 3.11.4

### Executing program

```
./Scripts/activate
jupyter notebook
```

## Version History

* 0.1
    * Initial Release

