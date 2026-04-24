# Brute Force Attack Detection using Log Analysis

## 📌 Project Overview

This project focuses on detecting brute force attacks by analyzing authentication logs. A simulated SSH brute force attack is performed, and logs are analyzed to identify repeated failed login attempts.

---

## 🎯 Objectives

* Simulate brute force attack using SSH
* Analyze authentication logs
* Detect suspicious login attempts
* Create detection rules

---

## 🛠️ Tools & Technologies

* Kali Linux (Attacker)
* Ubuntu (Target System)
* SSH Service
* Linux Authentication Logs (/var/log/auth.log)

---

## ⚙️ Lab Setup

1. Set up Ubuntu machine as target
2. Enabled SSH service on target
3. Used Kali Linux to perform brute force attack
4. Monitored authentication logs

---

## 🧪 Attack Simulation

Example brute force command:

```
hydra -l username -P passwords.txt ssh://TARGET_IP
```

---

## 🔍 Log Analysis

Checked logs using:

```
cat /var/log/auth.log | grep "Failed password"
```

---

## 🚨 Detection Logic

* Multiple failed login attempts
* Repeated attempts from same IP
* High frequency of authentication failures

---

## 📊 Sample Detection Command

```
grep "Failed password" /var/log/auth.log | wc -l
```

---

## 📈 Results

* Successfully simulated brute force attack
* Detected failed login attempts in logs
* Identified attacker IP address

---

## 🔗 Conclusion

This project shows how brute force attacks can be detected using simple log analysis techniques without advanced tools.

---

## 👤 Author

Umed Ali
BS Cyber Security Student
SOC Analyst (Blue Team)

#UmedAli
