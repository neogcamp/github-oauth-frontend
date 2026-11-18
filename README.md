# OAuth frontend

The React frontend for neoG Camp's GitHub OAuth lesson. It sends you to the backend's `/auth/github` route, receives the session cookie when you come back, and shows your GitHub profile using the token.

## Run it

1. Start the OAuth backend from the lesson. It must be running before you sign in.
2. Copy `.env.example` to `.env`. It points at the backend on port 4000 and at GitHub's API.
3. Install and start:

   ```
   npm install
   npm run dev
   ```

4. Open the URL Vite prints and choose "Sign in with GitHub".

## What to read

- `src/components/Home` starts the sign-in.
- `src/lib/axios.lib.js` holds the two API clients: your backend and GitHub's.
- `src/components/OwnerProfile` shows the signed-in user's profile.

Part of the neoG Camp curriculum.
