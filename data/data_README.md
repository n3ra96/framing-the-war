# Data

Due to size and licensing constraints, raw data files are not included in this repository.

## Tweet Corpus

Collect tweets by running **Module 1** of the notebook with your own X API Bearer Token.

**Politicians and their X user IDs:**
| Politician | Handle | User ID |
|---|---|---|
| Benjamin Netanyahu | @netanyahu | 17061263 |
| Yair Lapid | @yairlapid | 2946300174 |
| Benny Gantz | @gantzbe | 1082167187006242817 |
| Bezalel Smotrich | @bezalelsm | 3185280620 |
| Itamar Ben Gvir | @itamarbengvir | 716347920287678464 |

**Date range used in this study:** March 4, 2024 → April 19, 2026  
**Estimated cost:** ~$17 in X API credits

## Conflict Data (ACLED)

1. Register for a free account at [acleddata.com](https://acleddata.com)
2. Navigate to the Data Export Tool
3. Download the **Middle East aggregated dataset**
4. Upload it when prompted in Module 5 of the notebook

## Output Files (Google Drive)

After running the full pipeline, the following files will be in your Google Drive under `pol_discourse/`:

| File | Description |
|---|---|
| `corpus.parquet` | Raw tweets |
| `corpus_annotated.parquet` | GPT-4o annotated tweets |
| `sample_annotated.parquet` | 200-tweet annotation sample |
| `validation_sample.csv` | Human validation annotations |
| `acled_israel.parquet` | Israel conflict events |
| `acled_weekly.parquet` | Weekly Israel conflict summary |
| `acled_gaza_weekly.parquet` | Weekly Gaza conflict summary |
| `master_weekly.parquet` | Merged tweet + conflict data |
| `master_weekly_expanded.parquet` | Merged with all 6 fronts |
| `granger_results.csv` | Original Granger results |
| `granger_all_fronts.csv` | Full multi-front Granger results |
