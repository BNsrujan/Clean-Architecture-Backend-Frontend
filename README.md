# How to Update a Vite Project and Its Packages

Follow these steps to update your Vite project and its dependencies.

## 1. Update Vite to the Latest Version

Run the following command to check and update Vite to the latest version:

```bash
npm install vite@latest

2. Update All Dependencies
You can update all the dependencies in your project using npm-check-updates:

Install npm-check-updates globally:

bash
 
npm install -g npm-check-updates
Check for outdated dependencies: Run this command in your project folder:

bash
 
ncu
This will display a list of outdated packages and their latest versions.

Upgrade all dependencies: To update the package.json with the latest versions, run:

bash
 
ncu -u
Install updated dependencies: After updating package.json, install the updated packages:

bash
 
npm install
