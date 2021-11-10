# How-to: Accessibility

Accessibility is an important consideration for any open-source software
project.
Please see [this discussion][accessibility_discuss] for further
background information on accessibility.
This article details some best practices that can be adopted by ecosystem
projects to improve accessibility.

[accessibility_discuss]: https://discuss.scientific-python.org/t/discussion-accessible-open-source-projects/63

## Accessible documentation themes

Projects in the scientific Python ecosystem typically use [sphinx][sphinx-doc]
to generate reference and narrative documentation for projects.
Sphinx includes the ability to set a
[consistent theme for the generated html][sphinx-themes], which control various
aspects including page layout, color scheme, and keyboard navigation support.
It is strongly recommended for projects to select a sphinx theme that is
*explicitly designed with accessibility in mind*.
For example, the [pydata-sphinx-theme][pydata-sphinx-theme] integrates
[accessibility validation][accessibility-checks] into its development workflow.

[sphinx-doc]: https://www.sphinx-doc.org/
[sphinx-themes]: https://www.sphinx-doc.org/en/master/usage/theming.html
[pydata-sphinx-theme]: https://pydata-sphinx-theme.readthedocs.io/en/latest/
[accessibility-checks]: https://pydata-sphinx-theme.readthedocs.io/en/latest/contributing.html#accessibility-checks

## Alt-text for images in documentation

Including accurate, descriptive alt-text with html images is important for
users who rely on screen-readers or related technology.
General best-practices include:
- Ensure all images in the project documentation include alt-text
- Validate that alt-text accurately describes the image and integrates well
  with any surrounding text (e.g. avoid forward-references).
