# DevOps Directive GitHub Actions Course

## Development Environment Setup

1. **Clone this repository (including submodules)**  
```bash
git clone --recurse-submodules  git@github.com:rajeshkumarkanaparthi/devops-directive-github-actions-course.git
```

2. **Install DevBox** – DevBox bootstraps all required CLI tools (Go, Node.js, Python, `act`, `task`, `npc`, `civo`, `gh`, `jq`, `yq`, `kubectl`, `kluctl`, ...).  
   Follow the official installation guide: <https://www.jetify.com/docs/devbox/installing-devbox/index#>
   
   After installing devbox, run `devbox shell` to start a shell session with these tools installed/configured.

3. **Install Docker Desktop**  
   Download and install from: <https://docs.docker.com/get-started/introduction/get-docker-desktop/>

4. **Configure VS Code**

      a. **YAML** YAML syntax highlighting & linting

      b. **GitHub Actions** (optional): Workflow file syntax highlighting & snippets

> [!WARNING] 
> The GitHub Actions extension modifies the "file type" of wiles within /.github/workflows/ causing the YAML extension to not recognize those files.
> To fix this, you can add an explicit `files.associations` entry to your settings
> 
> ```json
> {
>   "files.associations": {
>     "**/.github/workflows/*.{yml,yaml}": "yaml",
>     "**/Taskfile.{yml,yaml}": "yaml"
>   }
> }
> ```
      
