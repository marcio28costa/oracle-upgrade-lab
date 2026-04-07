# 🚀 Oracle Upgrade Lab: 19c → 23c (Oracle AI Database)

## 📌 Overview
Hands-on upgrade using AutoUpgrade in a local lab.

## 🧪 Environment
- Oracle Linux 8.10
- 4GB RAM
- CDB + PDB

---

## 📸 Upgrade Steps (Real Screenshots)

### Analyze Phase
![Step1](images/upgrade_step1.png)
![Step2](images/upgrade_step2.png)

### Fix FRA / Archivelog
![Step3](images/upgrade_step3.png)
![Step4](images/upgrade_step4.png)

### Deploy (Upgrade Running)
![Step5](images/upgrade_step5.png)
![Step6](images/upgrade_step6.png)
![Step7](images/upgrade_step7.png)

### Monitoring Progress
![Step8](images/upgrade_step8.png)
![Step9](images/upgrade_step9.png)

### Final Result
![Step10](images/upgrade_step10.png)
![Step11](images/upgrade_step11.png)
![Step12](images/upgrade_step12.png)

---

## 🚀 Commands

### Analyze
```
java -jar autoupgrade.jar -config config.cfg -mode analyze
```

### Deploy
```
java -jar autoupgrade.jar -config config.cfg -mode deploy
```

---

## 🏆 Result
Oracle Database 23c (AI Database)

---

Author: Marcio Costa
