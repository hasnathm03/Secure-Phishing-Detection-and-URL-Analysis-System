1. Introduction
Phishing remains one of the most persistent and damaging threats in the cybersecurity landscape. Attackers create fake websites that are almost indistinguishable from the real thing, luring users into entering sensitive credentials like passwords, credit card numbers, and banking details. The financial and personal toll of these attacks runs into billions of dollars annually, and the problem isn't getting any smaller.
To tackle this problem ,we built the Secure Phishing Detection and URL Analysis System. It is a full-stack web application that lets users check whether any URL they encounter is likely to be safe, suspicious, or malicious. The workflow is straightforward: users register an account, log in, and paste a URL. In the backend, the system runs seven automated security checks and produces a risk score out of 10, along with a human readable verdict.
Beyond the core detection feature, the project gave us a chance to practice secure software design and development. It includes designing a normalized database and building REST APIs to implement OWASP-recommended security controls. Everything is wired together through a clean, responsive frontend that communicates with the backend entirely through fetch() calls.
1.1 Project Objectives
•Build a fully functional web-based phishing detection application 
•Implement seven automated URL analysis checks backed by a transparent risk-scoring system
•Develop a secure authentication layer using JWT tokens and bcrypt password hashing
•Apply five OWASP security practices throughout the application to guard against common web threats
•SQLite database with four linked tables and complete CRUD coverage
•Integrate the frontend and backend

1.2 Technology Stack
We kept the tech stack lean and purposeful,no heavy frameworks or over-engineered dependencies, just the right tools for each layer of the application.

Component	Technology	What It Does
Frontend	HTML, CSS, JavaScript	User interface, forms, and API calls
Backend	Node.js + Express	REST APIs, business logic, authentication
Database	SQLite (better-sqlite3)	Persistent data storage with four related tables
Auth Tokens	JWT (jsonwebtoken)	Stateless, expiry-aware session management
Password Security	bcryptjs	Password hashing with 10 salt rounds


2. System Scope
This project covers a web-based URL analysis system designed to run in a local development environment. Its primary purpose is to demonstrate secure full-stack development principles.
2.1 What the System Covers
•User registration and login with JWT-based authentication
•URL submission and automated analysis across seven rule-based security checks
•Risk scoring out of 10, with Safe, Suspicious, or Phishing verdicts
•Per-user scan history with the ability to delete individual records
•An admin role with visibility into all scans from every user
•Five OWASP security practices throughout the application
