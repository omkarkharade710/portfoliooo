# Portfolio Website

A modern, responsive portfolio website built with React (frontend) and Node.js/Express (backend).

## Features

- 🎨 Modern and responsive design
- ⚡ Fast and optimized with React and Vite
- 🎯 Smooth scrolling navigation
- 📱 Mobile-friendly layout
- 📧 Contact form with backend integration
- 🚀 RESTful API endpoints
- 💼 Skills showcase with progress bars
- 🎨 Project portfolio section

## Tech Stack

### Frontend
- React 19
- Vite
- Tailwind CSS
- React Icons

### Backend
- Node.js
- Express.js
- CORS enabled

## Project Structure

```
portfolio-website-using-react and nodejs/
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   │   ├── Navbar.jsx
│   │   │   ├── Hero.jsx
│   │   │   ├── About.jsx
│   │   │   ├── Skills.jsx
│   │   │   ├── Projects.jsx
│   │   │   ├── Contact.jsx
│   │   │   └── Footer.jsx
│   │   ├── App.jsx
│   │   └── main.jsx
│   └── package.json
├── backend/
│   ├── server.js
│   └── package.json
└── README.md
```

## Getting Started

### Prerequisites

- Node.js (v14 or higher)
- npm or yarn

### Installation

1. Clone the repository:
```bash
git clone <your-repo-url>
cd portfolio-website-using-react-and-nodejs
```

2. Install backend dependencies:
```bash
cd backend
npm install
```

3. Install frontend dependencies:
```bash
cd ../frontend
npm install
```

### Running the Application

1. Start the backend server:
```bash
cd backend
npm start
# or for development with auto-reload:
npm run dev
```
The backend will run on `http://localhost:5000`

2. Start the frontend development server (in a new terminal):
```bash
cd frontend
npm run dev
```
The frontend will run on `http://localhost:5173` (or another port if 5173 is busy)

3. Open your browser and navigate to the frontend URL.

## API Endpoints

### GET /api/portfolio
Returns portfolio data including:
- Personal information
- Skills with proficiency levels
- Projects with details
- Social links

### POST /api/contact
Handles contact form submissions.

**Request Body:**
```json
{
  "name": "John Doe",
  "email": "john@example.com",
  "subject": "Inquiry",
  "message": "Hello, I'd like to discuss a project..."
}
```

**Response:**
```json
{
  "success": true,
  "message": "Thank you for your message! I will get back to you soon."
}
```

### GET /api/health
Health check endpoint to verify server status.

## Customization

### Update Portfolio Data

Edit the portfolio data in `backend/server.js`:
- Personal information
- Skills and proficiency levels
- Projects details
- Social media links

### Styling

The frontend uses Tailwind CSS. Customize styles in:
- Component files for component-specific styles
- `src/index.css` for global styles

### Adding New Components

1. Create new component files in `frontend/src/components/`
2. Import and use them in `App.jsx`

## Environment Variables

Create a `.env` file in the `backend/` directory:

```env
PORT=5000
NODE_ENV=development
```

## Building for Production

### Frontend
```bash
cd frontend
npm run build
```
The built files will be in the `dist/` directory.

### Backend
The backend is ready for production. Consider:
- Using environment variables for configuration
- Adding error handling middleware
- Setting up email service for contact form (using nodemailer)
- Adding database integration if needed

## License

This project is open source and available under the MIT License.

## Contributing

Contributions, issues, and feature requests are welcome!
