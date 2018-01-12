# jupyter-notebooks
Jupyter notebooks intended for the WE1S Virtual Workspace.

The notebooks in this folder allow users to create or import manifests to the database using forms built with ipywidgets. They do not handle edge cases for documenting some kinds of information, but they should be usable for most workflows. Manifests created by the notebooks are validated against the [schema files](https://github.com/whatevery1says/manifest/tree/master/schema) on GitHub, so they require internet access.

**Notes:**

- Manifest creation forms do not yet handle global properties (`title`, `description`, `label`, etc.). A preliminary configuration form for this is in the works.
- The notebooks have some basic database query functions, including updates and searches.
