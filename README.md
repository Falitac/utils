# utils

Kill named process by query:
```bash
ps aux | grep python3 | grep client | awk '{print $2}' | xargs -I {} kill -9 {}
```

Proxy port between interfaces (WSL):
```powershell
netsh interface portproxy add v4tov4 listenport= listenaddress=0.0.0.0 connectport= connectaddress=(wsl hostname -I)
```
