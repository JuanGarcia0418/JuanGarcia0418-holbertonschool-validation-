## Prerequisites
### Hugo
- https://gohugo.io/
    ``` 
    $ hugo new site quickstart
    $ cd quickstart
    $ git init
    $ git submodule add
    $ echo "theme = 'ananke'" >> config.toml
    $ hugo server 
    ```
## Lifecycle
- Build
``` $ make build ```
- Clean
``` $ make clean ```
- Post
``` $ make post ```
- Help
``` $ make help  ```

## Workflow
- Clone the repository (checkout)
- Change to the appropriate directory and execute make help

## Build Workflow
- Github workflow

## Lifecycle
- this lfecycle section must be done now

- build: A website generator in ./dist directory clean: Clean the /dist directory thoroughly help: show help post: make a post with title = POST_TITLE and name = POST_NAME (environ variables) package: make a package