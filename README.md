# 🏆 Employee Recognition Tracker (Salesforce Project)

## 📌 Project Overview

The **Employee Recognition Tracker** is a Salesforce-based solution designed to automate the process of identifying, evaluating, recognizing, and rewarding high-performing employees. It enables HR teams and managers to streamline employee evaluation workflows, send automated recognition emails, and support budget-based rewards distribution.

---

## ⚙️ Key Features

- **Two Custom Objects**:
  - `Data`: Stores employee performance data.
  - `Voting`: Stores managerial ratings and feedback for shortlisted performers.

- **Automation with Flows**:
  - `Flow 1`: Automatically moves employees from `Data` to `Voting` object if **Performance % > 80**.
  - `Flow 2`: Sends **recognition email** to employees if **Rating ≥ 4** after feedback from manager.

- **Profiles & Permission Sets**:
  - `Manager Profile`: Full access to Voting object (rating & feedback), no access to Data entry.
  - `Company Profile`: Basic access for admin users; restricted view for employees.
  - `Permission Sets`: Granular visibility control.

- **Validation Rules**:
  - Ensures correct performance entry.
  - Prevents unauthorized changes in the Voting stage.

- **Reports & Dashboards**:
  - Track recognized employees, ratings, performance distribution.
  - Visualize top performers and recognition trends over time.

---

## 🧾 Recognition & Budget Allocation Workflow

1. Employees with **>80% performance** are automatically shortlisted for recognition.
2. Managers assign **ratings and feedback** in the Voting stage.
3. Top performers (**Rating ≥ 4**) receive **auto-generated recognition emails**.
4. Final recognition data is sent to the **Finance Department**.
5. Finance team **allocates budget** to top performers based on recognition data.
6. (Future Enhancement) Data to be **auto-sent to Finance via Flow**.

---

## 📈 Future Enhancements

- 🔁 Automate Finance data transfer using Flows.
- 🏅 Add a recognition **leaderboard** or historical tracker.
- 💰 Integrate with **payroll** or **reward platforms**.
- 🧮 Implement **reward points system** for recognized employees.

---

## 👩‍💼 User Roles

| Role           | Access                                  |
|----------------|------------------------------------------|
| Manager        | Voting Object (Rate, Comment, View)      |
| HR/Admin       | Both Objects, Dashboards, Reports        |
| Employee       | No access to Voting (restricted)         |

---

## 📧 Email Notification Sample

> **Subject**: Congratulations {!$Record.Emp_Name__c}, You’ve Been Recognized! 🎉  
> **Body**:
Hello {!$Record.Emp_Name__c},
We’re thrilled to inform you that you’ve been recognized as a Top-Performing Employee based on your outstanding contributions, dedication, and consistent performance.
Your hard work, positive attitude, and commitment to excellence have truly made a difference. Thank you for being an integral part of the team.
Keep up the great work!

Warm regards,
HR Team

## ✅ Requirements

- Salesforce Developer Edition
- Custom Object & Flow creation permissions
- Basic Lightning App Builder knowledge

---

## 👨‍💻 Developed By

**Rakesh Yarra and My Teammates**  
*Pragati Engineering College*  
LinkedIn: [linkedin.com/in/rakeshyarra](http://linkedin.com/in/rakeshyarra)
