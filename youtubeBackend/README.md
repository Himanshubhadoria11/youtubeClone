# **Backend: [youtubeBackend](https://github.com/Himanshubhadoria11/youtubeClone.git)**

The backend for the YouTube Clone project using Node.js, Express.js, and MongoDB. Handles user authentication, video and channel management, and comments with secure JWT-based authentication.

## Tech Stack
- Node.js
- Express.js
- MongoDB (Atlas)
- JWT (JSON Web Tokens)

## Live URLs

# Frontend [youtubeFrontend]-	  https://youtube-frontend-himanshu-bhadoria.vercel.app
# Backend [youtubeBackend]-	  https://youtubebackend-c26a.onrender.com

## API Endpoints

### User Routes: `/api/users`
- `GET /` - Get all users
- `GET /:id` - Get single user
- `POST /signup` - Register user (with avatar upload)
- `POST /login` - User login

### Video Routes: `/api/video`
- `GET /` - Get all videos
- `GET /:id` - Get single video
- `GET /search/:searchVideo` - Search videos
- `POST /addVideo` - Add video (protected)
- `PUT /likeVideo/:id/` - Like video
- `PUT /disLikeVideo/:id/` - Dislike video
- `DELETE /deleteVideo/:id/:cId/:uId` - Delete video
- `PUT /updateVideo/:id/:cId/:uId` - Update video

### Channel Routes: `/api/channel`
- `GET /` - Get all channels
- `POST /createChannel` - Create channel (protected)
- `GET /:id` - Get specific channel
- `PUT /updateChannel/:id/:uId` - Update channel (protected)
- `DELETE /deleteChannel/:id/:uId` - Delete channel (protected)
- `PUT /subscribeChannel/:id/:uId` - Subscribe to a channel (protected)

### Comment Routes: `/api/comment`
- `GET /` - Get all comments
- `GET /videoComments/:id` - Get comments for a video
- `POST /addComment` - Add comment
- `PUT /updateComment/:id/:vId/:uId` - Update comment
- `DELETE /deleteComment/:id/:vId/:uId` - Delete comment

## Installation

commands: 
  git clone https://github.com/Himanshubhadoria11/youtubeClone.git

  cd youtubeBackend
  
  npm install

  npm start

### Environment Variables
Create a `.env` file in the root:

PORT=5200
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret

### 🏃 **Run the Server**

command: npm start

Server runs on: [http://localhost:5200](http://localhost:5200)

## Project Structure

youtubeBackend/
├── config/
├── controllers/
├── models/
├── routes/
├── middleware/
├── server.js
├── .env
└── package.json


