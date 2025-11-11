# N-P-M

npm install <package>
➡️ Install package in the project folder and add it as dependency in package.json

npm install <package> --save-dev
⬅️ Install package in the project folder and add it as development dependency in package.json


### npm install [options]  
Installs dependencies (packages) in a Node.js project from the **npm registry**.

| Command | Description | Example |
| -------- | ------------ | -------- |
| `npm install` | ⭐ Installs all dependencies listed in `package.json`. | `npm install` |
| `npm install [package-name]` | ⭐ Installs the latest available version of a package | `npm install react` |
| `npm install [package-name] --save-dev` | Installs a package as a development dependency. | `npm install typescript --save-dev` |
| `npm install [package-name]@[version]` | Installs a specific version of a package. | `npm install react@18.2.0` |
| `npm install [package-name]@latest` | ⭐ Installs the latest available version of a package. | `npm install react@latest` |
| `npm install [package-name] -g` | Installs a package globally on your system. | `npm install nodemon -g` |
| `npm ci` | Performs a clean install using `package-lock.json` (used in CI/CD). | `npm ci` |


### npm view [package-name] [options]  
Displays information about a package from the **npm registry**.

| Command | Description | Example |
| -------- | ------------ | -------- |
| `npm view [package-name]` | Shows metadata about the package, such as version, dependencies, description. | `npm view react` |
| `npm view [package-name] versions` | Lists all published versions of the package. | `npm view react versions` |
| `npm view [package-name] dependencies` | Lists the package's dependencies. | `npm view react dependencies` |
| `npm view [package-name] devDependencies` | Lists the package's development dependencies. | `npm view react devDependencies` |


### npm update [package-name] [options]  
Updates installed packages to the latest versions that satisfy the version ranges in `package.json`.

| Command | Description | Example |
| -------- | ------------ | -------- |
| `npm update` | Updates all packages in `node_modules` to the latest version that matches the version ranges in `package.json`. | `npm update` |
| `npm update [package-name]` | Updates a specific package to the latest version that satisfies `package.json`. | `npm update react` |
| `npm update [package-name] --save` | Updates the package and **modifies `package.json`** to match the new version. | `npm update axios --save` |
| `npm update --dev` | Updates only the packages listed in `devDependencies`. | `npm update --dev` |
| `npm update --global` | Updates globally installed packages. | `npm update -g nodemon` |
| `npm outdated` | Shows which packages are outdated before updating. | `npm outdated` |
| `npm update [package-name]@latest` | Updates a package to the **latest version available**, ignoring the version range in `package.json`. | `npm update react@latest` |
