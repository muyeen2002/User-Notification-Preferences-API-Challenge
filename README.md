## User Preferences and Notification Management API
A Nest.js API for managing user preferences and notifications. Includes CRUD operations, notification simulation, rate limiting, logging, and basic analytics.

# Features
User Preferences: Create, read, update, and delete preferences (e.g., marketing, newsletter, channels).
Notification Management: Simulate notifications, log results, and track statistics.
Validation: Email, timezone, enums, and required fields validation.
Testing: Unit and integration tests for services, validation, and API endpoints.
Deployment: Serverless deployment to Vercel or AWS Lambda.
# API Endpoints
User Preferences
POST /api/preferences – Create preferences
GET /api/preferences/:userId – Retrieve preferences
PATCH /api/preferences/:userId – Update preferences
DELETE /api/preferences/:userId – Delete preferences
# Notification Management
POST /api/notifications/send – Simulate notifications
GET /api/notifications/:userId/logs – View notification logs
GET /api/notifications/stats – Get statistics
## Setup
# Clone & Install:
bash
git clone https://github.com/<your-repo>/notification-api.git
cd notification-api
npm install
# Environment Setup:
Create .env with:
env
MONGO_URI=<your-mongodb-uri>
PORT=3000
# Run:
bash
npm run start:dev
## Testing
# Run Tests:
bash
npm run test
npm run test:e2e
# Deployment
Vercel
Install CLI:
bash
npm install -g vercel
# Deploy:
bash
vercel
