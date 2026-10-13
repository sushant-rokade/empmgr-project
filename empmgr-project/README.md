1. For running the project
    i. Now we are in our project folder which is "empmgr-project" and when we are trying run out project file with "python empmgr/cli.py". We are getting an error as "ImportError : attempted relative import with no known parent package".
    ii. Here we didn't specify the parent folder for imported modules for example "from .validators import parse_salary" which is relative imoorts, so here .validators need the parent directory or package to run.
    iii. And when we are trying to run our code as "python -m empmgr.cli", it is working because we are specifying parent package as "empmgr".

2. For setting virtual environment
    i. To manage the versions of libraries for each different project we have virtual environment
    ii. To create virtual environment, we have command as "python -m venv package_name".
    iii. For e.g., if we have package name as .venv we can perform command as "python -m venv .venv".
    iv. After creating virtual environment, we need to check execution policy via "get-executionpolicy".
    v. If it is restricted then use command as "Set-ExecutionPolicy -Scope CurrentUser -ExecutionPolicy Unrestricted -Force".
    vi. And then to activate virtual environment we have command as "package_name\Scripts\activate", in our example it will be like ".venv\Scripts\activate".