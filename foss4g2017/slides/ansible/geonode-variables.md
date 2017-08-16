# GeoNode Variables

* `app_name` - GeoNode project name (default: `my_geonode`)
* `github_user` - GitHub username that owns the project (default: `GeoNode`)
* `repo_name` - GitHub repository name (defaults to `app_name`: `my_geonode`)
* `code_repository` - URL to the Code Repository
* `branch_name` - Git branch to use for deployment (default: `master`)

The `app_name` variable will be used to set the database names and credentials. You can override this behavior with the following variables:

* `db_data_instance` - Database instance for spatial data
* `db_metadata_instance` - Database instance for the application metadata
* `db_password` - Database password
* `db_user` - Database user

