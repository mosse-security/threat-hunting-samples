# Introduction

With this Github repository, Mossé Cyber Security Institute offers you three (3) datasets to practice Threat Hunting.

The datasets contain forensics data for 25, 50 and 75 machines respectively. The answers for dataset 1 have been provided for learning purposes. It will be up to you to discover which machines have been compromised for the other two dataset. We have included how many machines in total per dataset have been attacked.

# Installation

Install Python, and then do `python -m pip install -r requirements.txt`.

We recommend you use `Python 3.6` as some people have reported issues getting `Pyarrow` working on `3.7`.

# Reading the Datasets

```Python
import pandas as pd
import pyarrow as pa
import pyarrow.parquet as pq

dataset = pq.ParquetDataset('dataset-1/w32services/')
table = dataset.read()
w32services = table.to_pandas()
```

# Contact Us

We invite you to contact us if you have any questions or would like to report errors with the datasets. Our email is contact@mosse-security.com

Have fun!