# Utilities to work with Survey Solutions API


## Generate SQL database from the (Tabular) file export

call it from the command line:
```shell
python ./tabular_to_sql.py ./example_1_Tabular.zip
```

or in your script:
```python
import tabular_to_sql

tabular_to_sql.convert("example_1_Tabular.zip",  "sqlite:///example_1.db", "quest.json")
```

## Download export file and generate SQL database

```shell
python ./get_export.py --url 'https://demo.mysurvey.solutions' --username api_user --password pass1234
```

- Note : before with https://github.com/vlasvlasvlas/survey-solution-api-massive-export

- Note : changes were made into requirements.txt and install process (changes in new req.txt)

pip install --force-reinstall 'sqlalchemy<2.0.0'

pip install --force-reinstall 'tqdm<4.52.1'
