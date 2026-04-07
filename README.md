# 🚀 Oracle Upgrade Lab: 19c → 23c (Oracle AI Database)

## 📌 Overview
Hands-on upgrade using AutoUpgrade.

## 🧪 Environment
- Oracle Linux 8.10
- 4GB RAM
- CDB + PDB

## 📸 Screenshots
Place images in /images folder.

![Analyze](images/analyze.png)
![FRA Fix](images/fra_fix.png)
![Archivelog](images/archivelog.png)
![Upgrade Progress](images/upgrade.png)
![Final Version](images/final.png)

## 🚀 Commands

### Analyze
```
java -jar autoupgrade.jar -config config.cfg -mode analyze
```

### Fix FRA
```
alter system set db_recovery_file_dest_size=10G scope=both;
alter system set db_recovery_file_dest='/u01/app/oracle/fast_recovery_area' scope=both;
```

### Enable Archivelog
```
shutdown immediate;
startup mount;
alter database archivelog;
alter database open;
```

### Deploy
```
java -jar autoupgrade.jar -config config.cfg -mode deploy
```

## ✅ Result
Oracle Database 23c (AI Database)

---

Author: Marcio Costa
