+++
title = "Beberapa Manfaat Containerization"
description = "manfaat containerization"
[extra]
image = "favicon.ico"
+++ 

### 1. Consistent and Isolated Environment
  
Kita bisa memastikan OS requirement bisa berjalan sesuai standar yg ditetapkan dan terisolasi terhadap main/host OS.
SE atau DevOps tidak perlu manually setup App, Redis Server, DB Server dsb secara berulang kali di tiap komputer berbeda, 
cukup share satu file env untuk base config

### 2. Flexibility, Tidak terikat pada satu platform host services saja   
  
Misal skrg sipintarnet ini continoues deploy nya hanya directly ke app service azure saja tidak bisa ke GCP, AWS karena github action nya spesifik hanya untuk azure app service, Kalau mau pindah2 SaaS ke GCP AWS atau lainnya bisa dilakukan migrasi dengan mudah. 

### 3. Repeatability and Automation Test,Roll Back and Deploy
  
Bisa integrasi CI/CD tentunya secara otomatis bisa Github Action,
bisa rollback docker image, atau redeploy docker image tertentu

### 4. Collaboration, Modularity and Scaling
  
Memudahkan kolaborasi  antar SE, web services dapat dipecah di kemudian hari untuk pertimbangan skalabilitas secara horizontal (secara kebutuhan CPU, RAM, DiskSpace)