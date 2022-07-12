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
3. Run 1 and 2 only ONCE. never run it again!
4. import new data by:
```{r}
pls_long <- readRDS(file="../data/PLS_long.dta")
bit_long_par <- readRDS(file="../data/BIT_long_par.dta")
bit_long_father <- readRDS(file="../data/BIT_long_father.dta")
bit_long_mother <- readRDS(file="../data/BIT_long_mother.dta")
media_data <- readRDS(file="../data/media_data.dta")
demography <- readRDS(file="../data/demography.dta")

pls_wide <- readRDS(file="../data/PLS_wide.dta")
bit_wide <- readRDS(file="../data/BIT_wide.dta")
```

## what does those data means?

- **BIT_long_par**  include ONLY **BITSEA** scores in all waves (avg score of parents)
- **BIT_long_father**  include ONLY **BITSEA** scores in all waves (of father)
- **BIT_long_mother**  include ONLY **BITSEA** scores in all waves (of mother)
- **PLS_long**  include include ONLY **PLS** scores in all waves
- **Media**  include include ONLY  **media info** media data in all waves **has only media from wave 1 for now**
- **Demographic dataset** include ONLY demography (assuming that it doesn't change)
