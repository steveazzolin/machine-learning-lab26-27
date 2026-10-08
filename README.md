# Machine Learning for Master's in CS and AIS at University of Trento

Official repository for the lab sessions of the *Machine Learning* course (Academic Year 2025/2026), taught by Prof. Andrea Passerini at the University of Trento.

---

## Getting Started

Ensure that you have **Python 3.10 or higher** installed on your system (3.12 matches Google Colab). Then, install all the required packages (every lab, including `tabpfn` for the last section of `LAB1_sklearn`) using `pip`:

```bash
pip install -r requirements.txt
```

### Local environment inside the repository (optional)

To keep everything inside the project folder, with its own Python interpreter, you can create a [conda](https://docs.conda.io) environment in `./.venv` (it is git-ignored):

```bash
conda create -y -p ./.venv --override-channels -c conda-forge python=3.12 pip
./.venv/bin/python -m pip install -r requirements.txt
# On machines with an older NVIDIA driver (e.g., CUDA 12.6), pick the matching PyTorch build:
./.venv/bin/python -m pip install --upgrade --index-url https://download.pytorch.org/whl/cu126 --extra-index-url https://pypi.org/simple torch torchvision
conda activate ./.venv      # or, without activating: ./.venv/bin/jupyter lab
```

> The environment contains absolute paths, so it must be re-created (not moved) if the project folder changes location.

> Alternatively, you can use the provided **Google Colab** links for the notebooks (see folders for details).

---

## Contact

For any issues or questions, you can reach out to:

* Samuele Bortolotti – [samuele.bortolotti@unitn.it](mailto:samuele.bortolotti@unitn.it)
* Steve Azzolin – [steve.azzolin@unitn.it](mailto:steve.azzolin@unitn.it)
