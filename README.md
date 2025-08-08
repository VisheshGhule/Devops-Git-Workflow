## Git Workflow
- This project is part of Task 4 - Git branching and merging.

## Objective
Implement a basic Git workflow with multiple branches (`main`, `dev`, and `feature-readme`), manage `.gitignore`, and create a Git tag.

---

## 📦 Steps Performed

### Step 1: Create Repository
- Created a new empty repository on GitHub named **Devops-Git-Workflow**.
- Cloned it locally:
```bash
git clone https://github.com/VisheshGhule/Devops-Git-Workflow.git
cd Devops-Git-Workflow
```
---

### Step 2: Create dev Branch
```bash
git checkout -b dev
git push origin dev
```

---

### Step 3: Create feature-readme Branch from dev
```bash
git checkout -b feature-readme
```
<br><br>
<img width="750" height="180" alt="Screenshot from 2025-08-08 12-13-49" src="https://github.com/user-attachments/assets/991df62d-8569-40e6-ab17-0ac7df824171" />

---

### Step 4: Add README.md File
```bash
echo "# DevOps Git Workflow" > README.md
git add README.md
git commit -m "Added README file"
git push origin feature-readme
```

---

### Step 5:  Pull Request: ``feature-readme`` → ``dev``
- On GitHub, created a Pull Request from ``feature-readme`` to ``dev``.
- Merged the PR.
<br><br>
<img width="1000" height="300" alt="Screenshot from 2025-08-08 12-16-16" src="https://github.com/user-attachments/assets/20f24cc6-8078-4b95-a9d7-e71921236d2e" />

<br><br>

<img width="250" height="53" alt="Screenshot from 2025-08-08 12-16-34" src="https://github.com/user-attachments/assets/db65cb43-b356-4c7c-ae46-dcea7b4cd59d" />

<br><br>

<img width="650" height="1000" alt="Screenshot from 2025-08-08 12-17-37" src="https://github.com/user-attachments/assets/7d417f1c-6ef3-431f-99d4-96e78125abe6" />

<br><br>

<img width="1000" height="113" alt="Screenshot from 2025-08-08 12-20-36" src="https://github.com/user-attachments/assets/fb4035b9-a16b-4cdc-8e59-8269e8df1302" />

---

### Step 6: Merge ``dev`` into ``main``
- On GitHub, created a Pull Request from ``dev`` to ``main``.
- Merged the PR.
<br><br>
<img width="900" height="185" alt="Screenshot from 2025-08-08 12-21-23" src="https://github.com/user-attachments/assets/e7ddae34-b82b-46c1-b182-e358a3802c03" />

<br><br>

<img width="638" height="382" alt="Screenshot from 2025-08-08 12-22-42" src="https://github.com/user-attachments/assets/53719aa5-1c11-43aa-838d-6ec5cb540ead" />

<br><br>

<img width="638" height="382" alt="Screenshot from 2025-08-08 12-22-59" src="https://github.com/user-attachments/assets/b788b367-5096-488d-89df-e4d1d4d198de" />

<br><br>

<img width="638" height="382" alt="Screenshot from 2025-08-08 12-23-11" src="https://github.com/user-attachments/assets/6004b22f-84e6-4015-a642-7cc311d49a3c" />

---

### Step 7: Add ``.gitignore`` File in ``dev``
```bash
echo "node_modules/" > .gitignore
echo ".terraform/" >> .gitignore
git add .gitignore
git commit -m "Added .gitignore file"
git pull origin dev --rebase
git push origin dev
```

---

### Step 8: Merge ``.gitignore`` from ``dev`` into ``main``
- On GitHub, created a Pull Request from ``dev`` to ``main``.
- Merged the PR.
<br><br>
<img width="1000" height="236" alt="Screenshot from 2025-08-08 12-31-28" src="https://github.com/user-attachments/assets/d6efa491-e97d-48bf-a217-9c2c5bb52164" />

---

### Step 9: Create Git Tag
```bash
git checkout main
git pull origin main
git tag v1.0
git push origin v1.0
```
<br><br>
<img width="619" height="455" alt="Screenshot from 2025-08-08 12-33-34" src="https://github.com/user-attachments/assets/58142470-7dba-4d83-b1a0-1c47b48616b6" />

<br><br>

<img width="550" height="180" alt="Screenshot from 2025-08-08 12-33-53" src="https://github.com/user-attachments/assets/a40b4975-28fe-4772-af1a-a01911c7fbff" />


