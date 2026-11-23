Layers of Reproducibility
================
Jonas Schöley

## Layer 1: Aspirational reproducibility

> The setting: After 6 months of silence, you finally got the reviews for your paper. It's an R&R with many requests for additional analyses. You open your project folder and can't reproduce your old results. It's hard to remember how everything worked. You wish you had documented and organized your work better.

### Examples

- [Aspirational project](examples/aspirational_project/)

## Layer 2: Personal reproducibility

### Topics

1. Project organization
  - What is a project?
  - Folder structure, templates, and naming conventions
  - Research notes
2. Code organization
  - The analysis pipeline
  - Defining inputs and outputs
  - Configuration files
3. Version control
  - The git version control system
  - git as track changes
  - git branches for safe experimentation
  - keeping private things private

### Examples

- [Personal project](examples/personal_project/)
- [Project templates](examples/personal_templates/templates.zip)
- [Project diary](examples/project_diary/)
- [Paper to reproduce](https://www.demographic-research.org/articles/volume/44/19)

## Layer 3: Communal reproducibility

### Topics

1. Code repositories
  - Github/Gitlab/Codeberg as online code repositories
  - Keeping private things private
  - Code documentation
  - Large file
2. Data repositories
  - Zenodo
  - Integrating Zenodo into your code
  - Integrating Zenodo and Github
  - "I can’t share my data"
  - Data documentation
3. Advertisement of your shared resources

### Examples

- [Communal project](examples/communal_project/)
- [Git commands](examples/git_commands/gitcommands.sh)
- [gitignore](examples/gitignore/)
- [A failed attempt at archival](http://www.ageguess.org/)

### Excercises

- [Self-paced course on git & github by Aliakbar Akbaritabar](https://github.com/akbaritabar/Git-GitHub-Version-Control-Interactive-Self-paced-Course)

## Layer 4: Computational reproducibility

### Topics

1. Workflow automation
  - Disadvantages of a single script. Namespace issues, package conflicts, etc.
  - The `targets` R package for defining an analysis pipeline
    - Computational isolation of each target step
2. Reproducing R-language dependencies (with renv, mention rix as an option)
  - Listing dependencies in a project
  - Package version management
3. Containers for near complete reproducibility
  - The problem of system level dependencies
  - The container solution
  - Using other peoples containers
  - Building your own

### Exercises

- [Egors Repository](https://www.ekotov.pro/2025-mpidr-open-science-reproducible-workflows/)
- [renv excercise by Egor Kotov](https://www.ekotov.pro/2025-mpidr-open-science-reproducible-workflows/1-r-packages.html)
- [targets excercise by Egor Kotov](https://www.ekotov.pro/2025-mpidr-open-science-reproducible-workflows/2-analysis-pipeline.html)
