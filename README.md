# Education-3
Scientific Goal: Find the relationship between media habits on language and social emotional skills development.

data dictionary:

data collection approaches: 

# PROJECT NOTES

- Store all data inside folder `data`
```
Education-3
├── data
│   ├── wave-1-(9-mo)
│   ├── wave-2-(12-mo)
│   ├── wave-4-(18-mo)
│   └── wave-6-(24-mo)
└── README.md
```

# How to get cleaned data

1. open `./01-week-code/eda.Rmd` and run all chunk
2. open `./02-week-code/clean-new-data-jul7.Rmd` and run all chunk
3. import new data by:
```{r}
PLS_data <- readRDS(file="../data/PLS_data.dta")
BIT_data <- readRDS(file="../data/BIT_data.dta")
media_data <- readRDS(file="../data/media_data.dta")
demography <- readRDS(file="../data/demography.dta")
```

## what does those data means?

- **BITSEA**  include all **BITSEA** include ONLY BITSEA scores in all waves
- **PLS**  include all **PLS**  include ONLY PLS scores in all waves
- **Media**  include all **media info** without include ONLY media info in all waves **has only media from wave 1**
- **Demographic dataset** include ONLY demography (assuming that it doesn't change)
