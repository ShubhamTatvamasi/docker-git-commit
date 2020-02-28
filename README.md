# docker-git-commit

pass the commit hash as an argument  
```bash
docker build --build-arg GIT_COMMIT=$(git rev-parse HEAD) -t git-commit .
```

verity the hash
```bash
docker run --rm git-commit printenv GIT_COMMIT
```
