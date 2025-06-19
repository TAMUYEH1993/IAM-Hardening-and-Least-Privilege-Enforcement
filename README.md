# 🔐 Project 3: IAM Hardening and Least Privilege Enforcement

## 🎯 Objective
Secure AWS accounts by applying the principle of *least privilege*, auditing IAM users and permissions, and simulating real-world misconfiguration scenarios to strengthen cloud identity and access management.

---

## 🛠 Tools and Services Used
- AWS IAM (Users, Groups, Policies)
- Custom IAM JSON policies
- IAM Access Analyzer
- AWS S3 (to simulate access testing)

---

## ✅ Key Activities Performed

### 1. Created IAM Users and Groups
- Created dev-user and assigned to DevGroup
- Provided minimal access using built-in AmazonS3ReadOnlyAccess policy

### 2. Created Custom Least Privilege Policy
- Built a custom policy that allows only s3:PutObject to a specific bucket (secure-bucket-lab-bond)
- Attached policy to the group to enforce limited access

### 3. Simulated Over-Permission Scenario
- Temporarily attached AmazonS3FullAccess to demonstrate risky access
- Performed actions like listing/deleting other buckets
- Revoked permissions and returned user to least privilege

### 4. Enforced Security Controls
- Enabled *MFA* for IAM users
- Applied a *strong password policy* (min 14 chars, symbols, rotation)
- Blocked public access on unused IAM roles

### 5. Used IAM Access Analyzer
- Created analyzer to detect risky or public access
- Investigated findings related to S3, IAM roles, and policies
- Remediated any public access or cross-account risks

---

## 🧠 Real-World Skills Practiced

| Skill | Application |
|-------|-------------|
| Least Privilege | IAM policy creation and access minimization |
| Auditing | Used IAM Access Analyzer for visibility |
| Security Best Practices | MFA, password policy, restricted API permissions |
| Incident Simulation | Demonstrated escalation and rollback of over-permission |

---

## 📷 Screenshots (Include in Repo)
- IAM user and group creation
- Custom policy JSON
- Access Analyzer findings
- MFA setup screen
- Terminal output of denied vs allowed actions

---

## 💡 Lessons Learned
- Default IAM roles and users often have more access than needed — auditing is critical
- Custom policies allow for very fine-grained control over cloud services
- MFA and strong passwords are essential layers of defense
- IAM Access Analyzer is a powerful tool for detecting hidden security risks

---

## 🔗 Project Repo
*GitHub:* [https://github.com/TAMUYEH1993/IAM-Hardening-and-Least-Privilege-Enforcement]

Created by [Bon Tamuyeh]  
LinkedIn: [www.linkedin.com/in/bon-tamuyeh-b828a02ab]
