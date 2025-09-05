# Using uv and pip 
## uv 
When creating my portfolio, I first did everything with uv. Using uv really ismplifies the process and makes things easier. This the flow I used following [this](https://decherd.github.io/eng2_portfolio/projects/portfolio/) set of instructions and links: 

    mkdir eng2_portfolio # make the folder
    cd eng2_portfolio # navigate into the folder 

    uv pip install mkdocs mkdocs-material # install mkdocs and material into uv's environment 

    uv run mkdocs new . # initialize an mkdocs site

    uv run mkdocs serve # run a local dev server 

    git init
    git add .
    git commit -m "Initial MkDocs portfolio"
    git branch -M main
    git remote add origin https://github.com/<YOUR_GITHUB_USERNAME>/eng2_portfolio.git
    git push -u origin main

    uv run mkdocs gh-deploy # publish and push the site 

## pip 
Pip runs a lot slower and with more commands than uv. However, uv is not supported everywhere and so it is useful to know pip. This is a rundown of what I did and learned:

    mkdir project # creates a folder 

    cd project # navigates into that folder 

    python -m venv .venv # creates a virtual environment 

    source .venv/bin/activate # activates and enters the vitrtual environement on a mac

    pip install (your choice of library) # installs your choice of python libraries

    python main.py # run virtual environment 

Next, to clone a repo onto your comuputer you can do 

    git clone (link of the repo) # reate the folder with the repo
    cd (repo name) #navigate into repo

Then if you are using uv you can sync it with a simple line of code: 

    uv sync

However, with pip, you have to go through the process of creating and activating a virtual enviornment. The good news is that instead of adding each library indicidually, most projects have a requiremnets file which you can make use of like this:

    pip install -r requirements.txt
