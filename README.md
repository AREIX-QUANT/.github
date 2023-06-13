# Areix Quant Dev


## Language
Python should be used as the programming language to complete the capstone project. Either python script or jupyter notebook can be used.

We would recommend you to use Jupyter Notebook for DC/DM/DV (Data Collection / Data Management / Data Visualization). It is a powerful way to write and iterate on your Python code for data analysis. Rather than writing and re-writing an entire program, you can write lines of code and run them one at a time, the data is stored in the memory which allows you to reuse it.

**Further reading:**

http://docs.python-guide.org/en/latest/

## Style and linting
Follow the Python Style Guide (PSG) as formulated in PEP-8: http://www.python.org/dev/peps/pep-0008/


The critical points has been summarized below:

- Code Lay-out
    - Use spaces; never use tabs
    - 4 space indentation
    - 79 character line limit
        - use Backslashes `\` to separate the line
- Naming Conventions
    - Avoid using pre-defined words
        - E.g. ❌ `type = 'fintech'`
        - ✅ `type_ = 'fintech'`
        - in python, type is a function to return class type of the object
    - Variables, functions and methods should be `lower_case_with_underscores`
    - Constants are `CAPTIALIZED`
    - Classes are `TitleCase`
    - In classes, private varabile should be `_like_this`

And other preferences:

- All python code should be written to support Python3
- Use ' and not " as the quote character by default
- Error handling is important
- Memory and runtime management
    - Despite the GC (Grabage Collection), try to optimize your code through suitable data structure and algorithm
    - Use function for code re-use
    - Use class for method and variable encapsulation
- Follow the OOP (Object-oriented programming) priciples
- Use pylint to lint code (Optional)


The [python porting guide](https://docs.python.org/3/howto/pyporting.html) has great, practical advice on writing code for Python3.


## Version control
The git will be use for version control and source code management through out the project.

For those don't have experience in Git, we would highly recommend you to use [Github Destop](https://desktop.github.com/), a Graphical User Interface for GitHub.

Standard to follow:

1. Remember to checkout(switch) the branch to develop branch first before push/pull the code
    - Never commit directly to `master`
    - Always work from `develop branch` that is checked out from `master`
    - The `master` will only be used once the project is completed and we will merge the `develop branch` to `master`
2. Always pull the repository every time before push your work
3. Properly describe changes in commit messages
    - Clearly state the commit message every time you push your work
    - E.g. "Fixes database migration script failure on 20201010", not just "Fix."

**Note:**

- GitHub renamed the default branch of repositories from `master` to `main` since 2020-10-01

## Framework and API
https://pypi.org/project/areixio/

https://areixio.areix-ai.com/index.html

## Storege and Database
### Environment setup

Install [docker](https://www.docker.com/products/docker-desktop/)

Install [nosql workbench](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/workbench.settingup.html)

Install [areixlib](https://pypi.org/project/areixlib/)

Start the docker by running the below command on terminal

```python
docker run -d -p 8000:8000 amazon/dynamodb-local -jar DynamoDBLocal.jar -sharedDb -dbPath .
```

open the nosql workbench and setup the connection

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/1f829285-1a07-476d-bb52-d432ffd7fcba/Untitled.png)

## Documentation

[index.html](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/aa249af9-f5e2-424d-873c-d91e69254dc6/index.html)

## Sample

[areixlib_sample.py](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/1a0d0e72-db5f-42f9-a75a-3c91f3df48fb/areixlib_sample.py)

## Documentation

You are required to write your README file as if it was for a production service. 

The following items should be include:

1. Description of the problem and solution
2. Clearly clarifing the capstone project you choose to conduct
3. Explain the dataset you have been used
4. Reasoning behind your technical choices, including architectural
5. Trade-offs you might have made, anything you left out, or what you might do differently if you were to spend additional time on the project (future improvement)
6. Formulating an efficient plan where and how to host your application OR Link to the hosted application where applicable (Optional)

## 
