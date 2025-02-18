# Jobly - Backend

## Overview

Jobly is a full-stack job board application that allows users to browse companies, view job listings, and apply for jobs. This is the **backend** repository, built with **Node.js and Express**.

**Repository URL:** [https://github.com/marialclark/JoblyBackend](https://github.com/marialclark/JoblyBackend)

## Tech Stack

- **Backend:** Node.js, Express
- **Database:** PostgreSQL (via Supabase or ElephantSQL)
- **Authentication:** JWT-based authentication
- **Hosting:** Render (for API deployment)

## Installation & Setup

1. **Clone the repository**
   ```sh
   git clone https://github.com/marialclark/JoblyBackend.git
   cd JoblyBackend
   ```

2. **Install dependencies**
   ```sh
   npm install
   ```

3. **Set up the database**
   - Ensure you have **PostgreSQL** installed or use a cloud database like **Supabase** or **ElephantSQL**.
   - Run migrations and seed the database:
     ```sh
     psql < jobly-schema.sql
     psql < jobly-seed.sql
     ```

4. **Run the server**
   ```sh
   node server.js
   ```
   The API will be available at `http://localhost:3001`

## Features

- **User Authentication:** Secure login and signup with JWT authentication
- **Companies API:** Fetch company details and job listings
- **Jobs API:** Retrieve and manage job postings
- **User Profiles:** View and update user profiles
- **Job Applications:** Track user applications to jobs

## Authentication & Security

- **JWT Authentication:** Users receive a **JWT token** upon login
- **Authorization Middleware:** Protects private routes
- **Environment Variables:** Stores database credentials and secret keys

## Contributors

- **Maria L. Clark** - Full-Stack Developer
