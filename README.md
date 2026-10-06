# EPSS Data

Daily bulk EPSS score snapshots published by the FIRST EPSS SIG.

## Layout

- `metadata.json`: latest snapshot metadata, record count, model version, and SHA-256 checksum.
- `snapshots/YYYY/epss_scores-YYYY-MM-DD.csv.gz`: source CSV gzip preserved without transformation.

Each CSV contains the source fields `cve`, `epss`, and `percentile`. Scores and
percentiles are copied directly from FIRST; this repository does not calculate
or infer EPSS values.

Source: <https://www.first.org/epss/data.html>
