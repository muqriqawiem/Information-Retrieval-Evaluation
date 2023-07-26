# Information Retrieval Evaluation

## Project Background
  - Evaluate the performance of a set of search engine systems using a collection of input files simulating ranked documents.
  - Use relevance judgment files (qrels) from the TREC website to compute evaluation scores for each system using the metrics precision@10 and mean average precision (MAP).
    - Analysis includes:
        - Computing per system-per topic scores
        - Averaging these scores to compute overall precision@10 and MAP scores for each system
        - Performing correlation coefficient and significance testing on these system scores
    - Allows us to compare the similarity of system performance rankings when using different evaluation metrics and assess the significance of differences between pairs of systems.
