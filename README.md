# 🏙️ CityLink: Local Issue Mapping Platform

**CityLink** is a web-based platform that connects **citizens, authorities, and administrators** to collaboratively report, track, and resolve local civic issues such as potholes, waste management, and streetlight failures.  
It enables transparent communication between the public and local authorities to build smarter and cleaner cities 🌍.

---

## 🌟 Key Features

### 👥 Citizen Module
- Register and log in securely  
- Report issues with **location mapping**  
- Upload images of issues  
- Track issue status in real time  

### 🏢 Authority Module
- View reported issues based on assigned area  
- Update issue status and remarks  
- Communicate progress to citizens  

### 🛠️ Admin Module
- Manage authority and citizen accounts  
- Monitor all reported issues  
- Ensure transparency and efficiency in the workflow  

---

## 🧱 Tech Stack

| Layer | Technology |
|-------|-------------|
| **Frontend** | JSP, HTML5, CSS3 (Inline Styling), JavaScript |
| **Backend** | Java (Spring MVC Framework) |
| **Database** | MySQL (`civicmapDB`) |
| **Build Tool** | Maven |
| **Server** | Apache Tomcat |
| **IDE** | Eclipse / IntelliJ IDEA |
| **Version Control** | Git & GitHub |

---

## 🗂️ Project Structure

```
CityLink/
├── src/main/java/com/r3sys/controller/
│   ├── AdminController.java
│   ├── AuthorityController.java
│   ├── CitizenController.java
│   └── IssueController.java
│
├── src/main/java/com/r3sys/dao/
│   ├── AdminDAO.java
│   ├── AuthorityDAO.java
│   ├── CitizenDAO.java
│   └── IssueDAO.java
│
├── src/main/java/com/r3sys/model/
│   ├── Admin.java
│   ├── Authority.java
│   ├── Citizen.java
│   └── Issue.java
│
├── WebContent/WEB-INF/views/
│   ├── adminDashboard.jsp
│   ├── authorityDashboard.jsp
│   ├── citizenDashboard.jsp
│   ├── login.jsp
│   ├── register.jsp
│   └── issueReport.jsp
│
├── WEB-INF/
│   ├── web.xml
│   ├── spring-servlet.xml
│   └── config.xml
│
├── pom.xml
└── README.md
```

---

## ⚙️ Setup Instructions

### 1. Clone the Repository
```bash
git clone https://github.com/your-username/CityLink.git
cd CityLink
```

### 2. Create Database
```sql
CREATE DATABASE civicmapDB;
USE civicmapDB;
```

### 3. Import Tables
Import the SQL file (`civicmapDB.sql`) included in the project folder into MySQL.

### 4. Configure Database Connection
Edit the `config.xml` file and update your MySQL credentials:
```xml
<bean id="dataSource" class="org.apache.commons.dbcp.BasicDataSource">
    <property name="driverClassName" value="com.mysql.cj.jdbc.Driver"/>
    <property name="url" value="jdbc:mysql://localhost:3306/civicmapDB"/>
    <property name="username" value="root"/>
    <property name="password" value="yourpassword"/>
</bean>
```

### 5. Run on Tomcat Server
- Open the project in **Eclipse** or **IntelliJ IDEA**  
- Add the project to **Apache Tomcat**  
- Run the server  
- Open [http://localhost:8080/CityLink](http://localhost:8080/CityLink) 🌐

---

## 🧭 Project Workflow

1. **Citizen** reports issue → stored in DB  
2. **Authority** views assigned issues → updates resolution status  
3. **Admin** monitors and manages roles & reports  
4. **System** ensures transparent updates to users  

---

## 📸 Sample Use Cases
- 🕳️ Reporting potholes or broken roads  
- 🗑️ Complaining about garbage collection delays  
- 💡 Notifying about streetlight failures  
- 🚰 Reporting water leakage or public sanitation issues  

---

## 🤝 Contributing

1. Fork the repository  
2. Create a new branch (`feature-branch`)  
3. Commit your changes  
4. Push to your branch  
5. Open a Pull Request  

---

## 📜 License
This project is licensed under the **MIT License** – see the [LICENSE](LICENSE) file for details.

---

## 👩‍💻 Developed By

**Vaishnavi Chaudhari**  
🎓 B.Tech Student | 💡 Developer | 🌐 Passionate about Smart City Innovation
