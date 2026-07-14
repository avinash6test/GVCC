# Learnly MERN Learning Portal

Full-stack GVCC assignment built with React/Vite, Node/Express, and MongoDB/Mongoose. It supports videos, unlimited named bookmarks per video, click-to-seek, persistent watch progress, responsive layout, and bookmark deletion.

## Run

1. Start MongoDB locally or create an Atlas database.
2. Copy `server/.env.example` to `server/.env` and set `MONGODB_URI`.
3. Run `npm install`, then `npm run install:all`.
4. Run `npm run dev`, then open `http://localhost:5173`.

The server seeds three demo video records at its first startup.

## API

- `GET /api/videos`
- `GET` / `PUT /api/videos/:id/progress`
- `GET /api/bookmarks/video/:videoId`
- `POST /api/bookmarks`
- `PATCH` / `DELETE /api/bookmarks/:id`

## Screenshot deterrence

Browsers cannot guarantee blocking OS-level screenshots. The interface provides visible student watermarking, pauses the video and covers the content when focus is lost, and disables supported download/Picture-in-Picture browser controls. A production deployment should add authenticated users, expiring signed video URLs, DRM streaming (Widevine/FairPlay/PlayReady), and forensic watermarks.
