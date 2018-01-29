# jupyter-notebooks
Jupyter notebooks intended for the WE1S Virtual Workspace.

The notebooks in this folder allow users to create or import manifests to the database using forms built with ipywidgets. They do not handle edge cases for documenting some kinds of information, but they should be usable for most workflows. Manifests created by the notebooks are validated against the [schema files](https://github.com/whatevery1says/manifest/tree/master/schema) on GitHub, so they require internet access.

**Notes:**

- Not all manifest creation forms currently handle global properties (`title`, `description`, `label`, etc.).
- The notebooks have some basic database query functions, including updates and searches.

## Task List

- [x] Add global properties to `create_collection`
- [x] Add global properties to `manage_data_nodes`
- [x] Add global properties to `import_collection`
- [x] Add global properties to `manage_other_nodes`
- [ ] Add global properties to `publication-manager`
- [ ] Handle precise dates for `date` in global properties
- [x] Create notebook for `Metadata` nodes (handled by `manage_other_nodes`)
- [x] Create notebook for `Outputs` nodes (handled by `manage_other_nodes`)
- [x] Create notebook for `Related` nodes (handled by `manage_other_nodes`)
- [ ] Create notebook for `Processes`
- [ ] Create notebook for `Scripts`
- [ ] Create notebook for `Projects`
