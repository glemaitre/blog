---
title: "Chan Zuckerberg Initiative considers scikit-learn an Essential Open Source Software"
date: August 6, 2024
categories:
  - Funding
tags:
  - Open Source
  - Funding
  - Internship
  - Diversity
featured-image: sklearn_czi.png

postauthors:
  - name: Guillaume Lemaitre
    website: https://github.com/glemaitre
    image: guillaume-lemaitre.jpg
  - name: Lucy Liu
    website: https://github.com/lucyleeow
    image: lucyliu.jpeg
---
<div>
  <img src="/assets/images/posts_images/{{ page.featured-image }}" alt="">
  {% include postauthor.html %}
</div>

We are delighted to announce that `scikit-learn` has been awarded a grant from
the [Chan Zuckerberg Initiative (CZI)](https://chanzuckerberg.com/)'s [Essential Open
Source Software for Science
(EOSS)](https://chanzuckerberg.com/rfa/essential-open-source-software-for-science/)
program. This grant is funded by [Wellcome Trust](https://wellcome.org/).
As in previous rounds, this cycle supports open-source software projects that are
essential to biomedical research. This is the third time that CZI EOSS supports
`scikit-learn`.

In this new grant, we will focus on improving the [evaluation and inspection of
predictive
models](https://chanzuckerberg.com/eoss/proposals/predictive-models-evaluation-inspection-in-scikit-learn/).

## Predictive models evaluation & inspection

When building a machine learning pipeline for a specific research problem, two key
aspects are closely connected: (i) design of the pipeline and (ii) assessment, analysis, and
inspection of it. Researchers strive to identify the optimal pipeline, maximizing specific
evaluation metrics, while also seeking at explaining the validity and rationale behind
the pipeline's predictions. This is the cornerstone of answering research
questions. With this proposal we aim to improve and extend the available `scikit-learn`
tools.

`scikit-learn` provides building blocks for model evaluation and statistical analysis of
results. Originally, this information was presented in a raw format and required
expertise from scientists to create intuitive reports for outreach to peers and
outsiders. Recently, the `scikit-learn` community developed displays to easily generate
visual figures for communicating such results. However, these displays are still in
their early development stages and do not leverage all available statistical analysis
tools (i.e., cross-validation) from `scikit-learn`. Thus, we aim to expand these
displays, using the right statistical tools and thus promote the adoption of best
practices when reporting results. Additionally, we also intend to create new displays
to support common analysis tasks that are not yet covered in `scikit-learn`.

In the domain of model inspection, we aim to address several areas: (i) model inspection
during training, (ii) enhancing user experience through interactive inspection, and
(iii) model explainability. First, during the training of a pipeline, researchers are
interested in monitoring the internal characteristics of the model, which is a not yet
addressed long-standing issue in `scikit-learn`. We want to build upon some initial work
by implementing a "callback" framework that allows users to track these internal
parameters. Next, researchers commonly use interactive tools such as Jupyter Notebook to
develop pipelines. `scikit-learn` started some efforts to visually and interactively
display pipelines in these environments. However, there is room for improvement in terms
of user interaction and accessibility. Finally, as `scikit-learn` is widely used as a
reference package, it is crucial to improve the section of the library dedicated to
model explainability. We aim to improve the documentation and user experience with the
existing explainability tools, making sure that they use the appropriate tool for their
use cases. In addition, we propose to work on a scikit-learn enhancement proposal (SLEP)
to define a common API for model explainability within scikit-learn. Ultimately, the
goal is to come to a consensus to provide scikit-learn end-users with a consistent
experience when using model explainability tools.

On top of all these items, we intend to continue working on the general maintenance of
the project, addressing bug reports and performance regressions. As a community-driven
project, we also want to dedicate time reviewing external contributions.

## Involved people

To execute this project, we plan the following hires:

- [Lucy Liu](https://github.com/lucyleeow) (Quansight Labs) will work about half-time on
  the project, on topic related to displays and feature importance.
- We will hire full-time internships to work on the other part of the project. The
  initial plan is to hire two interns for a period of 6 months each and repeat this
  process for the next 2 years. We want to provide opportunities to underrepresented
  groups in the field of machine learning and data science, similarly to previous
  initiatives (cf. [NumFOCUS Small Development
  Grant](https://blog.scikit-learn.org/diversity/mentoring/)).

## Past CZI EOSS grants

In the past `scikit-learn` has been awarded two grants from the CZI EOSS program:

- [CZI EOSS Cycle 1](https://chanzuckerberg.com/eoss/proposals/scikit-learn-maintenance-and-enhancement-for-gradient-boosting/)
  helped at creating to the
  [`HistGradientBoostingClassifier`](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.HistGradientBoostingClassifier.html) and
  [`HistGradientBoostingRegressor`](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.HistGradientBoostingRegressor.html) estimators.
  These estimators are the equivalent of gradient boosting models implemented in
  `LightGBM` and `XGBoost`.
- [CZI EOSS Cycle 4](https://chanzuckerberg.com/eoss/proposals/maintenance-extension-of-scikit-learn-machine-learning-in-python/)
  extended `scikit-learn` to work better with missing values and categorical data in
  several estimators.

Both grants allowed us to maintain and enhance `scikit-learn` to better serve the
community.
