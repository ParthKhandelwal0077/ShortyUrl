# ShortyURL

A full-stack URL shortening service built with Spring Boot and React.js. This application allows users to create short, memorable URLs from long ones, making them easier to share and manage.

## 🚀 Features

- **URL Shortening**: Convert long URLs into short, manageable links
- **Real-time List View**: See all your shortened URLs in a clean, organized list
- **Session-based Storage**: URLs are stored in session storage for the current session
- **RESTful API**: Clean and efficient API endpoints for URL management
- **Cross-Origin Support**: CORS enabled for all origins, methods, and headers
- **Secure Slug Generation**: Uses JNanoId for generating unique, secure slugs

## 🛠️ Technology Stack

### Frontend
- **React.js**: For building reusable UI components
- **Bootstrap 5**: For responsive and modern styling
- **Axios**: For efficient API request handling
- **Session Storage**: For temporary data persistence

### Backend
- **Spring Boot**: For robust and scalable REST API
- **Java**: For type-safe and object-oriented programming
- **JNanoId**: For generating unique URL slugs
- **In-memory Storage**: For URL mapping (can be extended to use a database)

## 📋 API Endpoints

- `POST /slugs`: Create a new shortened URL
- `GET /slugs`: Retrieve all shortened URLs
- `GET /{slug}`: Redirect to the original URL

## 🏗️ Architecture

The application follows a client-server architecture with clear separation of concerns:

### Frontend Structure
- **URLShortnerForm**: Component for URL input and shortening
- **SlugList**: Component for displaying shortened URLs
- **Service Layer**: Handles API communication and data management

### Backend Structure
- **REST Controllers**: Handle HTTP requests
- **Service Layer**: Business logic implementation
- **In-memory Storage**: URL mapping storage
- **CORS Configuration**: Cross-origin resource sharing setup

## 🔄 Development Workflow

The project follows a structured branching strategy:

- **main**: Production code branch (no direct commits)
- **release/{version}**: Release management branch
- **feature/{feature-name}**: Feature development branches

## 🚀 Getting Started

### Prerequisites
- Java 17 or higher
- Node.js and npm
- Git

### Backend Setup
1. Navigate to the Backend directory
2. Run `./gradlew build`
3. Start the application with `./gradlew bootRun`

### Frontend Setup
1. Navigate to the Frontend directory
2. Install dependencies: `npm install`
3. Start the development server: `npm start`

## 🔒 Security Features

- Secure slug generation using JNanoId
- CORS configuration for safe cross-origin requests
- Session-based storage for temporary data

## 📈 Performance Considerations

- Spring Boot's efficient request handling
- In-memory storage for fast URL lookups
- Optimized slug generation with collision probability management


## 📝 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 👥 Author

Parth Khandelwal

## 🙏 Acknowledgments

- JNanoId for secure slug generation
- Spring Boot team for the excellent framework
- React.js community for the frontend library


