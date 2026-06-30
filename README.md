# WhiteSync — Collaborative Whiteboard

Real-time collaborative whiteboard app. Sign up, create a canvas, draw, share it with others, see edits live.

**Live demo:** https://white-board-app-inky.vercel.app/

## Run it locally

### Backend
```bash
cd Backend
npm install
```
Create `Backend/.env`:
```env
MONGO_URI=your_mongodb_uri
JWT_ACCESS_SECRET=any_random_string
GOOGLE_CLIENT_ID=your_google_oauth_client_id
RESEND_API_KEY=your_resend_api_key
```
```bash
npm run dev
```
Runs on `http://localhost:5000`.

### Frontend
```bash
cd Frontend
npm install
npm start
```
Runs on `http://localhost:3000`.

## Notes
- Email signup requires a [Resend](https://resend.com) API key (sends OTP verification codes).
- Google login requires a Google OAuth Client ID, set in both the backend `.env` and `Frontend/src/index.js`.
- Deployed using Render (backend) and Vercel (frontend).