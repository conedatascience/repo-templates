# Repository Templates

The purpose of this repository is to house some common repository templates.

These can be called from within internal packages or written directly as needed.

When using version control it is important to practise good hygeine regarding data and privacy.

## Things that shouldn't be a repository

* Large data sets
* Any confidential or private data
* Authorization tokens, passwords, credentials
* Virtual environments

## Documents we have

.gitignore for what git should ignore
.gitattributes for how git should track some things (e.g. binaries vs text)
.dockerignore for what docker should ignore

## Adding to your repository

Using our `eatemplates` packages:

```r
## Single funciton
eatemplates::prep_repo()

## Or one by one
eatemplates::write_attributes()
eatemplates::write_gitignore()
eatemplates::write_docker_ignore()
```
Or from the command line directly:

```
curl https://raw.githubusercontent.com/conedatascience/repo-templates/master/.gitattributes > .dockerignore

curl https://raw.githubusercontent.com/conedatascience/repo-templates/master/.gitattributes > .dockerignore

curl https://raw.githubusercontent.com/conedatascience/repo-templates/master/.gitignore > .gitignore


```
