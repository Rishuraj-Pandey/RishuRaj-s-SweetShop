🍬 Sweet Shop Management System
A full-stack Sweet Shop Management System built using the MERN stack as part of the Incubyte TDD Kata assessment.
The project demonstrates RESTful API design, database persistence, authentication, role-based authorization, frontend integration, and Test-Driven Development (TDD).

📌 Project Objective
The objective of this project is to design, build, and test a production-ready application that manages sweet inventory for a shop.
It allows users to browse and purchase sweets, while admin users securely manage inventory operations.
This project strictly follows:
•	MERN stack architecture
•	Persistent database usage (no in-memory database)
•	JWT-based authentication
•	TDD (Red → Green → Refactor)
•	Clean coding practices
•	Transparent AI usage

🧩 Tech Stack
Backend
•	Node.js
•	Express.js
•	TypeScript
•	MongoDB + Mongoose
•	JWT Authentication
•	bcrypt (password hashing)
•	Jest + Supertest (testing)
Frontend
•	React
•	TypeScript
•	React Router
•	Axios
•	Responsive UI (CSS / Tailwind)

🔐 User Roles
Role	Capabilities
User	View sweets, search/filter, purchase sweets
Admin	Add, update, delete, and restock sweets

🚀 Features
Authentication
•	User registration
•	User login
•	JWT-based authentication
•	Role-based authorization
Sweets & Inventory
•	View all sweets
•	Search sweets by name, category, and price range
•	Purchase sweets (quantity decreases automatically)
•	Purchase disabled when quantity is zero
Admin Functionality
•	Add new sweets
•	Update sweet details
•	Delete sweets
•	Restock inventory
UI / UX
•	Clean and responsive design
•	Protected routes
•	Clear success and error messages
•	Mobile-friendly layout

🔗 API Endpoints
Auth
POST /api/auth/register
POST /api/auth/login
Sweets (Protected)
POST   /api/sweets            (Admin only)
GET    /api/sweets
GET    /api/sweets/search
PUT    /api/sweets/:id        (Admin only)
DELETE /api/sweets/:id        (Admin only)
Inventory (Protected)
POST /api/sweets/:id/purchase
POST /api/sweets/:id/restock  (Admin only)

🧪 Test-Driven Development (TDD)
The backend is developed using strict TDD methodology:
1.	Write failing tests (Red)
2.	Implement minimal logic (Green)
3.	Refactor for clean and maintainable code (Refactor)
Test Coverage Includes:
•	Authentication and authorization
•	Role-based access control
•	Sweet CRUD operations
•	Purchase and restock logic
•	Edge cases (zero quantity, unauthorized access, invalid IDs)

📁 Project Structure
sweet-shop/
│
├── backend/
│   ├── src/
│   │   ├── controllers/
│   │   ├── routes/
│   │   ├── models/
│   │   ├── services/
│   │   ├── middleware/
│   │   └── tests/
│   ├── app.ts
│   └── server.ts
│
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── services/
│   │   └── utils/
│   ├── App.tsx
│   └── index.tsx

⚙️ Setup Instructions
Backend Setup
cd backend
npm install
npm run test
npm run dev
Create a .env file:
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret

Frontend Setup
cd frontend
npm install
npm start

📊 Test Report
•	All backend tests pass successfully
•	Jest and Supertest used for API testing
•	Test cases cover both positive and negative scenarios

🤖 My AI Usage
AI Tools Used
•	VS Code AI Extension (Kilo)
•	ChatGPT
How AI Was Used
•	Generating initial boilerplate code
•	Assisting with test case structure
•	Architectural guidance and refactoring suggestions
Reflection
AI tools significantly improved development speed and code structure.
All AI-generated output was carefully reviewed, understood, and manually refined to ensure originality, correctness, and compliance with the assignment requirements.
AI was used as an assistant, not as a replacement for learning or decision-making.

📌 Notes for Interview
•	Persistent storage implemented using MongoDB
•	Authentication handled via JWT
•	Authorization enforced using role-based middleware
•	Backend developed using TDD principles
•	Frontend cleanly consumes REST APIs
•	AI usage is transparent and documented

🌐 Deployment (Optional)
Deployment link will be added if deployed on platforms like Vercel, Netlify, or AWS.

✅ Conclusion
This project demonstrates a real-world approach to full-stack development, combining backend robustness, frontend usability, testing discipline, and responsible AI usage, fully aligned with Incubyte’s TDD Kata requirements.



