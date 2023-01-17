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