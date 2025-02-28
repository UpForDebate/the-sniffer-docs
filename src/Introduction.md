# Introduction

# How To Use

[MDBook Documentation](https://rust-lang.github.io/mdBook)

- (Optional) - Install Mdbook and run on VSCode accordingly to the Documentation to see the results in browser
- Write the pages in Markdown on the "src" folder, .md files outside the src folder won't have access to css like [this](../README.md)
- Subfolders in src are fine as along as they're referenced in the SUMMARY.md
- Add the markdown files to SUMMARY.md
- Push to Github
- Github Actions will build the webpage and display on the web
- WARNING: Because we are poor and can't afford a private website or private repository, please avoid writing sensitive information in these docs