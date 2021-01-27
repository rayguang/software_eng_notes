CI/CD steps:
- black
- flake8
- isort

```
black --check .
```

```
flake8 --max-line-length=88 --ignore E121,E123,E126,E203,E226,E24,E501,E704,W503,W504 src tests
```

```
isort --check-only --line-length 88 --multi-line 3 --trailing-comma --diff src tests
```
