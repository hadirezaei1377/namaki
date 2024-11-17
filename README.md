# Namaki - Internal Company Share Management Platform

**Namaki** is an innovative platform designed for organizations to facilitate seamless management and trading of company shares among employees. This system ensures transparency, efficient transactions, and real-time updates for all stakeholders.

---

## Features  

### 1. **Share Management**  
- View individual share ownership and overall equity distribution.  
- Dashboard displaying each employee's share percentage and its real-time value.

### 2. **Internal Market for Trading Shares**  
- Employees can sell shares directly or set up auction-based pricing.  
- Flexible pricing mechanisms: seller-determined prices or market-driven rates.  
- Transparency through detailed transaction histories.

### 3. **Transaction History and Reports**  
- Comprehensive records of buy/sell transactions for clarity and auditing.  
- Generate share change reports for managers.  

### 4. **Dynamic Share Value Tracking**  
- Historical trends of share prices with interactive charts.  
- Instant notifications on share price changes.  

---

## System Architecture  

Namaki is built with scalability and performance in mind, supporting thousands of transactions in real time. Key architectural highlights include:  
- **Backend**: Written in **Golang**, leveraging its concurrency capabilities for handling high-traffic scenarios.  
- **Frontend**: A clean, intuitive interface for seamless user experience (Framework TBD).  
- **Database**: Uses a relational database (e.g., **PostgreSQL**) for storing transactional data, share values, and user details.  
- **Caching**: Implements caching mechanisms with **Redis** to reduce database load and improve speed.  

---


## Setup  

### Prerequisites  
- **Go** (>=1.20)  
- **PostgreSQL** 
- **Redis** 

### Steps  
1. Clone the repository:  
   ```bash
   git clone https://github.com/hadirezaei1377/namaki.git
   cd namaki
   ```
2. Set up the environment variables:  
   ```bash
   cp .env.example .env
   ```  
   Fill in the database and Redis details in `.env`.  

3. Run database migrations:  
   ```bash
   go run cmd/migrate.go
   ```  

4. Start the server:  
   ```bash
   go run main.go
   ```  

5. Access the platform in your browser at `http://localhost:8080`.  

---

## Contributing  

Contributions are welcome! Please follow these steps:  
1. Fork the repository.  
2. Create a feature branch: `git checkout -b feature-name`.  
3. Commit your changes: `git commit -m "Add feature"`.  
4. Push to the branch: `git push origin feature-name`.  
5. Open a pull request.  

---

## License  

This project is licensed under the MIT License. 

---



