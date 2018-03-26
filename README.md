# scripts
Useful script snippets

# prettyprint all json files in directory
find . -type f | sed "s|^\./||" | xargs -n1 -I % sh -c 'python -m json.tool % > pp%'
