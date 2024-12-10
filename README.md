

###1. Update All Dependencies
You can update all the dependencies in your project using npm-check-updates:

Install npm-check-updates globally:

```bash
 
npm install -g npm-check-updates
```
Check for outdated dependencies: Run this command in your project folder:

```bash
ncu
```
This will display a list of outdated packages and their latest versions.



Upgrade all dependencies: To update the package.json with the latest versions, run:
```bash
ncu -u
````

Install updated dependencies: After updating package.json, install the updated packages:
```bash
npm install
```

###2: Use --force or --legacy-peer-deps
If you need React 19 and are okay with potential issues:
```bash
npm install --force
```
Or:
```bash
npm install --legacy-peer-deps
```
These options allow npm to bypass the dependency conflict. However, be cautious as this might cause runtime issues.
