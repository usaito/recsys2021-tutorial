## Counterfactual Learning and Evaluation for Recommender Systems (RecSys'21 Tutorial)

Materials for **"Counterfactual Learning and Evaluation for Recommender Systems: Foundations, Implementations, and Recent Advances"**, a tutorial delivered at the 15th ACM Conference on Recommender System ([RecSys'21](https://recsys.acm.org/recsys21/)).

- Presenters: [Yuta Saito](https://usaito.github.io/) (Cornell University, USA) and [Thorsten Joachims](https://www.cs.cornell.edu/people/tj/) (Cornell University, USA).

- The tutorial website: https://sites.google.com/cornell.edu/recsys2021tutorial
- The tutorial proposal: https://dl.acm.org/doi/10.1145/3460231.3473320
- The list of tutorials at RecSys2021: https://recsys.acm.org/recsys21/tutorials/
- Reference Package (Open Bandit Pipeline): https://github.com/st-tech/zr-obp
- A survey of related papers and resources: https://github.com/hanjuku-kaso/awesome-offline-rl


### Contents

- [examples](./examples): brief examples describing how to use Open Bandit Pipeline with synthetic data, classification data, and real-world bandit data
- [simulations](./simulations): simulation codes comparing a wide variety of existing OPE estimators on synthetic data
- [real-world](./real-world): a brief demo of OPE/OPL on real bandit dataset (need [Open Bandit Dataset](https://research.zozo.com/data.html))
<!-- - [slides](./slides): tutorial slides -->

The Google Colab version of implementations (examples) are available [here](https://drive.google.com/drive/folders/1P3IPoFhVQ0n19EU5PCF_ZfkxRdpTJnJa?usp=sharing).

### Requirements and Setup

The Python environment is built using [poetry](https://github.com/python-poetry/poetry). You can build the same environment as in our examples and simulations by cloning the repository and running `poetry install` directly under the folder (if you have not install poetry yet, please run `pip install poetry` first.).

```
# clone the obp repository
git clone git@github.com:usaito/recsys2021-tutorial.git
cd benchmark/ope

# build the environment with poetry
poetry install

# activate jupyter-lab environment
poetry run jupyter lab
```

The versions of Python and used packages are as follows.
```
[tool.poetry.dependencies]
python = "^3.9,<3.10"
scikit-learn = "0.24.2"
numpy = "^1.21.2"
pandas = "^1.3.3"
obp = "0.5.1"
matplotlib = "^3.4.3"
jupyterlab = "^3.1.13"
```

### Contact
If you have any question, please feel free to contact: ys552@cornell.edu
