# Quest App

## Overview

Quest App is an interactive platform where users can create, participate in, and rate quests. The application supports user authentication, multimedia-rich tasks, real-time progress tracking, and a rating system.

### User Registration & Authentication
- Sign up via email or social networks
- User profiles with avatars and quest history

### Quest Creation
- Define quest name, description, number of tasks, and time limits
- Add multimedia elements (text, images, videos) to tasks
- Create various types of questions (open-ended, multiple-choice, image-based)

### Quest Participation
- Interactive task map
- Real-time progress tracking
- Timer for time-limited tasks

### Rating & Feedback
- Author rating system
- User reviews (star rating, comments)

## Technologies Used

### Backend (Spring Boot)
- Spring Boot (REST API, Security, JPA)
- Spring Security + OAuth2 (Authentication via email/social networks)
- PostgreSQL / MongoDB (Database)
- WebSocket (Real-time progress tracking)
- Flyway (Database migrations)
- Docker (Containerization)

### Frontend (React)
- React + React Router (Routing)
- Redux Toolkit / Zustand (State management)
- Tailwind CSS (Styling)
- Axios (API requests)
- Leaflet.js / Google Maps API (Interactive maps)
- Firebase / Auth0 (Authentication)

## Installation & Setup

URL : http://team-quests.surge.sh/

## API Endpoints

### Authentication
- `POST /auth/register` - User registration
- `POST /auth/login` - User login
- `GET /auth/me` - Get current user
- `POST /auth/social` - Social login

### Quests
- `POST /quests` - Create a quest
- `GET /quests/{id}` - Get quest details
- `GET /quests` - Get all quests
- `PUT /quests/{id}` - Update quest
- `DELETE /quests/{id}` - Delete quest

### Participation
- `POST /quests/{id}/start` - Start quest
- `POST /quests/{id}/submit` - Submit answer
- `GET /quests/{id}/progress` - Get current progress

### Ratings & Feedback
- `POST /quests/{id}/rating` - Submit rating
- `GET /quests/{id}/ratings` - Get all ratings

## License

This project is licensed under the MIT License.
