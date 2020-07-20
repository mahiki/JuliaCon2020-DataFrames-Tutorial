# juliacon 2020 - Dataframes.jl
Bogumił Kamiński


## prep items
* clone repo
* download dataset from kaggle via UI

```bash
# go to repo and fork:
# https://github.com/bkamins/JuliaCon2020-DataFrames-Tutorial

git clone https://github.com/mahiki/JuliaCon2020-DataFrames-Tutorial.git dataframes

cd dataframes

git remote add upstream https://github.com/bkamins/JuliaCon2020-DataFrames-Tutorial

# bring in all packages and precompile so its ready when you run jupyter nb
julia --project=. -e "using Pkg; Pkg.instantiate(); Pkg.precompile()"

# start up jupyter server in the same folder
julia --project=. -e "using IJulia; notebook(dir=pwd())"

# we:lco:me: b:ack, b:ro
# install Jupyter via Conda, y/n? [y]: y
# [ Info: Running `conda install -y jupyter` in root environment
```

Now its running, but no idea which URL to open in browser.
You need a token, so you can't just `http://localhost:8888`
```bash
jupyter notebook list
# Currently running servers:
# http://localhost:8888/?token=1f812cbf2b3d1729cf261695f740a74dbb802f2857b366ea :: /Users/merlinr/repo/julia-repos/juliacon2020/dataframes

# it prompts token, paste in:
1f812cbf2b3d1729cf261695f740a74dbb802f2857b366ea
```

Boom [Now its running on the browser](http://localhost:8888/notebooks/indexing_part1_introduction.ipynb)

*After you are done please make sure to choose "Quit" option in the top right hand side in the Jupyter Notebook.*
