# Trustworthy MLLM Tutorial

## From Hallucination Detection to Adversarial Defense: A Unified Framework for LVLM and LLM Safety

This repository contains the website, slides, practical sessions, code, and supplementary material for the tutorial:

> **From Hallucination Detection to Adversarial Defense: A Unified Framework for LVLM and LLM Safety**

The tutorial studies the reliability and safety of **Large Language Models (LLMs)** and **Large Vision-Language Models (LVLMs)** through three complementary perspectives:

1. **Hallucination detection and mitigation**
2. **Uncertainty quantification and calibration**
3. **Adversarial attacks and robust defenses**

Our objective is to provide a unified introduction to the main failure modes of modern generative models and to present practical methods for detecting, quantifying, and mitigating these failures.

---

## Website

The tutorial website is available at:

```text
https://amiad-research.github.io/trustworthy-mllm-tutorial/
```

---

## Tutorial Overview

LLMs and LVLMs are increasingly used for visual question answering, information retrieval, code generation, mathematical reasoning, and autonomous systems.

Despite their impressive capabilities, these models may:

* generate convincing but incorrect information;
* exhibit poor calibration and excessive confidence;
* rely on spurious visual or textual evidence;
* follow misleading assumptions contained in user prompts;
* be manipulated through jailbreaks or prompt injection;
* fail under adversarially perturbed inputs;
* provide unreliable answers without expressing uncertainty.


## Repository Structure

```text
trustworthy-mllm-tutorial/
├── index.html              # Main tutorial website
├── README.md               # Repository documentation
├── assets/                 # Images, photographs, logos, and CSS files
├── slides/                 # Tutorial slides
├── notebooks/              # Practical Jupyter notebooks
├── code/                   # Demonstration scripts
├── references/             # Bibliography and reading material
└── .github/
    └── workflows/          # GitHub Pages deployment workflow
```


Some directories will be added as the corresponding material becomes available.
Also, please note that there is also inside this repository the index.html of the tutorials at ECCV and WACV of previous editions.

---

## Running the Website Locally

Clone the repository:

```bash
git clone  https://amiad-research.github.io/trustworthy-mllm-tutorial/
cd trustworthy-mllm-tutorial
```

Start a local web server:

```bash
python3 -m http.server 8000
```

Then open:

```text
http://localhost:8000
```

in your browser.

---

## Updating the Website

Create a new branch before making modifications:

```bash
git checkout -b update-website
```

After editing the files:

```bash
git add .
git commit -m "Update tutorial website"
git push -u origin update-website
```

Then create a Pull Request on GitHub to merge the changes into `main`.

---

## GitHub Pages Deployment

The website can be deployed using GitHub Pages.

1. Open the repository on GitHub.
2. Go to **Settings**.
3. Select **Pages**.
4. Under **Build and deployment**, select **GitHub Actions** or **Deploy from a branch**, depending on the repository configuration.
5. Select the `main` branch when branch-based deployment is used.
6. Save the configuration.

The website should then become available at:

```text
https://YOUR-GITHUB-USERNAME.github.io/trustworthy-mllm-tutorial/
```

---

## Contributing

Contributions to the tutorial material are welcome.

To propose a change:

1. create a new branch;
2. modify the relevant files;
3. commit and push the branch;
4. open a Pull Request;
5. describe the motivation and content of the modification.

Please avoid pushing directly to the `main` branch.

---

## Citation

A formal citation will be added once the tutorial details are finalized.

For now, the tutorial may be cited as:

```bibtex
@misc{franchi2026trustworthymllm,
  title  = {From Hallucination Detection to Adversarial Defense:
            A Unified Framework for LVLM and LLM Safety},
  author = {Franchi, Gianni and Jenny, Mael and Brellmann, David
            and Bursuc, Andrei and Yao, Angela},
  year   = {2026},
  note   = {Tutorial},
  url    = {https://YOUR-GITHUB-USERNAME.github.io/trustworthy-mllm-tutorial/}
}
```

---

## Related Resources

* [Torch-Uncertainty](https://github.com/ENSTA-U2IS/torch-uncertainty)
* [Many Faces of Reliability](https://abursuc.github.io/many-faces-reliability/)
* [Jailbreaking LLMs and Agentic Systems](https://jailbreak-tutorial.github.io/)

Additional papers, benchmarks, libraries, and tutorials will be added to the annotated bibliography.

---

## License

The website source code and tutorial material are distributed under the license provided in this repository.

Please check the individual licenses of external datasets, pretrained models, libraries, images, and referenced material before reuse.

---

## Contact

For questions concerning the tutorial, please open a GitHub issue or contact the organizing team.

```text
Tutorial repository:
https://amiad-research.github.io/trustworthy-mllm-tutorial/
```
