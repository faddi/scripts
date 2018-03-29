# scripts

Prettyprint all json files in directory
```bash
find . -type f | sed "s|^\./||" | xargs -n1 -I % sh -c 'python -m json.tool % > pp%'
```

Find all files containing "data" and copy them to ../data
```bash
grep -r -l --null "data" . | xargs -0 -J % cp % ../data
```
