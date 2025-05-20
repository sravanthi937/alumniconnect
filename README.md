
# Alumni Association Platform

🛠️ Project Contributors
This alumni association platform was collaboratively developed by me and my team VIJAY VOLETY AND RAZIYA MOHAMMAD  as part of a team project to streamline alumni networking and engagement.


## Getting Started

### Prerequisites

- Node.js 18+ and npm
- PostgreSQL database

### Environment Setup

1. Copy the `.env.local.example` file to `.env.local`:

\`\`\`bash
cp .env.local.example .env.local
\`\`\`

2. Update the environment variables in `.env.local`:

\`\`\`
# Database
DATABASE_URL=postgresql://username:password@localhost:5432/alumni_db

# NextAuth
NEXTAUTH_URL=http://localhost:3000
NEXTAUTH_SECRET=your_nextauth_secret_key

# PayPal
NEXT_PUBLIC_PAYPAL_CLIENT_ID=your_paypal_client_id
PAYPAL_API_URL=https://api-m.sandbox.paypal.com
PAYPAL_ACCESS_TOKEN=your_paypal_access_token
\`\`\`

### Database Setup

1. Install dependencies:

\`\`\`bash
npm install
\`\`\`

2. Generate the database schema:

\`\`\`bash
npm run db:generate
\`\`\`

3. Push the schema to your database:

\`\`\`bash
npm run db:push
\`\`\`

Alternatively, you can run the migration script:

\`\`\`bash
npm run db:migrate
\`\`\`

### Running the Application

\`\`\`bash
npm run dev
\`\`\`

The application will be available at http://localhost:3000.

## Troubleshooting

### Database Connection Issues

If you encounter database connection issues:

1. Verify your PostgreSQL server is running
2. Check your DATABASE_URL in .env.local
3. Make sure you've run the database migrations
4. Try the test endpoint: http://localhost:3000/api/test-db

### Signup Issues

If you encounter issues during signup:

1. Check the server logs for detailed error messages
2. Verify your database schema is properly set up
3. Make sure all required environment variables are set



