All of your source code (and other program resources) should be placed in this sub-directory.
# Commit message standard
## Git Commit Message Convention (DermaXplain)

We follow a lightweight structured commit format:

<type>(<scope>): <short description>

Optional body:
- bullet points describing changes
- mention generated artifacts when relevant


### Types

- feat      = new functionality
- fix       = bug fix
- refactor  = code restructuring
- data      = dataset / preprocessing changes
- exp       = experiments
- docs      = documentation / report


### Scopes

- inventory
- preprocessing
- model
- xai
- metrics
- pseudo-concepts
- experiments
- report


---

## Examples by Project Phase


### Phase 1 – Data & Preprocessing

feat(inventory): add dataset audit and diagnostics

feat(preprocessing): implement resizing and normalization pipeline

feat(preprocessing): add mask coverage and border-touch features

data(preprocessing): export cleaned dataset manifests

feat(preprocessing): generate enriched preprocessing manifests

- update preprocessing and pseudo-concept notebooks
- export <dataset>_preprocessed.csv files
- include lesion geometry and mask diagnostics


---

### Phase 2 – Model (ResNet)

feat(model): add ResNet-50 baseline classifier

feat(model): implement training loop and evaluation metrics

fix(model): correct label encoding for binary classification


---

### Phase 3 – XAI

feat(xai): implement Grad-CAM using Captum

feat(xai): add SHAP and LIME explanations

refactor(xai): unify saliency map output format


---

### Phase 4 – Metrics

feat(metrics): implement IoU, Dice, and SIR evaluation

feat(metrics): add stability and perturbation tests


---

### Phase 5 – Pseudo-Concepts

feat(pseudo-concepts): generate centroid-based region decomposition

feat(pseudo-concepts): implement border vs core region extraction

feat(metrics): evaluate saliency distribution across pseudo-concepts


---

### Experiments

exp(preprocessing): test hair removal and color normalization

exp(model): compare ImageNet vs dataset-specific normalization


---

### Report / Writing

docs(report): add methodology section for preprocessing pipeline

docs(report): draft pseudo-concept framework description


---

## Notes

- Always mention generated files when relevant (e.g. CSV manifests)
- Keep messages concise but informative
- Use present tense ("add", "implement", not "added", "implemented")