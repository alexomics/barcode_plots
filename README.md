# README

---

### Requires:

```python
python>=3.6
seaborn>=0.11.1
```

### Dataset overiew:

CSV file consists of three subsets of sequencing summary files. The control is
just from the last hour of sequencing for that experiment as the experimental
conditions ("Barcodes 08 & 11", "Barcodes 09 & 10") were only run for an hour
each.

Data columns (total 11 columns):
```
 #   Column                     Dtype    Comment
---  ------                     -----    -------
 0   read_id                    object   Unique read id
 1   run_id                     object   Experiment run id
 2   start_time                 float64  Read start time offset from run start
 3   sequence_length_template   int64    Read length
 4   barcode_arrangement        object   -
 5   barcode_full_arrangement   object   -
 6   barcode_score              float64  -
 7   barcode_front_id           object   -
 8   barcode_rear_id            object   -
 9   Group                      object   Alias for experiment
 10  Sequenced                  object   Grouping var, one of {'Sequenced', 'Unblock sent'}
```
