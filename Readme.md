# Graded Lab Assignment 1 – Linux Command Line Interfaces & Scripting

This repository contains the complete submission for **Graded Lab Assignment 1 (Modules 1–4)**. Each folder corresponds to a specific question from the assignment, including the executed commands, terminal outputs, observations, created lab files, and screenshot evidence.

---

## 📁 Repository Structure

```text
├── Question_1/   # Linux Environment Verification
│   ├── Environment_Report.txt
│   └── Screenshots of command execution & outputs
├── Question_2/   # Secure Project Workspace Setup
│   ├── Project_Workspace_Report.txt
│   └── Screenshots showing directory creation, permissions (chmod 750), & umask
├── Question_3/   # File System and Link Analysis
│   ├── Link_Analysis_Report.txt
│   ├── hard.txt (Hard link test file)
│   └── Screenshots showing inode numbers, stat outputs, and link behaviors
├── Question_4/   # File Access and I/O Investigation
│   ├── IO_Investigation_Report.txt
│   ├── success.log & error.log (Output redirection logs)
│   └── Screenshots showing lsof, /proc/$$/fd, redirection, & ulimits
└── Question_5/   # Storage Health Assessment and Documentation
    ├── Storage_Assessment_Report.txt
    └── Screenshots showing lsblk, df -h, and df -i storage metrics
```

---

## 📝 Assignment Overview & Verification

### **Question 1: Linux Environment Verification**
- Verified user context (`id`), system shell (`echo $SHELL`), working directory (`pwd`), directory contents (`ls -la`), and network connectivity (`ping`).
- All observations and explanations are documented in `Question_1/Environment_Report.txt`.

### **Question 2: Secure Project Workspace Setup**
- Created nested project structure (`project_workspace/{docs,code}`).
- Configured secure permissions (`chmod 750`) and verified default system mask (`umask`).
- Demonstrated how ownership and permission flags protect sensitive project documentation.
- Documented in `Question_2/Project_Workspace_Report.txt`.

### **Question 3: File System and Link Analysis**
- Analyzed inode behavior between original files, hard links, and symbolic (soft) links using `ls -li` and `stat`.
- Evaluated the impact of deleting the target file on both hard links and soft links.
- Documented in `Question_3/Link_Analysis_Report.txt`.

### **Question 4: File Access and I/O Investigation**
- Investigated active open file descriptors (`lsof`, `/proc/$$/fd`).
- Performed stdout and stderr stream redirection (`> success.log 2> error.log`).
- Examined shell resource restrictions using `ulimit -a`.
- Documented in `Question_4/IO_Investigation_Report.txt`.

### **Question 5: Storage Health Assessment and Documentation**
- Assessed block storage devices (`lsblk`), disk capacity usage (`df -h`), and inode utilization (`df -i`).
- Documented findings and long-term storage health recommendations using the `vi` editor in `Question_5/Storage_Assessment_Report.txt`.
