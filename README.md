# installation
reference: https://github.com/leggedrobotics/legged_gym

```bash
# (if needed) sudo apt install libreadline-dev
pyenv install 3.8.19
pyenv local 3.8.19
poetry install --no-root
```
download isaacgym from webpage

```bash
vcs import . < leggedgym.repos
```

after activation, install related packages
```bash
cd isaacgym/python && pip install -e .
cd rsl_rl && pip install -e .
cd legged_gym && pip install -e .
```



# training

after activate poetry
in legged_gym directory
```bash
python legged_gym/scripts/train.py --task=anymal_c_flat

after training, check policy
```bash
python legged_gym/scripts/play.py --task=anymal_c_flat
```

after training, if needed resume training
```bash
python legged_gym/scripts/train.py --resume
```







