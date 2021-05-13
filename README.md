# init_script_node
Create new node progect with only one script

```
function node-project {
  git init
  npx license $(npm get init.license) -o "$(npm get init.author.name)" > LICENSE
  npx gitignore node
  npx covgen "$(npm get init.author.email)"
  npm init -y
  git add -A
  git commit -m "Initial commit"
}
```

Add to: ~/.bashrc \b
Activate: source ~/.bashrc or open a new command line window and run node-project. \b
Start: node-project
