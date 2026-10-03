# 📊 Project Tracking App

A lightweight project management canvas app built with **Microsoft Power Apps** to replace manual spreadsheet tracking. It provides project managers and team members with instant visibility into active projects, associated tasks, assigned ownership, and real-time completion progress.

---

## 🖥️️ Core App Structure

### 1. Projects
Displays an overview of organizational projects organized into visual cards separated by status (e.g., *In Progress* and *Completed*).

* **Project Card Details:**
  * Project Name & Description
  * Start Date & Due Date
  * Assigned Person / Project Lead
  * Real-Time Task Progress Tracker (e.g., `2/4 tasks complete`)
* **Project Creation:** Integrated form to create and save new projects directly within the app.

---

### 2. Tasks
A dedicated **Kanban-style task board** that categorizes work across four distinct lifecycle stages:
`To-do` ➔ `In progress` ➔ `Ready for QA` ➔ `Completed`

* **Task Card Details:**
  * Title & Description
  * Associated Parent Project
  * Assigned Team Member
  * Priority (*Low*, *Medium*, *High*)
  * Dates
* **Quick Workflow Actions:** Includes a **Mark Started** action button on task cards that immediately moves a task into the active `In progress` workflow.

---

## 📝 Task Management & Forms

The task creation and editing interface allows users to configure and update task details with the following controls:

* **Task Title & Description:** Scoped details and requirements.
* **Project Selection:** Dropdown to bind the task to its parent project.
* **Assigned User / Team Member:** People selector for task ownership.
* **Priority Level:** Dropdown options for *Low*, *Medium*, or *High*.
* **Due Date:** Date picker for task deadlines.
* **Status Selector:** Direct lifecycle control across board stages.
* **Form Controls:** Save and Cancel actions.

---

## 🎯 Overall Purpose

This application streamlines team collaboration by providing a single source of truth where any user can instantly see:
1. **What projects are active**
2. **What tasks each project contains**
3. **Who is responsible for each item**
4. **What stage each task is currently in**
5. **How much of the total project is completed**