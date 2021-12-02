# to start working with great expectation
pip install great_expectations

JFI (not need to run for this project)
great_expectation --v3-api init (this commnd is used to create a new project with great expectations)

# to create new suite
1) great_expectation --v3-api suite new
2) select 3d option, to generate expectations automatically, using a profiler
![image](https://user-images.githubusercontent.com/66337412/144492370-e2a7b6d8-d313-43a8-8e53-fc022e2d15db.png)
3) select data_asset
4) and give name to the Expectation suite

# to edit existing suite
For homework purpose prod_suite was created. To observe it or edit and run use the following command:
 1) great_expectation --v3-api suite edit prod_suite
 2) run all cells in opened Jupyter notebook

Jupyter notebook itself stored in /uncommited/edit_prod_suite.ipynb
Created Expectations Suite is stored as json file in /expectations.prod_suite.json

# Data Docs (report to validate results of ExpectationSuite execution)
Data Docs can be viewed from /uncomitted/validations/data_docs/local_site/index.html
or
it will be opened automatically after running notebook with Expectations
![image](https://user-images.githubusercontent.com/66337412/144494296-5b12b031-0698-455a-a06a-a7972cb4bcd7.png)

# checkpoint creation
To create checkpoint run the command:
1) great_expectation --v3-api checkpoint new <checkpoint_name>
2) created checkpoints are stored in /checkpoints/<checkpoint_name>.yml
3) to run existing checkpoints execute great_expectation --v3-api checkpoint run hw_checkpoint
