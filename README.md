# **Job Portal Application**

## **Project Overview**
The **Job Portal Application** is a simple, console-based system designed to simulate a job portal. It allows users to post jobs, browse available job listings, apply for jobs, and track applications. This project demonstrates essential object-oriented programming principles and practical software development concepts.

## **Key Features**
1. **Job Listing Management**:
   - Add new job postings.
   - View all available job listings.
   - Search jobs by category or keyword.
   
2. **Job Application System**:
   - Apply for jobs using the job title.
   - Store applicant details.
   - Track applications.

3. **Console-Based Interface**:
   - User-friendly menu-driven interface for interaction.

---

## **Technologies Used**
- **Programming Language**: Java 11 or higher
- **Development Tools**: IntelliJ IDEA, Eclipse, or any Java IDE
- **Data Structures**: Collections (`ArrayList`, `HashMap`) for efficient data storage and retrieval
- **File Handling**: (Optional for persistence in future versions)
- **Version Control**: Git for tracking changes

---

## **Installation and Setup**

### **Prerequisites**
1. **Java JDK**: Version 11 or higher.
   - Download from the official [Oracle JDK website](https://www.oracle.com/java/technologies/javase-jdk11-downloads.html).
2. **IDE (Optional)**: IntelliJ IDEA, Eclipse, or any preferred Java IDE.

### **Steps to Run**
1. **Clone the Repository**:
   ```bash
   git clone <repository_url>
   cd Job-Portal-Application
   ```

2. **Compile the Code**:
   - Using the command line:
     ```bash
     javac Main.java
     ```

3. **Run the Application**:
   - Execute the compiled code:
     ```bash
     java Main
     ```

4. **Interact with the Application**:
   - Use the menu options displayed in the console to interact with the application.

---

## **How the Application Works**

### **Menu System**
Upon running the application, the user is presented with a menu:
1. Add Job Listing
2. View All Jobs
3. Search Job by Keyword
4. Apply for a Job
5. Exit

### **Job Listing Management**
- **Add Job Listing**: Users can add a new job by entering the job title, category, description, and salary.
- **View All Jobs**: Displays a list of all jobs currently in the system.
- **Search Jobs**: Users can search jobs by keyword (title or category).

### **Job Applications**
- **Apply for a Job**: Users can enter their name, email, and the title of the job they wish to apply for. The system validates if the job exists before saving the application.

---

## **Design Choices**

### **Object-Oriented Principles**
- **Encapsulation**: The `Job` and `Applicant` classes encapsulate the data and methods related to job postings and applicants, respectively.
- **Abstraction**: The `JobPortal` class abstracts the logic for managing jobs and applications.
- **Modularity**: Each class handles a specific responsibility, ensuring maintainable and reusable code.

### **Data Storage**
- **In-Memory Storage**: The application uses `ArrayList` and `HashMap` to store jobs and applications in memory, providing efficient data retrieval and manipulation.

### **Input Validation and Error Handling**
- Ensures valid inputs for job details and applicant information.
- Prevents applying for non-existent jobs or entering invalid data.

### **Scalability**
- The modular design makes it easy to extend functionality, such as adding persistence with file storage or integrating a database.

---

## **Assumptions**
1. **Job Titles are Unique**: Job titles are used as identifiers for applying to jobs.
2. **Applicant Data is Limited**: Only the applicant’s name and email are collected during job applications.
3. **Case Sensitivity**: Search functionality assumes case-sensitive keywords for simplicity.
4. **No Persistent Storage**: All data is lost when the application terminates. This can be extended in future versions.
5. **Basic Validation**: Input fields are validated for basic correctness, but advanced checks (e.g., email format) are not implemented.

---

## **Future Enhancements**
- **Persistent Data Storage**: Implement file-based or database storage for job listings and applications.
- **Web-Based Interface**: Transition to a web-based application using a framework like Spring Boot.
- **Enhanced Search**: Implement advanced search functionality, including partial matching and filters.
- **User Authentication**: Add a login system for job seekers and recruiters.
- **Notification System**: Notify applicants and recruiters about updates via email or SMS.

---

## **Example Output**
```
=== Job Portal Menu ===
1. Add Job
2. View All Jobs
3. Search Jobs
4. Apply for Job
5. View Applicants
6. Exit
Enter your choice: 2
No jobs available.
=== Job Portal Menu ===
1. Add Job
2. View All Jobs
3. Search Jobs
4. Apply for Job
5. View Applicants
6. Exit
Enter your choice: 1
Enter Job Title: Software Engineer
Enter Job Category: IT
Enter Job Description: Develop and maintain software applications.
Job added successfully!
=== Job Portal Menu ===
1. Add Job
2. View All Jobs
3. Search Jobs
4. Apply for Job
5. View Applicants
6. Exit
Enter your choice: 1
Enter Job Title: Data Analyst
Enter Job Category: Analytics
Enter Job Description: Analyze data and provide actionable insights.
Job added successfully!
=== Job Portal Menu ===
1. Add Job
2. View All Jobs
3. Search Jobs
4. Apply for Job
5. View Applicants
6. Exit
Enter your choice: 1
Enter Job Title: Digital Marketing Manager
Enter Job Category: Marketing
Enter Job Description: Plan and execute online marketing strategies.
Job added successfully!
=== Job Portal Menu ===
1. Add Job
2. View All Jobs
3. Search Jobs
4. Apply for Job
5. View Applicants
6. Exit
Enter your choice: 1
Enter Job Title:  Mechanical Engineer
Enter Job Category:  Engineering
Enter Job Description:  Design and oversee manufacturing processes.
Job added successfully!
=== Job Portal Menu ===
1. Add Job
2. View All Jobs
3. Search Jobs
4. Apply for Job
5. View Applicants
6. Exit
Enter your choice: 1
Enter Job Title: Civil Engineer
Enter Job Category: Construction
Enter Job Description: Manage construction projects and site supervision.
Job added successfully!
=== Job Portal Menu ===
1. Add Job
2. View All Jobs
3. Search Jobs
4. Apply for Job
5. View Applicants
6. Exit
Enter your choice: 1
Enter Job Title:  UI/UX Designer
Enter Job Category: Design
Enter Job Description: Design user interfaces and enhance user experiences.
Job added successfully!
=== Job Portal Menu ===
1. Add Job
2. View All Jobs
3. Search Jobs
4. Apply for Job
5. View Applicants
6. Exit
Enter your choice: 1
Enter Job Title:  Product Manager
Enter Job Category: Management
Enter Job Description: Oversee product lifecycle and development teams.
Job added successfully!
=== Job Portal Menu ===
1. Add Job
2. View All Jobs
3. Search Jobs
4. Apply for Job
5. View Applicants
6. Exit
Enter your choice: 1
Enter Job Title: Content Writer
Enter Job Category:  Content
Enter Job Description: Write engaging content for blogs and websites.
Job added successfully!
=== Job Portal Menu ===
1. Add Job
2. View All Jobs
3. Search Jobs
4. Apply for Job
5. View Applicants
6. Exit
Enter your choice: 1
Enter Job Title: Financial Analyst
Enter Job Category: Finance
Enter Job Description: Provide insights and reports on financial data.
Job added successfully!
=== Job Portal Menu ===
1. Add Job
2. View All Jobs
3. Search Jobs
4. Apply for Job
5. View Applicants
6. Exit
Enter your choice: 1
Enter Job Title: Network Administrator
Enter Job Category: IT
Enter Job Description: Manage and maintain computer networks.
Job added successfully!
=== Job Portal Menu ===
1. Add Job
2. View All Jobs
3. Search Jobs
4. Apply for Job
5. View Applicants
6. Exit
Enter your choice: 2
Job ID: 1
Title: Software Engineer
Category: IT
Description: Develop and maintain software applications.
--------------------
Job ID: 2
Title: Data Analyst
Category: Analytics
Description: Analyze data and provide actionable insights.
--------------------
Job ID: 3
Title: Digital Marketing Manager
Category: Marketing
Description: Plan and execute online marketing strategies.
--------------------
Job ID: 4
Title:  Mechanical Engineer
Category:  Engineering
Description:  Design and oversee manufacturing processes.
--------------------
Job ID: 5
Title: Civil Engineer
Category: Construction
Description: Manage construction projects and site supervision.
--------------------
Job ID: 6
Title:  UI/UX Designer
Category: Design
Description: Design user interfaces and enhance user experiences.
--------------------
Job ID: 7
Title:  Product Manager
Category: Management
Description: Oversee product lifecycle and development teams.
--------------------
Job ID: 8
Title: Content Writer
Category:  Content
Description: Write engaging content for blogs and websites.
--------------------
Job ID: 9
Title: Financial Analyst
Category: Finance
Description: Provide insights and reports on financial data.
--------------------
Job ID: 10
Title: Network Administrator
Category: IT
Description: Manage and maintain computer networks.
--------------------
=== Job Portal Menu ===
1. Add Job
2. View All Jobs
3. Search Jobs
4. Apply for Job
5. View Applicants
6. Exit
Enter your choice: 3
Enter Job Title to search jobs: Software Engineer
Job ID: 1
Title: Software Engineer
Category: IT
Description: Develop and maintain software applications.
--------------------
=== Job Portal Menu ===
1. Add Job
2. View All Jobs
3. Search Jobs
4. Apply for Job
5. View Applicants
6. Exit
Enter your choice: 4
Enter your Name: Kshitija Garud
Enter your Email: shraddhagarud2003@gmail.com
Enter Job Title you wish to apply for: Software Engineer
Application submitted successfully!
=== Job Portal Menu ===
1. Add Job
2. View All Jobs
3. Search Jobs
4. Apply for Job
5. View Applicants
6. Exit
Enter your choice: 5
Name: Kshitija Garud
Email: shraddhagarud2003@gmail.com
Applied Job Title: Software Engineer
--------------------
=== Job Portal Menu ===
1. Add Job
2. View All Jobs
3. Search Jobs
4. Apply for Job
5. View Applicants
6. Exit
Enter your choice: 6
Exiting Job Portal. Goodbye!

```
