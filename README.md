# **ITNE352-Project-Group-B1**


## **Project Title**

**Multithreaded News Client/Server Information System**


## **Project Description**

The **News Exchange System** is a client-server application designed to provide users with news updates from **NewsAPI.org**.  
It comprises two primary components:

- A **server script** that fetches news data and processes client requests.  
- A **client script** that enables user interaction with the server to access news updates.


## **Semester**  

**1st Semester 2024**


## **Group Details**  

- **Group Name:** Group B1  
- **Course Code:** ITNE352  
- **Section:** 2  
- **Student Names:**  
  - **Hamza ALi Albasara** - 202207575  
  - **Yusuf Hesham Shareeda** - 202206065  


## **Table of Contents**

1. [Requirements](#requirements)  
2. [How to Run](#how-to-run)  
3. [The Scripts](#the-scripts)  
4. [Additional Concept](#additional-concept-implementing-tlsssl-for-secure-communication)  
5. [Acknowledgments](#acknowledgments)  
6. [Conclusion](#conclusion)  
7. [Resources](#resources)  


## **Requirements**

Follow these steps to set up and run the project in a local environment:

1. **Install Python** (if not installed): [Download Python](https://www.python.org/downloads/)  
2. Clone the repository:  
   ```bash
   git clone https://github.com/o5g5o/ITNE352-Project-GroupB1.git
   ```  
3. Navigate to the cloned directory:  
   ```bash
   cd ITNE352-Project-Group-B1
   ```  
4. Install required dependencies:  
   ```bash
   pip install -r requirements.txt
   ```  
5. **Get a NewsAPI API Key**:  
   - Register on [NewsAPI.org](https://newsapi.org/)  
   - Replace `"api_key"` in the server script with your API_KEY.


## **How to Run**

To run the system:  

1. Open a terminal.  
2. Navigate to the project directory:  
   ```bash
   cd ITNE352-Project-Group-B1
   ```  
3. Start the server:  
   ```bash
   python server.py
   ```  
4. In another terminal, start the client:  
   ```bash
   python client.py
   ```  
5. Use the client-side interface to:  
   - Search headlines  
   - View sources  
   - Exit the application  


## **The Scripts**

### **Client Script (`client.py`)**

The **client script** allows users to interact with the server for news updates.

#### **Key Functionalities**  

1. **Connects to the server using sockets**  
   ![Connection to server](images/connection.png)  
2. **Displays a menu-driven interface**  
   - Search headlines  
   ![Headline search](images/headline.png)  
   - View sources  
   ![Sources search](images/sources.png)  
   - Exit the application  
3. **Receives and displays results from the server**  
   ![Display data](images/display_data.png)
   ![Display data2](images/display_data2.png)


### **Server Script (`server.py`)**

The **server script** manages connections, retrieves data, and processes requests.

#### **Key Functionalities**  

1. **Manages client connections** using sockets and threading  
   ![Sockets](images/server.png)  
2. **Fetches news data** from NewsAPI.org using the `requests` library  
   ![Fetch data](images/server2.png)  
3. **Processes client requests**  
   ![Process request](images/server3.png)  
4. **Returns relevant responses**  
   ![Returned responses](images/server4.png)


## **Additional Concept**: Implementing TLS/SSL for Secure Communication  

### **Description**

To enhance security, **TLS/SSL** (Transport Layer Security/Secure Sockets Layer) was implemented. This ensures that all data exchanged between the client and server is encrypted, preventing unauthorized access.  

By using TLS/SSL:  
- Packet transactions are secured.  
- Data confidentiality and integrity are maintained.


## **Acknowledgments**

We express our gratitude to NewsAPI.org for providing invaluable resources. Their comprehensive and regularly updated news database forms the backbone of our application, ensuring users receive accurate and relevant information.

A special thanks to Dr. Mohamed Almeer for his guidance, support, and encouragement throughout this project. His expertise and valuable insights greatly contributed to the successful completion of our work.


## **Conclusion**

The development of the **News Socket Client/Server System** is a significant milestone in mastering concepts of:  
- Network programming  
- API integration  
- Client-server frameworks  

This project demonstrates a robust and scalable approach, incorporating:  
- Error handling  
- Logging  
- Serialization  
- Threading  
- Enhanced user interface  



## **Resources**

- **NewsAPI Documentation**:  
  [Visit Documentation](https://newsapi.org/docs)  
  *Description*: Official documentation for **NewsAPI.org**.
