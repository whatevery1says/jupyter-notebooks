# `publication-manager`

`publication-manager` is a Jupyter notebook which creates WE1S `Publications` manifests. As input, it takes an Excel or CSV file (or a list of files) containing columns for each field in the WE1S `Publications` manifest schema. Users may perform the following actions:

- `import` loads the source file(s) and converts them to a list of `Publications` manifests, then inserts them in the WE1S database.
- `update` updates an existing manifest in the database with a user configured dictionary of properties.
- `delete` deletes an existing manifest from the database using its `_id` property.

All of the above actions insert a record of the transaction in a log data base. A log for each transaction contains a MongoDB-generated `_id`, and `id` corresponding to the `_id` property in the WE1S manifest, the datetime of the transaction, and the type of transaction (`import`, `update`, `delete`).

The API contains a number of useful methods:

- `show_databases()` displays all databases in the WE1S database.
- `show_log()` displays the log database.
- `list_publications()` displays a list of all publication manifests in the `Publications` database.
- `clear(database)` deletes all entries from the specified database.

## Important

The first cell in this notebook runs the `configuration_form.ipynb` file, which uses `ipywidgets` to create an interactive user form. If this cell is run, the internal configuration values in cell 2 will be ignored. If you wish to configure the notebook internally, run cell 2 instead.