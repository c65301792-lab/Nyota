fetch("https://nyota-backend.onrender.com/api/loans/apply", {
    method: "POST",
    headers: { "Content-Type": "application/json" },
    body: JSON.stringify({ ... })
})Project ready for download:

Directory: nyota-microfinance/

frontend/

index.html (Landing page + loan calculator + Paybill payment section)

dashboard.html (User loan dashboard)

css/styles.css (Bootstrap + custom styles)


backend/

server.js (Node.js + Express server)

routes/auth.js (User register/login)

routes/loans.js (Loan application + automatic approval)

routes/payments.js (Payment verification)

models/User.js (MongoDB User schema)

models/Loan.js (MongoDB Loan schema)

models/Payment.js (MongoDB Payment schema)

middleware/auth.js (JWT authentication middleware)

config/db.js (MongoDB connection)


.env.template MONGODB_URI=<Your MongoDB URI> JWT_SECRET=<Random secure key> PAYBILL_NUMBER=400200 ACCOUNT_NUMBER=01101398719001

package.json (with dependencies: express, mongoose, cors, body-parser, bcrypt, jsonwebtoken)

README.md (deployment instructions for Render + Netlify, setup MongoDB, environment variables, and connecting frontend to backend)

All code is pre-configured with:

Automatic loan approval logic

5% interest rate

Processing fee min 150/max 1000

Paybill auto-filled with your provided numbers

Auto-payment section scroll after calculation

Beginner-friendly deployment structure


You can now deploy backend to Render and frontend to Netlify using the included files and instructions.
