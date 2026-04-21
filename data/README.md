# Data

## HuggingFace Datasets
The following datasets are loaded directly from HuggingFace using the `datasets` library:

- `andreagasparini/dreaddit` — train, test
- `solomonk/reddit_mental_health_posts` — train
- `AIMH/SWMH` — train, validation, test
- `hugginglearners/reddit-depression-cleaned` — train

```python
from datasets import load_dataset
from huggingface_hub import login
import os

login(token=os.getenv("HF_TOKEN"))

dreaddit = load_dataset("andreagasparini/dreaddit")
solomon  = load_dataset("solomonk/reddit_mental_health_posts")
swmh     = load_dataset("AIMH/SWMH")
depres   = load_dataset("hugginglearners/reddit-depression-cleaned")
```
