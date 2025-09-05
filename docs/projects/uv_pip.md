# Using uv and pip 
## uv 
When creating my portfolio, I first did everything with uv. Using uv really ismplifies the process and makes things easier. These are some of the commands I used:
`uv pip install mkdocs mkdocs-material` This command was the first I used and it installed mkdocs into the uv's environment. Next I initialized my start mkdocs site with `uv run mkdocs new .`
To push my code to build my site, and to update it when I make changes, I use `uv run mkdocs gh-deploy`. This is by far the string of code I use most often for my portoflio. 
Using `uv run mkdocs serve` allows you to see a quick, local preview of your site. 

## pip 
Pip runs a lot slower and with more commands than uv. However, uv is not supported everywhere and so it is useful to know pip. 