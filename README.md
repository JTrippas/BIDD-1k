# BIDD-1k

The Bard Intelligence and Dialogue Dataset (BIDD-1k) contains 1,000 anonymized prompts
collected from Google Gemini[^1] via an online crowdsourcing study.
Data collection from crowd workers was conducted with RMIT University's ethics approval between
02/01/2024 and 03/01/2024.

[^1]: Google Bard at the time of data collection.

## Data

The prompt data is provided in CSV format with session information, where session boundaries were
determined using an interval of 15 minutes. Each session is listed in ascending chronological order
in the file, for example:

```
1447,show me your new graphic feature?
1447,show me your new animations
...
1447,can you visualize this with graphics
```

shows a session where the first line is time step `t1`, the second line is time step `t2`, and so
on.

## Example Behaviours

The `examples.md` file contains some concrete examples of specific behaviour from users. Note some
of the examples may not be a part of BIDD-1k, [see the paper][jt] for further details on the
crowdsourcing data that was collected.

[jt]: https://www.johannetrippas.com/papers/trippas2024what.pdf

## Usage

If you use the `BIDD-1k`, please cite the paper:

```
@inproceedings{trippas2018informing,
 author = {Trippas, Johanne R. and Al Lawati, Sara Fahad Dawood and Mackenzie, Joel and Gallagher, Luke},
 title = {What do Users Really Ask Large Language Models? An Initial Log Analysis of Google Bard Interactions in the Wild},
 booktitle = {Proceedings of the 47th International ACM SIGIR Conference on Research and Development in Information Retrieval (SIGIR '24)},
 series = {SIGIR '24},
 year = {2024},
 location = {Washington, DC, USA},
 numpages = {5},
 doi = {10.1145/3626772.3657914},
 publisher = {ACM},
 address = {New York, NY, USA},
 keywords = {Large Language Models, Log Analysis, Prompt Analysis, Dataset}
}
```
