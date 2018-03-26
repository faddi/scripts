# scripts

# prettyprint all json files in directory
```bash
find . -type f | sed "s|^\./||" | xargs -n1 -I % sh -c 'python -m json.tool % > pp%'
```
