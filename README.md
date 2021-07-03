## Congressional Biographies


## 97th ---  104th Congress

We use text from the [pdfs](https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/NZPPJM) (downloaded from Google Books, from where these are freely available) and then parse the text.

### Scripts

1. [parse](scripts/parse-biocong-from-text-all.ipynb)
2. [clean](scripts/clean-biocong-from-text-all.ipynb)

## 105th --- 115th Congress

We scrape congressional biographies for 105th to the 115th Congress from the [Congressional Directory](https://www.govinfo.gov/app/collection/cdir/). We download the biographical files, e.g.,  https://www.govinfo.gov/content/pkg/CDIR-2018-10-29/html/CDIR-2018-10-29-STATISTICALINFORMATION-2.htm and parse them to extract information such as birthdate, number of children, education, etc.  

### Scripts

1. [Scrapes the Congressional Directory](scripts/biocong.ipynb) produces [biocong.csv](data/biocong.csv), [biocong-browsepath.csv](data/biocong-browsepath.csv), and [html files (tar.gz)](data/cong_bio_1997_2018.tar.gz) 
2. [Download Congressional Biographies Using the API](scripts/biocong-api.ipynb) provides the script for downloading the data using the API. (It produces incomplete data so we don't use this script.)
3. [Parse](scripts/03_parse-biocong.ipynb) iterates through biocong-browsepath.csv and parses the [html files (tar.gz)](data/cong_bio_1997_2018.tar.gz) and produces [biocong-parsed.csv](data/biocong-parsed.csv)
4. [Clean](scripts/04_clean-biocong.ipynb) takes biocong-parsed.csv produces [biocong-cleaned.csv](data/biocong-cleaned.csv)

### Data

The final dataset---[biocong-cleaned.csv](data/biocong-cleaned.csv)---has the following columns: 

```
'level', 'docCount', 'browsePath', 'title', 'lastpage', 'granuleid', 'packageid', 'pdffile', 'pdf', 'text',
 'agencyLevel', 'nodeStatus', 'textfile', 'htmlfile', 'browseline1', 'processingcode', 'nodetype', 'index.1', 
 'publishdate', 'part', 'forGpo', 'hasChildren', 'hasParents', 'rootNode', 'documentResults', 'hasDocumentResults',
 'collectionCode', 'searchPath', 'isContentArea', 'pageSize', 'pageNumber', 'count', 'digitizedFR', 'section',
 'firstpage', 'congress', 'biography', 'name', 'party', 'location', 'born_in', 'birthdate', 'education', 'professional', 
 'married', 'children', 'committees', 'url', 'n_children'
```
