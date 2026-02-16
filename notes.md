## Day 1

Imported dataset
Looked at: 
    - shape()
    - info()
    - describe()

### Nulls & Duplicates

#### Nulls

    - Several columns appear to contain missing data. Need to verify weather that's true or not
        - age 
        - job
        - marital
        - education 
        - default 
        - housing 
        - loan
        - cons.price.idx
        - euribor3m
        - date

Those categorical columns whose null % is less than 10% I've decided to put as unknown instead of Nan