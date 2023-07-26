# Information Retrieval Evaluation

## Project Background
- Evaluate the performance of a set of search engine systems using a collection of input files simulating ranked documents.
- Use relevance judgment files (qrels) from the TREC website to compute evaluation scores for each system using the metrics precision@10 and mean average precision (MAP).
  - Analysis includes:
    - Computing per system-per topic scores
    - Averaging these scores to compute overall precision@10 and MAP scores for each system
    - Performing correlation coefficient and significance testing on these system scores
  - Allows us to compare the similarity of system performance rankings when using different evaluation metrics and assess the significance of differences between pairs of systems.

## Systems to be Evaluated
- System 1 = acsys8alo2
- System 2 = apl8ctd
- System 3 = att99atdc
- System 4 = att99ate
- System 5 = CL99XTopt
- System 6 = Flab8as
- System 7 = fub99td
- System 8 = GE8ATDN1
- System 9 = GE8MTD2
- System 10 = ibms99c
- System 11 = INQ602
- System 12 = mds08a2
- System 13 = Mer8Adtd4
- System 14 = nttd8alx
- System 15 = orcl99man

## Scores of Precision @ k and Average Precision

### Precision@k
| P@10 | System 1 | System 2 | System 3 | System 4 | System 5 | System 6 | System 7 | System 8 | System 9 | System 10 |
|----------|----------|----------|----------|----------|----------|----------|----------|----------|-----------|-----------|-----------|-----------|-----------|-----------|-----------|
| Data     | Data     | Data     | Data     | Data     | Data     | Data     | Data     | Data     | Data      | Data      | Data      | Data      | Data      | Data      | Data      |
