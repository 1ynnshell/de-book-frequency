# de-novel-frequency
These frequency lists were generated from a bank of 20,000+ german e-books.

## WordRank Format

WordRank format is every word, in order of most frequent to least:
```
und
die
sie
...
```
This is the format most associated with frequency lists.

## WordFrequency Format

WordFrequency contains both the word and the number of occurrences:
```
und 4552864
die 3993582
sie 3318814
...
```
The format is `{word}{space}{occurences}`.

The inclusion of occurences allows you to edit this frequency list with your own data.
## WordJSON Format

WordJSON format is identical to WordRank, but as a JSON file:
```
["und", "die", "sie", ...]
```
This format is specially made to support the [Migaku Web Browser](https://www.migaku.io/). *I am in no way affiliated with Migaku.*

## Purpose

In order to properly score books based on their difficulty, I needed a frequency list. Unfortunately, every list I could find online were based off of Subtitles (TV-Shows, Movies), which use vastly different language than written text. 

## Drawbacks

Due to the german language, some information has been lost in the creation of this frequency list. 

1. All words were converted to lower-case. This means a `Noun`'s frequency mixes with the same `verb`'s, there is no distinction.
2. The words were not stemmed. This means that every spelling of a word is treated as it's own unique word. An example would be `verloren` vs `verlorene`. This was a conscious decision, but an important one to be aware of.

## Can I use this for {x}?

Please feel free to use this for any project. For more information please refer to `LICENSE`, or for an easier read, refer to this link about the [Apache 2.0 License](https://tldrlegal.com/license/apache-license-2.0-(apache-2.0)).

If you do use this for a project, referencing back to this repository is not mandatory but would be appreciated. I would also love to hear about it!