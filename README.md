# Graduate worker contracts and funding policies at US universities: published data

This repository holds the published data behind the [Academic Union Network](https://academic-union-network.org/)'s comparison of graduate student worker pay, contract terms and living costs across US universities. It is generated automatically whenever the data changes; please do not edit it, and send corrections to mail@academic-union-network.org instead.

## Files

- `graduate-worker-contracts-dataset/`: the research dataset: CSV tables (UTF-8) for institutions, sources, agreements, pay rates, benefit terms, bargaining-history events, cost-of-attendance lines, Fair Market Rents, citations and the figures the website charts, with a `datapackage.json` codebook (Frictionless Data Package v2) and its own README.
- `graduate-worker-contracts-dataset.zip`: the same dataset in one download.
- `graduate-worker-contracts.json`: the data the website's page reads.
- `tracker/en/` and `tracker/zh/`: the Graduate Worker Contract Tracker's pages, which https://en.academic-union-network.org/contract-tracker/ and https://zh.academic-union-network.org/contract-tracker/ serve. Like the widget file below, they are published so that the site can serve them; they are not licensed for reuse.
- `graduate-worker-contracts-widget.js`: the tracker's built code on its own, for embedding it in another page. It is published so that the page can load it; it is not licensed for reuse, and the CC0 dedication below covers the data only.

Every fact cites the document, page and passage it comes from, so each one can be checked against its source. The repository's history records every change to the published data.

## License

The data is dedicated to the public domain under [CC0 1.0 Universal](https://creativecommons.org/publicdomain/zero/1.0/). Credit is appreciated but not required: "Data: Academic Union Network, 'Graduate worker contracts and funding policies at US universities,' academic-union-network.org". The short passages quoted in `citations.csv` remain their authors' and are included only so that each fact can be verified.
