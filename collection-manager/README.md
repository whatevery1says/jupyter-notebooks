# `collection-manager`

`collection-manager` is a series of Jupyter notebooks which create WE1S `collection` manifests. The functions of each notebook are listed below:

## `create_collection`

Creates and displays a top-level collection manifest from user configurations. The user has the option to insert the manifest into the WE1S database.

## `import_collection_data`

Inserts a list of data manifests into the WE1S database. The script first checks whether the collection and Data Node listed in the manifest exist in the database. If the node does not exist, one is created using user-configured variables.

**Notes:**

- Data manifests are not validated before they are inserted in the database.
- There probably needs to be a notebook that allows the user to insert or update a Data Node manifest without importing data. These could be added to the API, but the filename `import_collection_data` would probably have to be changed to something more general.