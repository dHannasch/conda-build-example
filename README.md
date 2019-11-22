# conda-build-example
Example of building a conda package locally.

This package builds and installs successfully...but the dependencies are ignored and not installed.
```
~/anaconda3/bin/conda build purge
~/anaconda3/bin/conda build . --channel conda-forge
~/anaconda3/bin/conda create --name tmpEnv python=3.7 funniest --channel ~/anaconda3/conda-bld/linux-64/
~/anaconda3/envs/tmpEnv/bin/python
>>> import funniest
```

