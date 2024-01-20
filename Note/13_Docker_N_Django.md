## 1. Using Docker with Django

- Many Benefits
    - Consistent dev and prod development
    - Easier Collaboration
    - Capture all dependencies as code
    - Easier cleanup
    - Save a LOT of time

- Drawbacks
    - VSCode unable to access interpreter
    - More difficult to use integrated features (interactive debugger, linting)
    - Suggest using Terminal

## 2. Configure Docker

- Create a Dockerfile
- Lists steps for creating image
    - Choose a base image (python)
    - install dependencies
    - Setup users

## 3. Docker Compose

- How our Docker image(s) should be used
- Define our "services"
    - Name (eg: app)
    - Port mappings
    - Volume mappings

## 4. Using Docker Compose

- Run all commands through Docker Compose

    - docker-compose run --rm app sh -c "python manage.py collectstatic"

- `docker-compose` runs a Docker Compose command
- `run` will start a specific container defined in config
- `--rm` removes the container
- `app` s the name of the service
- `sh -c` passes in a shell command
- command to run inside container