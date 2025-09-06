## This is a customizable Python project template 
Particularly to be used with VScode

Instructions to set up your Python project:
1. **Clone the Repository**: Start by cloning this repository to your local machine. I would just delete git, rename the folder and start fresh.
    ```bash
    git clone <repository_url>
    cd <repository_name>
    # Remove existing git history
    rm -rf .git
    # rename the folder
    mv <repository_name> my-python-project-template
    git init
    ```

2. **Set Up a Virtual Environment**: Create and activate a virtual environment to manage your
    project dependencies. You can use `venv` or `conda` for this purpose.
    Edit the "python.defaultInterpreterPath": "<path_to_your_virtual_environment>/bin/python" in .vscode/settings.json

3. **Install Dependencies**: Use the provided `pyproject.toml` file to install the necessary
    dependencies. You can do this using a package manager like `pip` or `poetry`.
    ```bash
    # either install with or without [dev]
    pip install -e .[dev]
    # Note: If you are using zsh, then use pip install -e '.[dev]'
    ```
4. **Customize the Project**: Modify the project files to suit your specific needs. Update the
    project name, version, description, and author information in the `pyproject.toml` file.

5. **Add Your Code**: Start adding your Python code, modules, and scripts to the project.
    Note: There are many ways to structure a python project. Use the structure that best suits your needs.

6. **Version Control**: Use Git for version control. Commit your changes regularly and push them to a remote
    repository if needed.
    Use the following commands to commit and push your first changes:
    ```bash   
    git add .
    git commit -m "Initial commit"
    git remote add origin <your_remote_repository_url>
    git push -u origin main
    ```
    It obviously assumes that you have already created a remote repository on GitHub, GitLab, or any other platform. 
    If you are using VSCode, you can use the built-in source control features to publish your repository.

7. **Edit README.md**: Update this README file to provide information about your project, how to set it up, and how to use it.  
