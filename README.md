# OUCRU R training course 2025
The GitHub repository for the OUCRU R training course in 2025

Materials for the course in their quarto format are stored here

## For instructors

- Make sure you are using `renv` for R package version control
    - Always start your session with `renv::restore()`
    - Before commit and push, run `renv::snapshot()`
- Locations:
    - Slides go into `slides/`
        - Slides should have `format: revealjs` in the YAML headers
    - Handouts go into `handouts/`
        - Handouts should have `format: html` in the YAML headers (or `pdf` if you wish)
    - Custom CSS rules go into `styles.css`
        - Append your own CSS rules here
- Test **locally** with
    - `quarto preview`: live preview and continuously render on save
    - `quarto render`: one-time render; resulting main page is `_render/index.html`
- **Publish** by:
    - simply push your commits to the `main` branch, GitHub Actions should handle the rendering and publishing (desired)
    - `quarto publish gh-pages` (undesired)
- Project metadata is in `_quarto.yml`. You can control the metadata in your specific `.qmd` files with its YAML header, which will override the project metadata. 
