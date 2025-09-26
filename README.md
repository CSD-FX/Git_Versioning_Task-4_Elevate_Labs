# DevOps Task 4 — Version-Controlled Fantastic Beasts Website

This repository demonstrates Git version control best practices in a DevOps workflow. 
It contains a small static website themed around the "Fantastic Beasts" movie series 
(Harry Potter prequel), showing how feature branches, pull requests, and version tagging work.

## Project Objective
- Learn and apply Git branching strategies (`main`, `dev`, feature branches)
- Create pull requests and merge features systematically
- Tag versions for milestones (v1.0, v2.0)
- Deploy a static website using GitHub Pages

## Website Structure
- **Version 1.0 (v1.0):**  
  - Landing page (`index.html`) with movie poster  
  - About page (`about.html`) with detailed movie info

- **Version 2.0 (v2.0):**  
  - Contact page (`contact.html`) with project creator info  

All pages share a common CSS file (`assets/css/style.css`) for consistent styling.

## Branch Strategy
- `main` — production-ready code, always stable  
- `dev` — integration branch for feature testing  
- `feature1-about` — adds the About page  
- `feature2-contact` — adds the Contact page

** YOU CAN READ MORE ABOUT THE BRANCHING AND TAGGING DETAILED STEPS IN TASKS.MD FILE

---

## Deployment

---
*** METHOD 1 ***
- Hosted on **GitHub Pages** (free, static hosting)  
- URL: `https://<your-username>.github.io/devops-task4/`

___

*** METHOD 2: Run Locally ***
1. Clone the repository:
```bash
   git clone https://github.com/CSD-FX/Git_Versioning_Task-4_Elevate_Labs.git
   cd Git_Versioning_Task-4_Elevate_Labs
```
2.Serve site locally
```bash
   python3 -m http.server 8000
```
3.Access in browser
```bash
   http://localhost:8000/index.html
```
---

*** If you want to edit the HTML pages, then run on another port after the editing of the files or kill the pid process of port 8000 and run again on port 8000

1) Using different port:
  ```bash
     python3 -m http.server 9000
  ```
  ```bash
     python3 -m http.server 9000
  ```
2) Kill the process using port 8000 and run again on port 8000:
  * Find the PID (process ID) of the process using port 8000
    ```bash
       lsof -i :8000
    ```
  * kill that process
    ```bash
       kill -9 <your PID>
    ```
  * Now you can use port 8000 again to host your own edited HTML pages
    ```bash
       python3 -m http.server 9000
    ```
---

🫡 HOPE YOU LIKED THE PROJECT AND LEARNT ABOUT GIT VERSIONING / TAGGING AND HOW TO CREATE SPECIFIC BRANCHES FOR PERTICULAR FEATURES WITH ALL THESE PRACTICES USED IN REAL WORLD PROJECTS / DEPLOYMENT ☺️✌🏼
