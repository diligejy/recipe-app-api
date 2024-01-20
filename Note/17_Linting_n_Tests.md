## 1. What is Linting?

- Tool to check code formatting
- Highlights errors, typos, formatting issues

## 2. How we'll handling Linting

- Install `flake8` package
- Run it through Docker Compose
    - `docker-compose run --rm app sh -c "flake8"`
    
## 3. Testing

- Django test suite
- Setup tests per Django app 
- Run tests through Docker COmpose
    - `docker-compose run --rm app sh -c "python manage.py test`