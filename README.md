# Fuzzy Join JSON Dataset

This repository provides a **synthetic dataset for benchmarking fuzzy joins over JSON collections**, with controlled variations in **schema**, **nesting**, and **noise**. It is intended to evaluate join methods that go beyond strict structural matching; e.g., approaches based on semantic representations (embeddings) or robust token/structure features.

## Repository contents

- `collectionA.jsonl.zip`  
  Baseline JSON collection **A** (one JSON document per line).

- `collectionB_same_schema.jsonl.zip`  
  Collection **B** where documents are intended to be comparable to A under **the same schema** (schema-aligned setting).

- `collectionB_diff_schema.jsonl.zip`  
  Collection **B** where comparable documents may use a **different schema** than A (e.g., key renaming, different nesting/layout).

- `collectionB_mixed_schemas.jsonl.zip`  
  Collection **B** combining multiple schema regimes (a mixture of schema-aligned and schema-divergent documents).

- `collectionB_noise.jsonl.zip`  
  Collection **B** with additional **noise** injected (e.g., distracting fields/values, minor perturbations), intended to stress robustness.

- `join_ground_truth.jsonl.zip`  
  Ground-truth join signal (gold standard) describing which cross-collection pairs should be considered matches under the dataset’s similarity assumptions.

> All datasets are provided as **zipped JSON Lines** (`.jsonl.zip`): each line is an independent JSON object (or record).

