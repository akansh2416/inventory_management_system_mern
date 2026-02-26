📦 Inventory Management System – MERN CRUD (Dockerized + Manual Setup)




A full-stack MERN CRUD application that allows users to:

➕ Insert products

📋 View products

✏️ Update products

❌ Delete products

This project supports:

🐳 Dockerized Setup (Recommended)

💻 Manual Local Setup

🧰 Tech Stack

MongoDB

Express.js

React.js

Node.js

Docker & Docker Compose

🐳 Run With Docker (Recommended)
✅ Prerequisites

Make sure you have installed:

Docker

Docker Compose

Check versions:

docker --version
docker compose version
📥 1. Clone the Repository
git clone https://github.com/akansh2416/inventory_management_system_mern.git
cd inventory_management_system_mern
🚀 2. Start All Containers

From the root directory (where docker-compose.yml is located):

docker compose up --build

This will:

Build frontend container

Build backend container

Pull MongoDB image

Create Docker network

Start all services

🌐 Access the Application (Docker Mode)
Service	URL
Frontend	http://localhost:3000

Backend	http://localhost:3001

MongoDB	mongodb://localhost:27017
🛑 Stop Containers
docker compose down

Reset database (remove volumes):

docker compose down -v
💻 Run Without Docker (Manual Setup)
To Run App:
1️⃣ Open the folder in VS Code and run:
npm install
2️⃣ In MongoDB Compass:

Create Database: IMS

Collection Name: products

3️⃣ Open two terminals in split:

https://github.com/mhy20401/Inventory-Management-System-MERN-CRUD-Project/assets/99351091/86ed0828-84b8-43b0-89fd-8caa17b88833

4️⃣ In one terminal run these commands (For Backend / Server):
cd Backend
npm run server

Backend runs on:

http://localhost:3001
5️⃣ In the other terminal run these commands (For Frontend / Client):
cd Frontend
cd inventory_management_system
npm start

Frontend runs on:

http://localhost:3000

https://github.com/mhy20401/Inventory-Management-System-MERN-CRUD-Project/assets/99351091/93fa528b-bc88-49c2-9922-19b317336b7c

📡 API Endpoints

Base URL:

http://localhost:3001
Method	Endpoint	Description
GET	/products	Display all products
POST	/insertproduct	Insert new product
PUT	/updateproduct/:id	Update product
DELETE	/deleteproduct/:id	Delete product

Example:

http://localhost:3001/products
🧪 Application Output
1️⃣ GET (Displaying products)

https://github.com/mhy20401/Inventory-Management-System-MERN-CRUD-Project/assets/99351091/09f7d43a-344b-4122-b415-b3736307cf45

2️⃣ POST (Inserting a new product)

https://github.com/mhy20401/Inventory-Management-System-MERN-CRUD-Project/assets/99351091/d31e9f36-c119-4a04-9cc0-ddc9fe94b159

https://github.com/mhy20401/Inventory-Management-System-MERN-CRUD-Project/assets/99351091/39ec387f-5efc-4c1f-a7eb-a87612acc17a

https://github.com/mhy20401/Inventory-Management-System-MERN-CRUD-Project/assets/99351091/a6b5c6bf-77d7-41ab-9ca0-3a8bfc71954d

https://github.com/mhy20401/Inventory-Management-System-MERN-CRUD-Project/assets/99351091/3d43e877-c2e6-414b-bef9-410caae1668e

3️⃣ PUT (Updating a product)

https://github.com/mhy20401/Inventory-Management-System-MERN-CRUD-Project/assets/99351091/d35f7ab0-3fda-4b1c-9055-67ca8c7b2ab6

https://github.com/mhy20401/Inventory-Management-System-MERN-CRUD-Project/assets/99351091/7dd107db-6fde-416d-b5c6-2175916f872f

4️⃣ DELETE (Deleting a product)

https://github.com/mhy20401/Inventory-Management-System-MERN-CRUD-Project/assets/99351091/d846ff43-6abd-4baa-9ed6-df736f2d411e

https://github.com/mhy20401/Inventory-Management-System-MERN-CRUD-Project/assets/99351091/cc6368bd-f391-4d6b-b814-c931d48a0878

🏗 Docker Architecture Overview
Browser (localhost:3000)
        ↓
Frontend Container
        ↓
Backend Container (port 3001)
        ↓
MongoDB Container (port 27017)
📂 Project Structure
Inventory-Management-System-MERN/
│
├── Backend/
├── Frontend/
├── docker-compose.yml
└── README.md
👨‍💻 Author

Akansh
