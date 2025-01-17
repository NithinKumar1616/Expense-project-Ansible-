# Automated Full-Stack Deployment Using Ansible  

## Project Overview  
This project demonstrates the automated deployment of a full-stack application using **Ansible**. The application stack consists of:  
- **Frontend:** React.js  
- **Backend:** Node.js  
- **Database:** MySQL  

By leveraging Ansible’s automation capabilities, I successfully deployed and configured the application across multiple AWS EC2 instances.  

---

## Key Features  
1. **Automated Deployment:**  
   - Used Ansible playbooks to automate the setup of database, backend, and frontend services.  
2. **Idempotent Tasks:**  
   - Ensured tasks were executed only when necessary, avoiding redundancy.  
3. **Reverse Proxy Configuration:**  
   - Configured Nginx as a reverse proxy to enable seamless communication between services.  
4. **Scalable and Consistent:**  
   - Managed deployments across multiple EC2 instances with a single tool.  

---

## Deployment Architecture  
The application is deployed on three separate AWS EC2 instances:  
- **Database Server:** Hosts the MySQL database.  
- **Backend Server:** Runs the Node.js application.  
- **Frontend Server:** Hosts the React.js application using Nginx.  

### Commands needed to run the ansible playbooks
ansible-playbook -i inventory.ini database.yml  
ansible-playbook -i inventory.ini backend.yml  
ansible-playbook -i inventory.ini frontend.yml  
