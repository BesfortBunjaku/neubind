# Welcome to MkDocs

For full documentation visit [mkdocs.org](https://www.mkdocs.org).

## Commands

* `mkdocs new [dir-name]` - Create a new project.
* `mkdocs serve` - Start the live-reloading docs server.
* `mkdocs build` - Build the documentation site.
* `mkdocs -h` - Print help message and exit.

```mermaid  
    graph TD
    A[Working Directory] -->|Add Changes| B(Git Staging Area)
    B -->|Commit| C[Git Repository]
    C -->|History| D((Commits))
    style A fill:#FFD700,stroke:#000,stroke-width:2px
    style B fill:#87CEEB,stroke:#000,stroke-width:2px
    style C fill:#90EE90,stroke:#000,stroke-width:2px
    style D fill:#FFF,stroke:#000,stroke-width:2px
```

## Project layout

    mkdocs.yml    # The configuration file.
    docs/
        index.md  # The documentation homepage.
        ...       # Other markdown pages, images and other files.

``` py
def bubble_sort(items):
    for i in range(len(items)):
        for j in range(len(items) - 1 - i):
            if items[j] > items[j + 1]:
                items[j], items[j + 1] = items[j + 1], items[j]
```



!!! tip
    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et euismod
    nulla. Curabitur feugiat, tortor non consequat finibus, justo purus auctor
    massa, nec semper lorem quam in massa.

::: neubind.functions
 