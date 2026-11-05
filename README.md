# MultiFate-2: Exploring Dimerization Affinities

Repository for the Theoretical Systems Biology project, part of the M2 Interdisciplinary Master in Life Sciences (IMaLiS) program at ENS-PSL.

## About

This project explores the **MultiFate-2** mathematical model developed by Zhu et al. (2022), which describes how interacting transcription factors can generate multiple stable expression states.

The original model assumes equal dissociation constants for AA, BB, and AB dimers. We extend it by allowing these three constants (**KAA, KBB, and KAB**) to vary independently, to examine how relative dimerization affinities affect multistability and state transitions.

## Notebooks

- **`MF2_Phase_Portrait.ipynb`** — Derives the modified model, checks its agreement with the original model when the dissociation constants are equal, and compares phase portraits under different affinities.
- **`MF2_Parameter_Screen.ipynb`** — Validates the modified implementation and explores how changing model parameters and dimerization affinities affects the number and types of stable states.

## Running the notebooks

Use Python 3 and Jupyter Notebook. Install the main dependencies with:

```bash
pip install notebook numpy scipy matplotlib seaborn pandas scikit-learn shapely
```

Then open either `.ipynb` file in Jupyter and run its cells in order.

## AI Use Disclosure

ChatGPT (GPT-6, OpenAI) was used as an assisting tool during the derivation of the modified equations and for code debugging. All suggestions were reviewed by the repository author, who retained control over the mathematical derivation, code, analyses, and final decisions and takes responsibility for the work.

## Reference

Zhu, R., del Rio-Salgado, J. M., Garcia-Ojalvo, J., & Elowitz, M. B. (2022). **Synthetic multistability in mammalian cells.** *Science, 375*(6578), eabg9765. https://doi.org/10.1126/science.abg9765

This project builds on the model and original computational work described in that paper.
