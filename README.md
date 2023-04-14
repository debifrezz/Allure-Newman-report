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
![Environments](https://github.com/debifrezz/Allure-Newman-report/blob/main/Pict/Environments.PNG)
2. Export Collections postman
![Collections](https://github.com/debifrezz/Allure-Newman-report/blob/main/Pict/Collections.PNG)
3. Buka cmd dan arahkan pada folder yang berisi Environments dan Collections
![CMD](https://github.com/debifrezz/Allure-Newman-report/blob/main/Pict/CMD.PNG)
4. Jalankan "newman run Collection.json -e Environment.json -r allure"
![Run-newman](https://github.com/debifrezz/Allure-Newman-report/blob/main/Pict/Allure-report.PNG)
5. Jalankan Allure server untuk melihat hasil reportnya "Allure serve (direktori report)"
![Allure-serve](https://github.com/debifrezz/Allure-Newman-report/blob/main/Pict/Allure-serve.PNG)
6. Allure Dashboard
![Dashboard](https://github.com/debifrezz/Allure-Newman-report/blob/main/Pict/Allure-Dashboard.png)
