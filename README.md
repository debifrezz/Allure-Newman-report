# Allure-Newman-report
Reporting postman menggunakan allure dan newman

## Module yang dibutuhkan
1. Install [Node.js](https://nodejs.org/en/download)
2. Install [Allure](https://docs.qameta.io/allure/)
```
1. Open PowerShell
2. Input
Set-ExecutionPolicy RemoteSigned -Scope CurrentUser # Optional: Needed to run a remote script the first time
irm get.scoop.sh | iex
3. scoop install allure
4. scoop update allure
```
3. Install [Newman](https://www.npmjs.com/package/newman)
```
npm install -g newman
```
4. Install [Newman-reporter-allure](https://www.npmjs.com/package/newman-reporter-allure?activeTab=readme)
```
npm install -g newman-reporter-allure
```

## Cara Menggunakan
1. Export Environments postman
2. Export Collections postman
3. Buka cmd dan arahkan pada folder yang berisi Environments dan Collections
4. Jalankan "newman run Collection.json -e Environment.json -r allure"
5. Jalankan Allure server untuk melihat hasil reportnya "Allure serve <direktori report>"
