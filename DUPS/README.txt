The DUPS (Diachronic Usage Pair Similarity) dataset contains similarity judgements of English word usage pairs from different time periods, as described in:

Mario Giulianelli, Marco Del Tredici, and Raquel Fernández. 2020. Analysing Lexical Semantic Change with Contextualised Word Representations. In Proceedings of the 58th Annual Meeting of the Association for Computational Linguistics (ACL-2020). Association for Computational Linguistics.


The annotations are available in two formats: full.csv and aggregate.csv. In full.csv, each annotation item is listed individually. In aggregate.csv, annotations are aggregated per usage pair. Annotations were collected using the Figure Eight (now Appen) crowdsourcing platform.


These are the fields in full.csv. For further information about usage sentences, clusters and time intervals, please refer to the paper above.

- _unit_id: a unique ID number identifying this usage pair
- lemma: the lemma for which this usage pair was annotated
- a: the first usage of the lemma (in a sentence)
- b: the second usage of the lemma (in a sentence)
- time_a: the time interval to which the first usage sentence belongs
- time_b: the time interval to which the second usage sentence belongs
- cluster_a: the K-Means cluster to which the first usage belongs
- cluster_b: the K-Means cluster to which the second usage belongs
- id_a: the (lemma-specific) identifier of the first usage
- id_b: the (lemma-specific) identifier of the second usage
- sim_score: the usage similarity score assigned to the two usages
- cannot_decide_reason: a comment by the annotator describing why annotating this usage pair was difficult
- _created_at: the time the contributor submitted the judgement
- _id: a unique ID number generated for this specific judgment
- _started_at: the time at which the contributor started working on the judgement
- _tainted: this will be "true" if the contributor has been flagged for falling below the required accuracy - in that case, this judgment will not be used in the aggregation
- _channel: the work channel that the contributor accessed the job through
- _trust: the contributor's accuracy (as defined by Figure Eight)
- _worker_id: a unique ID number assigned to the contributor
- _country: the country the contributor is from
- _region: a region code for the area the contributor is from
- _city: the city the contributor is from


These are the fields in aggregate.csv. For further information about usage sentences, clusters and time intervals, please refer to the paper above.

- _unit_id: a unique ID number identifying this usage pair
- lemma: the lemma for which this usage pair was annotated
- a: the first usage of the lemma (in a sentence)
- b: the second usage of the lemma (in a sentence)
- time_a: the time interval to which the first usage sentence belongs
- time_b: the time interval to which the second usage sentence belongs
- cluster_a: the K-Means cluster to which the first usage belongs
- cluster_b: the K-Means cluster to which the second usage belongs
- id_a: the (lemma-specific) identifier of the first usage
- id_b: the (lemma-specific) identifier of the second usage
- sim_score: the list of usage similarity scores collected for a usage pair
- cannot_decide_reason: a comment by the annotator describing why annotating this usage pair was difficult
- _trusted_judgments: the number of non-tainted judgment the row has accumulated
- _last_judgment_at: the time the latest judgment was received
