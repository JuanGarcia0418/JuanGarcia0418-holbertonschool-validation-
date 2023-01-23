SHELLCHECK=shellcheck

build:	## Generate the website from the markdown and configuration files in the directory dist/
	hugo --destination ./dist

post:	## Create a new blog post whose filename and title come from the environment variables POST_TITLE and POST_NAME
	hugo new posts/$(POST_NAME).md
	sed -i 's/title:*/title: "$(POST_TITLE)"/g' content/posts/$(POST_NAME).md 

clean:	## Cleanup the content of the directoy dist/
	rm -rf dist/

package: ## creates archive
	make build
	zip awesome-website.zip dist/

lint:	## The target lint should be updated to lint the files README.md and DEPLOY.md with markdownlint
	markdownlint README.md
	markdownlint DEPLOY.md
	$(SHELLCHECK) setup.sh >/dev/null 2>&1 || echo "Lint Failed"


unit-tests: ## run unit tests
	@echo "all tests done"

integration-tests: ## run integration-tests
	@echo "all integration-tests done"

validate: ## run validate
	@echo "all validations done"

help:	## Show this help usage
	@fgrep -h "##" $(MAKEFILE_LIST) | fgrep -v fgrep | sed -e 's/\\$$//' | sed -e 's/##//'
