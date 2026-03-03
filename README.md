# Training Tracker

A full-stack web application for tracking training sessions and managing fitness goals.

## Project Structure

### Backend (Java)
- **Language**: Java
- **Build Tool**: Maven
- **Database**: MySQL
- **Location**: `backend/`

Key directories:
- `src/main/java/com/trainingtracker/` - Java application source code
- `src/main/resources/` - Configuration files
- `src/test/java/` - Unit tests
- `pom.xml` - Maven project configuration

### Database (SQL)
- **Type**: MySQL
- **Location**: `database/`

Files:
- `schema.sql` - Database schema and table definitions
- `migrations/` - Database migration scripts

### Frontend (HTML/CSS/JavaScript)
- **Language**: HTML, CSS, JavaScript (Vanilla)
- **Location**: `frontend/`

Structure:
- `index.html` - Main HTML page
- `css/styles.css` - Styling
- `js/api.js` - API client library
- `js/main.js` - Application logic
- `public/` - Static assets

## Setup Instructions

### 1. Database Setup
1. Install MySQL Server
2. Run the schema initialization:
   ```sql
   mysql -u root -p < database/schema.sql
   ```

### 2. Backend Setup
1. Navigate to the backend directory:
   ```bash
   cd backend
   ```
2. Build the project with Maven:
   ```bash
   mvn clean install
   ```
3. Run the application:
   ```bash
   mvn exec:java -Dexec.mainClass="com.trainingtracker.App"
   ```

### 3. Frontend Setup
1. Navigate to the frontend directory:
   ```bash
   cd frontend
   ```
2. Open `index.html` in a web browser or serve with a local HTTP server:
   ```bash
   python -m http.server 3000
   ```

## API Endpoints (To Be Implemented)

- `GET /api/sessions` - Get all training sessions
- `POST /api/sessions` - Create a new training session
- `DELETE /api/sessions/{id}` - Delete a training session
- `GET /api/goals` - Get all training goals
- `POST /api/goals` - Create a new training goal
- `DELETE /api/goals/{id}` - Delete a training goal
- `GET /api/user/profile` - Get user profile information

## Features

- [x] Database schema design
- [x] Frontend UI structure
- [ ] Java backend REST API implementation
- [ ] Database connection pooling
- [ ] Authentication and authorization
- [ ] Data validation
- [ ] Error handling

## Technologies Used

- **Frontend**: HTML5, CSS3, Vanilla JavaScript
- **Backend**: Java 11+, Maven
- **Database**: MySQL 8.0+

## Contributing

1. Create a feature branch
2. Commit your changes
3. Push to the branch
4. Create a Pull Request

## License

MIT License - See LICENSE file for details