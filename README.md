# utils

Kill named process by query:
```bash
ps aux | grep python3 | grep client | awk '{print $2}' | xargs -I {} kill -9 {}
```
