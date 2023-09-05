# mon-premier-programme-nodejs

# Brief - Mon premier programme NodeJS

## SetUp
1- Creation du dossier mon-premier-programme-nodejs
2- Aller sur le dossier précédent
3- Taper : npm init pour ajouter le dossier node-modules et le fichier package.json
4- Creer le fichier .nvmrc avec touch .nvmrc
5- Afficher la liste des fichiers et sous-dossiers avec plus d'option avec la commande LL à la place de LS
6- Ajouter des droits d'éxécution du fichier .nvmrc avec : chmod +x .nvmrc
7- recuperer la version de node installer ==> node -v
8- copier la version et la coller dans .nvmrc
9- lancer la commande nvm use

10-ajouter les commandes au package.json
    "dev": "concurrently -k -n \"Typescript,Node\" -p \"[{name}]\" -c \"blue,green\" \"tsc --watch\" \"nodemon dist/index.js\"",
    "start": "tsc && node dist/index.js"
==> Ouvrir package.json    
==>Ajouter :
```
      "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1",
    "dev": "concurrently -k -n \"Typescript,Node\" -p \"[{name}]\" -c \"blue,green\" \"tsc --watch\" \"nodemon dist/index.js\"",
    "start": "tsc && node dist/index.js"
  },
```

11- ```
    npx tsc --init { "compilerOptions": { "module": "commonjs", "esModuleInterop": true, "outDir": "dist", "target": "es6", "strict": true }, "include": [ "src/**/*" ] }
    ```
==> Creation du tsconfig.json



