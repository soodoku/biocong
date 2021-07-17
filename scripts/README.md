## Parse name

### Parse the member of congress name

Using https://github.com/appeler/clean-names to extract first name to new column.

```
python process_names.py ../biocong/data/biocong-cleaned.csv -c name -a -o ../data/biocong-cleaned-parse-name.csv

python process_names.py ../biocong/data/biocong-text-all-cleaned.csv -c name -a -o ../data/biocong-text-allcleaned-parse-name.csv
```

### Parse children first name

Using this [notebook](extract_children_first_name.ipynb)
