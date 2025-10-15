# BEET: A Comprehensive Taxonomy for IT Job Classification

BEET (Bee-inspired Employment and Expertise Taxonomy) is a hierarchical framework designed to classify IT jobs within the ISCO-08 structure. It provides a structured and precise classification system that helps categorize IT roles, forecast workforce demands, and guide educators in preparing professionals for Industry 5.0.

## Why BEET?

A decade of digitalization has pushed **Technology-driven roles to the center of the global job market**, yet employers and educators still lack a common, **skills-first** language to describe what different IT jobs actually require. That inconsistency makes it harder to (i) classify jobs accurately, (ii) align training, and (iii) forecast demand. Existing standards such as **ISCO-08** are invaluable but not sufficiently granular for today’s hybrid roles and fast-moving stacks. This paper presents **BEET**: a hierarchical framework built from **real job postings** collected worldwide between **2023 and 2025**.  
> Source: World Economic Forum; Frontiers in Education (2025)

**BEET** addresses this gap by introducing:

- A hierarchical structure with 5 major groups, 15 sub-major groups, and 35 unit groups as shown in Figure 1.

- A focus on hard skills and seniority levels.

- A data-driven approach based on global IT job postings (2023-2025).


![BEET Taxonomy](figs/BEET.png)

*Figure 1: Hierarchical structure of BEET Taxonomy.*

## Where the data comes from (and what it looks like)

The team gathered **public, English-language job postings** directly from company sites and verified sources, spanning **October 2023 to February 2025**. Collection mixed **web crawlers** and **targeted manual searches** to balance categories and avoid over-representing only the most advertised roles. Postings were filtered to ensure **explicit technical requisites** relevant to Industry 5.0 skills.  
> Source: Frontiers in Education (2025)

To build, validate, and illustrate BEET, the **labeled dataset** comprises **389 IT postings** from **221 unique companies** of varied sizes and regions. Company names were anonymized and mapped to **LinkedIn size codes (A–I)**. The distribution is dominated by the largest organizations: sizes **I** and **G** contribute most postings; **B** has only two, and **A** has none.

![Company size distribution (A–I)](figs/fig3_company_size.png)  

*Figure 3 — Frequency of job postings by company size.*

A handful of companies account for a disproportionate share of postings, while most contribute **six or fewer**.

![Top companies by postings](figs/fig4_top_companies.png) 

*Figure 4 — Top companies by number of postings.*

Geographically, the **United States** publishes the highest count (**263**), followed by **Brazil** and **Mexico** (**24** each), **Spain** (**13**), and the **UAE** (**11**). These patterns reflect both market size and recruiting practices in innovation hubs.

![Top countries by postings](figs/fig5_top_countries.png)  
*Figure 5 — Top countries by number of postings.*

Crossing **country × size** shows that postings from **large firms (I, G)** concentrate in leading tech geographies (e.g., USA, UK, UAE). When roles cluster in specific regions and company sizes, **language clusters too**, shaping which skills appear salient.

![Company size by country](figs/fig6_size_by_country.png)  
*Figure 6 — Company size by country of publication.*

> Source for figures and counts: Frontiers in Education (2025)

---



## Applications

BEET is designed to support various stakeholders in the IT job market, including:

- HR Professionals: Align applicants with job opportunities more effectively.

- Workforce Analysts: Forecast labor market trends and IT job demands.

- Educators: Structure training programs aligned with Industry 5.0 needs.


## Citation

When referencing this project, please use the following citation formats:


Jorge Valverde-Rebaza, Fabiana Góes, Julieta Noguez, and Nathalia C. Da Silva. Skill-based Employment Taxonomy in the global IT Industry 5.0. Frontiers in Education, April 2025.

```bibtex
@article{valverde:frontiers:25,
  title={{Skill-based Employment Taxonomy in the global IT Industry 5.0}},
  author={Valverde-Rebaza, J. and Góes, F. and Noguez, J. and Da Silva, N.},
  journal={Frontiers in Education},
  volume = {10},
  DOI={10.3389/feduc.2025.1418184},
  ISSN={2504-284X},
  year={2025},
}
```


# Skill-based Employment Taxonomy in the Global IT Industry 5.0 (BEET)








## How BEET was constructed (in brief)

From the cleaned corpus of postings, the authors extracted features with **TF-IDF** and applied **Average Linkage Hierarchical Clustering (ALHC)** with **Ward’s criterion**. The process initially yielded **32 clusters**, which were then grouped into **nine** broader thematic groups and, through expert synthesis, consolidated as the backbone of the taxonomy. Cluster validity scores (e.g., **Silhouette ≈ 0.047**) highlight the **expected overlap** among IT roles: modern descriptions often blend stacks and responsibilities, so low separability is **informative**, not a flaw.  
> Source: Frontiers in Education (2025)

![Clustering dendrogram](figs/fig1_dendrogram.png)  
*Figure 1 — Hierarchical clustering dendrogram from vacancy text.*

Taking clustering as **evidence rather than endpoint**, the team defined **BEET** as a **three-level hierarchy**: **5 Major Groups (MG)**, **15 Sub-Major (SM)**, and **35 Unit Groups (UG)**, each aligned with **ISCO-08**. *MG names follow the article verbatim (e.g., MG4 is “Data”).*

![BEET hierarchical map](figs/fig2_beet_taxonomy.png)  
*Figure 2 — BEET: MG → SM → UG, aligned to ISCO-08.*

> Source for figures: Frontiers in Education (2025)

---

## Conclusion

### What BEET reveals about the market

Once BEET labels are applied, the market becomes **legible at skill resolution**. **Word clouds** per Major Group surface the **anchors**—terms that reliably signal scope—without collapsing distinct roles into vague umbrellas. This is where BEET adds value beyond a keyword index: the **same word** can mean different things across MGs; the **hierarchy disambiguates**.

![Word clouds by Major Group](figs/fig7_wordclouds_mg.png)  
*Figure 7 — Word clouds for the five Major Groups.*

Finally, **Unit Group** distribution by **company size** and **country** nuances demand. Some UGs (e.g., those tied to large-scale platforms or data infrastructure) skew toward **size I** firms, while niche UGs appear in specific geographies. This is actionable for **workforce planning** and **curriculum design**: it points to **where**, and in **which company profiles**, certain skills translate into roles.

![UG distribution by size and country](figs/fig8_distribution_ugs_by_size_country.png)  
*Figure 8 — Unit Group distribution by company size and country.*

### What this means (for analysts, HR, and education)

**Analysts** gain a comparable lens to track demand across countries and employer sizes. **HR teams** get a **skills-first index** to normalize titles and write clearer requisitions. **Educators** obtain a syllabus-level checklist to ensure programs cover the clusters of practice that the market actually signals. Because BEET is **derived from postings** and **aligned to ISCO-08**, it bridges **research rigor** and **operational reality**—a prerequisite for labor statistics, HR systems, and academic programs to **converge** rather than talk past each other.  
> Source for figures and interpretation: Frontiers in Education (2025)

---

## Scope and limitations

The present dataset is **English-only** and drawn from **public** postings, which may under-represent internal pipelines or markets where English is not dominant. Company size and region are **uneven by market**, not by design, and should be considered when generalizing results. Next steps include **multilingual expansion** and **automated classifiers** (including GenAI models) that ingest BEET and label postings at scale.  
> Source: Frontiers in Education (2025)

---

## How to reproduce the figures and clustering (`BEET-EDA.ipynb`)

You can regenerate the descriptive figures and clustering visuals using the notebook in this repository.

**Environment**  
Use **Python 3.10+** in a fresh virtual environment (or Google Colab).

**Dependencies**  
Install the libraries referenced in the **first cell** of `BEET-EDA.ipynb` (for local runs, common requirements include `pandas`, `numpy`, `scikit-learn`, `matplotlib`, `seaborn`, and `wordcloud`). If a `requirements.txt` is added later, prefer it.

**Data placement**  
Place the input files in the repo’s `data/` directory as expected by the notebook.

**Run**  
Open `BEET-EDA.ipynb` and select **Run All**. The notebook writes images to `figs/`. In this README, image links assume filenames like:
- `figs/fig1_dendrogram.png`  
- `figs/fig2_beet_taxonomy.png`  
- `figs/fig3_company_size.png`  
- `figs/fig4_top_companies.png`  
- `figs/fig5_top_countries.png`  
- `figs/fig6_size_by_country.png`  
- `figs/fig7_wordclouds_mg.png`  
- `figs/fig8_distribution_ugs_by_size_country.png`

If the notebook outputs different names, **adjust the links accordingly**.  
> Source: GitHub repository structure

---

## Data & code availability

All materials for this article are available in `jvalverr/beet-it-jobs-taxonomy` (folders: `data/`, `clusters/`, `figs/`, and `BEET-EDA.ipynb`). Please check the repository for updates as the taxonomy evolves.  
> Source: GitHub

---

## Citation

Valverde-Rebaza, J., Rodrigues de Góes, F., Noguez, J., & Da Silva, N. C. (2025). **Skill-based employment taxonomy in the global IT industry 5.0.** *Frontiers in Education*, 10:1418184. https://doi.org/10.3389/feduc.2025.1418184 (Open access, **CC BY 4.0**).


## Generate the Images 

### 1) Environment (Python 3.10+)
```bash
pip install -U pandas numpy matplotlib seaborn plotly scipy dython
```

### 2) Data
Download the CSV from the article’s **Supplementary material** and place it where you prefer (recommendation: `materials/`).  
Link: https://www.frontiersin.org/journals/education/articles/10.3389/feduc.2024.1418006/full#supplementary-material


### 3) Run
```bash
jupyter notebook Data_processing.ipynb
```
The notebook will generate or update figures under `images/`.

---

## Citation

When referencing this project, please use the following citation formats:

**Journal Article:**

Valverde-Rebaza, J., González, A., Navarro-Hinojosa, O., & Noguez, J. (2024). *Advanced large language models and visualization tools for data analytics learning*. Front. Educ. 9:1418006. DOI: [10.3389/feduc.2024.1418006](https://www.frontiersin.org/journals/education/articles/10.3389/feduc.2024.1418006/abstract).

```bibtex
@article{valverde:frontiers:24,
  title={Advanced large language models and visualization tools for data analytics learning},
  author={Valverde-Rebaza, J. and González, A. and Navarro-Hinojosa, O. and Noguez, J.},
  journal={Front. Educ.},
  volume={9},
  pages={1418006},
  year={2024},
  doi={10.3389/feduc.2024.1418006}
}
```

**Conference Extended-Abstract:**

Valverde-Rebaza, J., González, A., Navarro-Hinojosa, O., & Noguez, J. (2024). Empowering Data Analytics Learning: Leveraging Advanced Large Language Models and Visualization Tools. Proceedings of the 19th World Conference on Continuing Engineering Education, IACEE 2024, pp. 47-49. ISBN: 978-1-7327114-3-3.

```bibtex
@inproceedings{Valverde:iacee:24b, 
 author = {Valverde-Rebaza, J. and González, A. and Navarro-Hinojosa, O. and Noguez, J.},
 title = {{Empowering Data Analytics Learning: Leveraging Advanced Large Language Models and Visualization Tools}},
 booktitle = {Proceedings of The 19th World Conference on Continuing Engineering Education},
 series = {IACEE 2024},
 pages = {47--49},
 isbn = {978-1-7327114-3-3},
 publisher = {IACEE},
 year = {2024}
}
```
