## ESLint (Version Airbnb)
Run the following :
```
sudo npm install -g eslint
npm info "eslint-config-airbnb@latest" peerDependencies
```

## Prettier
1. Run the following :
```
npm info "eslint-config-airbnb@latest" peerDependencies
```
2. Then, create an empty config file to let editors and other tools know you are using Prettier :
```
echo {}> .prettierrc.json

```
3. Create a .prettierignore file to let the Prettier CLI and editors know which files to not format :
    - Tips : You can base your .prettierignore on your .gitignore file
```
vi .prettierignore
```

Pour utiliser Prettier :
    - `npx prettier . --write` pour formatter tous les fichiers.
    - `npx prettier . --write folder/` pour formatter seulement un dossier.
    - `npx prettier . --check` pour vérifier que tous les fichiers sont formatter.

## StyleLint
1. Run the following :
```
npm init stylelint
npm install -D stylelint stylelint-config-standard
```
2. Run Stylelint on all the CSS files in your project :
```
npx stylelint "**/*.css"
```




