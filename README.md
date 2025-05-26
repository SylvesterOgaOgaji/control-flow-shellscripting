# Bash Control Flow Scripting: End-to-End Workflow

A complete implementation guide with verification steps for each operation.

---

## 1. Directory Creation & Verification
![Directory Creation](./img/1.%20Create%20a%20directory.jpg)  
**Command**:
```bash
mkdir Bash-Control-flow
```
**Verification**:
```bash
ls -latr Bash-Control-flow
```
**Output**:
```
drwxrwxr-x 2 ubuntu ubuntu 4096 May 26 18:03 Bash-Control-flow
```
**Best Practice**:  
Always create project-specific directories to maintain organized workspaces

---

## 2. Script File Initialization
![File Creation](./img/2.%20file%20created.jpg)  
**Command**:
```bash
touch control_flow.sh
```
**Verification**:
```bash
ls -latr control_flow.sh
```
**Output**:
```
-rw-rw-r-- 1 ubuntu ubuntu 0 May 26 18:05 control_flow.sh
```
**Best Practice**:  
Use `.sh` extension and lowercase filenames for scripts

---

## 3. Permission Elevation
![Permission Update](./img/3.%20Elevated%20the%20permission%20of%20the%20user-owner.jpg)  
**Command**:
```bash
chmod u+x control_flow.sh
```
**Verification**:
```bash
ls -latr control_flow.sh
```
**Output**:
```
-rwxrw-r-- 1 ubuntu ubuntu 0 May 26 18:05 control_flow.sh
```
**Best Practice**:  
Use symbolic notation (`u+x`) for explicit permission management

---

## 4. Script Editing Workflow
![File Editing](./img/4.%20Open%20the%20file%20using%20vim%20editor.jpg)  
**Command**:
```bash
vi control_flow.sh
```
**Editor State**:
```bash
#!/bin/bash
read -p "Enter a number: " num
```
**Best Practice**:  
Always start scripts with shebang line (`#!/bin/bash`)

---

## 5. Core Command Implementation
![Command Entry](./img/5.%20Command%20entered.jpg)  
**Command**:
```bash
read -p "Enter a number: " num
```
**Verification**:
```bash
grep "read -p" control_flow.sh
```
**Output**:
```
read -p "Enter a number: " num
```
**Best Practice**:  
Use `-p` flag with `read` for inline prompts

---

## 6. Complete Workflow Validation
![Permission Update](./img/6.%20Command.jpg)
**Execution Test**:
```bash
./control_flow.sh <<< 5
```
**Expected Output**:
```
Enter a number: 5
```

**Output**:
![Permission Update](./img/7.%20Executed%20successfully.jpg)

---

## 7. Core Command Implementation
![Permission Update](./img/8.%20Entered%20the%20stt.jpg)  

---

## 8. Core Command Execution
![Permission Update](./img/9.%20checked%20for%20a%20positve%20number.jpg)

**Execution Test**:
```bash
./control_flow.sh <<< 5
```
**Expected Output**:
```
Enter a number: 5
```
---

## 9. Core Command Implementation of if Statement
![Permission Update](./img/10.%20if%20stt%20checking%20for%20positive.jpg)  

![Permission Update](./img/11.%20if%20stt%20chk%20positive%20and%20negative.jpg)

**Output**:
![Permission Update](./img/12.%20Cked%20for%20+%20-%200.jpg)

---
## 10. Core Command Implementation: for Loop
![Permission Update](./img/13.%20Types%20of%20for%20loop.jpg)  

**Output**:
![Permission Update](./img/13a.%20Output%20for%20types%20of%20loops.jpg)

## 11. Core Command Implementation: for C-Style Form
![Permission Update](./img/14.%20C-style%20form.jpg)  

**Output**:
![Permission Update](./img/15.output%20for%20c-style.jpg)

---