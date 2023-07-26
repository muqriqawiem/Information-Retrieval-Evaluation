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

## Scores of Precision@k and Average Precision

### Precision@k

#### Precision@10
| P@10 | System 1 | System 2 | System 3 | System 4 | System 5 | System 6 | System 7 | System 8 | System 9 | System 10 | System 11 | System 12 | System 13 | System 14 | System 15 |
|----------|----------|----------|----------|----------|----------|----------|----------|----------|-----------|-----------|-----------|-----------|-----------|-----------|-----------|
| 401     | 0.6     | 0     | 0     | 0.4     | 0.3     | 0.2     | 0     | 1     | 1      | 0      | 0      | 0      | 0.1      | 0.1      | 0.9      |
| 402 | 0.8 | 0.8 | 0.8 | 0.6 | 0.7 | 0.7 | 0.4 | 0.8 | 0.6 | 0.8 | 0.5 | 0.5 | 0.7 | 0.7 | 0.8 |
| 403 | 1 | 1 | 1 | 0.9 | 0.4 | 1 | 1 | 1 | 1 | 0.9 | 1 | 0.9 | 0.7 | 1 | 0.9 |
|404|0.4|0.4|0.6|0.2|0.6|0.3|0.5|0.4|0.4|0.4|0.5|0|0.3|0.4|0.6|
|405|0.2|0.6|0.3|0.3|0.6|0.4|0.5|0.4|0.6|0.4|0.5|0.4|0.6|0.4|0.6|
|406|0.4|0.6|0.6|0.5|0.6|0.6|0.6|0.3|0.4|0.5|0.5|0.3|0.6|0.4|0.4|
|407|0.2|0.8|0.9|0.9|0.9|1|0.9|0.8|0.6|0.7|0.8|0.5|0.8|1|0.7|
|408|0.2|0.3|0.3|0.2|0.7|0.4|0.4|0.3|0.7|0.6|0.4|0.4|0.3|0.5|0.9|
|409|0.4|0.3|0.2|0.1|0.5|0.2|0.3|0.5|0.4|0.3|0.4|0.2|0.1|0.3|0.6|
|410|1|1|1|1|1|1|1|1|1|1|1|1|1|1|1|
|411|0.5|0.3|0.6|0.6|0.8|0.3|0.6|0.6|0.8|0.2|0.5|0.4|0.5|0.7|0.3|
|412|0.8|0.1|0.9|0.9|0.9|0|0.6|0.9|1|0.3|0.3|0.1|0.9|0.5|0.8|
|413|0.5|0.2|0.8|0.1|0.9|1|0.6|1|0.6|0.9|0.9|0.5|0.2|0.5|0.8|
|414|0.3|0.3|0.4|0.4|0.5|0.3|0.4|0.4|0.9|0.5|0.2|0.3|0.3|0.4|0.7|
|415|1|1|1|1|1|1|1|0.9|0.8|0.9|0.9|0.9|0.9|1|1|
|416|0.4|0.2|0.3|0.3|0.9|0.3|0.5|0.6|0.4|0.3|0.3|0.5|0.5|0.4|0.8|
|417|0.6|0.5|0|0|1|0|0.8|0.3|0|0.8|0|0.1|0.9|0.4|0.5|
|418|0.7|0.7|0.8|0.8|1|0.6|0.7|0.6|0.7|0.6|0.6|0.9|0.6|0.8|0.7|
|419|0.1|0.3|0.2|0.1|0.6|0.1|0.6|0.2|0.3|0.5|0.2|0.3|0.1|0.3|0.4|
|420|0.8|0.9|0.9|0.9|0.6|0.9|0.9|0.6|0.4|0.9|0.7|0.6|0.7|0.7|0.7|
|421|0|0.3|0|0|0.3|0|0.4|0.3|0.2|0|0.2|0|0.2|0.1|0.5|
|422|0.6|0|0.8|0.5|0.9|0.8|1|0.7|0.6|0.7|0.9|0.5|0.8|0.1|0.9|
|423|0.9|0.9|0.9|0.9|0.8|0.9|0.6|0.7|0.9|0.9|0.9|0.9|0.7|0.9|0.8|
|424|0.4|0.3|0.7|0.4|1|0.7|0.6|0.5|0.9|0.3|0.6|0.1|0.7|0.5|0.8|
|425|0.9|0.8|1|1|1|1|1|0.6|1|0.9|1|0.9|0.9|0.9|0.9|
|426|0.5|0.2|0.2|0|1|0.4|0.5|0.6|0.9|0.1|0.1|0.2|0.3|0.6|0.9|
|427|0.4|0.5|0.5|0.4|0.8|0.6|0.3|0.4|0.9|0.6|0.5|0.5|0.4|0.4|0.9|
|428|0.4|0.5|0|0.2|0.9|0.4|0.2|0.2|0.7|0.1|0.6|0.3|0.2|0.3|0.8|
|429|0.5|0.1|0.4|0.3|0.7|0.2|0.1|0.5|0.4|0.3|0.3|0.4|0.3|0.3|1|
|430|0.5|0.3|0.3|0.3|0.5|0.3|0.3|0.4|0.5|0.3|0.3|0.3|0.3|0.4|0.5|
|431|0.7|0.7|0.9|0.9|0.9|0.8|0.8|0.7|0.8|0.6|0.5|0.9|0.9|1|0.7|
|432|0|0|0.2|0|0|0|0|0|0|0.2|0.1|0|0|0|0.7|
|433|0.1|0|0.1|0.2|0.1|0.1|0|0.1|0.1|0.1|0|0.2|0|0.1|0|
|434|0.9|0.3|0.7|0.6|1|0.7|1|0.7|0.8|0.8|0.7|0.9|0.7|0.6|1|
|435|0|0.6|0.5|0.6|0.9|0.4|0.4|0.3|0.4|0.4|0.5|0.3|0.3|0.2|0.7|
|436|0.4|0.5|0.9|0.8|0.8|0.5|0|0.5|1|0.4|0.5|0.2|0.6|0.3|1|
|437|0|0|0|0|0.4|0|0|0|0.2|0|0|0.1|0.1|0.1|0|
|438|0.3|0.3|0.8|0.3|0.4|0.2|0.3|0.3|0.4|0.6|0.4|0.6|0.9|0.4|0.6|
|439|0.2|0|0.2|0.2|0.4|0.1|0.1|0.2|0.4|0.2|0.2|0.1|0.2|0.1|0.9|
|440|0.6|0.5|0.8|0.7|0.7|0.7|0.5|0.5|0.8|0.3|0.5|0|0.2|0.3|0.8|
|441|0.8|0.8|0.7|0.7|0.7|0.8|0.7|0.8|0.8|0.7|0.8|0.7|0.7|0.8|0.9|
|442|0|0.2|0.2|0|0.7|0.2|0|0|0|0|0|0.1|0.1|0.1|1|
|443|0|0|0.3|0.5|0.2|0.3|0.5|0.4|0.5|0.4|0.5|0.2|0.1|0.3|0.2|
|444|0.9|1|0.9|0.9|1|0.8|0.5|0.3|0.7|0.7|0.7|0.8|0.8|0.8|1|
|445|0.4|1|0.9|0.8|1|0.9|0.9|0.5|0.9|0.8|0.7|0.7|0.5|0.3|1|
|446|0.5|0.8|0.8|0.9|0.7|0.7|0.7|0.8|0.9|0|0.2|0.4|0.8|0.3|0.9|
|447|0.5|0.1|0.1|0|0.4|0.2|0.1|0|0|0.3|0.4|0.5|0.1|0.7|1|
|448|0.1|0|0.2|0|0.6|0.1|0.3|0.2|0.3|0.2|0.2|0.1|0.4|0.2|0.2|
|449|0.4|0.5|0.4|0.5|0.4|0.4|0.4|0.4|0.5|0.2|0.5|0.2|0.4|0.3|0.6|
|450|0.9|1|1|1|0.9|0.8|1|0.9|1|0.9|0.6|0.9|0.9|0.9|0.8|
|AVG|0.474|0.45|0.54|0.476|0.692|0.486|0.51|0.502|0.602|0.47|0.472|0.416|0.486|0.476|0.722|

#### Mean Precision@10 and Mean Precision@100

|Systems|Mean Precision@10|Mean Precision@100|
|-------|-----------------|------------------|
|System 1|0.474|0.2424|
|System 2|0.450|0.2324|
|System 3|0.540|0.2702|
|System 4|0.476|0.2498|
|System 5|0.692|0.3030|
|System 6|0.486|0.2546|
|System 7|0.510|0.2772|
|System 8|0.502|0.2460|
|System 9|0.602|0.2718|
|System 10|0.470|0.2186|
|System 11|0.472|0.2196|
|System 12|0.416|0.2026|
|System 13|0.486|0.2122|
|System 14|0.476|0.2460|
|System 15|0.722|0.3440|

- Based on table, when different depth is used to calculate precision, the final result will differ.
    - All the scores for Mean P@10 are higher than P@100.
- The depth or cutoff value determines the number of retrieved items considered for calculating precision.
    - When a smaller depth is used, only a subset of the retrieved items is evaluated.
        - This can lead to a higher precision score since the focus is on a more limited set.
    - Conversely, when a larger depth is used, a larger pool of retrieved items is considered.
        - This can potentially dilute the precision as more non-relevant items are included in the calculation.

### Average Precision

#### Average Precision@100
| AP@10 | System 1 | System 2 | System 3 | System 4 | System 5 | System 6 | System 7 | System 8 | System 9 | System 10 | System 11 | System 12 | System 13 | System 14 | System 15 |
|----------|----------|----------|----------|----------|----------|----------|----------|----------|-----------|-----------|-----------|-----------|-----------|-----------|-----------|
|401|
|402|
|403|
|404|
|405|
|406|
|407|
|408|
|409|
|410|
|411|
|412|
|413|
|414|
|415|
|416|
|417|
|418|
|419|
|420|
|421|
|422|
|423|
|424|
|425|
|426|
|427|
|428|
|429|
|430|
|431|
|432|
|433|
|434|
|435|
|436|
|437|
|438|
|439|
|440|
|441|
|442|
|443|
|444|
|445|
|446|
|447|
|448|
|449|
|450|
|AVG|

#### MAP@10 and MAP@100
|Systems|MAP@10|MAP@100|
|-------|------|-------|
|System 1|0.615645|0.455366|
|System 2|0.579611|0.425485|
|System 3|0.656433|0.487752|
|System 4|0.487752|0.439029|
|System 5|0.825472|0.602349|
|System 6|0.633674|0.454345|
|System 7|0.661865|0.492832|
|System 8|0.674001|0.492043|
|System 9|0.777742|0.562690|
|System 10|0.634144|0.460350|
|System 11|0.626426|0.445300|
|System 12|0.562317|0.394284|
|System 13|0.394284|0.394284|
|System 14|0.394284|0.462806|
|System 15|0.825339|0.648299|

- Based on table, when different depth is used to calculate the mean average precision (MAP), the final result will differ.
    - All the scores for MAP@10 are higher than MAP@100.
- When calculating MAP@10, only the top 10 retrieved items are considered.
    - This leads to a more focused evaluation.
    - Can highlight the system's ability to retrieve relevant items within a smaller subset, potentially resulting in higher scores.
- However, MAP@100 takes into account a larger pool of retrieved items.
    - Includes more non-relevant items, which can impact the overall average precision score.
