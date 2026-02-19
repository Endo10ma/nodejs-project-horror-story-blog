# From the Other Side - Paranormal Sighting Platform

A Node.js web application for sharing and discovering paranormal encounters and ghost stories. Built with vanilla JavaScript and modern ES modules, this platform demonstrates server-side rendering, RESTful API design, and secure data handling.

## 🎭 Features

- **Story Submission**: Users can submit their paranormal encounters through a secure form
- **Story Viewing**: Browse through a collection of user-submitted ghost stories
- **Responsive Design**: Mobile-friendly interface with a spooky aesthetic
- **Security**: Input sanitization and validation to prevent XSS attacks
- **RESTful API**: Clean API endpoints for data management

## 🛠️ Tech Stack

- **Backend**: Node.js with ES modules
- **Frontend**: Vanilla HTML5, CSS3, and JavaScript
- **Security**: sanitize-html for input sanitization
- **Styling**: Custom CSS with Google Fonts integration
- **Data Storage**: JSON-based data persistence

## 🚀 Getting Started

### Prerequisites

- Node.js (v14 or higher)
- npm

### Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/horror-stories-blog.git
cd horror-stories-blog
```

2. Install dependencies:
```bash
npm install
```

3. Start the server:
```bash
npm start
```

4. Open your browser and navigate to `http://localhost:8000`

## 📁 Project Structure

```
horror-stories-blog/
├── handlers/              # Route handlers for API endpoints
│   └── routeHandlers.js   # GET and POST request handlers
├── public/                # Static assets and frontend files
│   ├── index.html         # Landing page
│   ├── sightings.html     # Story viewing page
│   ├── upload-sighting.html # Story submission form
│   ├── index.css          # Main stylesheet
│   └── *.js               # Frontend JavaScript files
├── utils/                 # Utility functions
│   ├── serveStatic.js     # Static file serving
│   ├── getData.js         # Data retrieval
│   ├── addNewSighting.js  # Data persistence
│   ├── sanitizeInput.js   # Input sanitization
│   └── ...                # Other utilities
├── data/                  # Data storage
├── server.js              # Main server file
├── package.json           # Project configuration
└── README.md              # This file
```

## 🔧 API Endpoints

### GET /api
- Retrieves all paranormal sighting stories
- Returns JSON array of story objects

### POST /api
- Accepts new paranormal sighting submissions
- Expects JSON payload with story details
- Returns created story object with 201 status

## 🛡️ Security Features

- **Input Sanitization**: All user inputs are sanitized using `sanitize-html`
- **XSS Prevention**: Malicious scripts are stripped from user submissions
- **Error Handling**: Comprehensive error handling for robust operation

## 🎨 Design Highlights

- **Spooky Theme**: Dark, atmospheric design perfect for horror stories
- **Responsive Layout**: Works seamlessly on desktop and mobile devices
- **Accessibility**: Semantic HTML5 with proper ARIA labels
- **Modern Typography**: Google Fonts integration for enhanced readability

## 📝 Example Story Submission

```json
{
  "title": "The Shadow in the Corner",
  "location": "Old Victorian House, Maine",
  "date": "2024-01-15",
  "story": "I saw a dark figure standing in the corner of my bedroom...",
  "witness": "Anonymous"
}
```

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the ISC License - see the package.json file for details.

## 👻 About

This project showcases modern Node.js development practices including:
- ES6 module system
- Async/await patterns
- RESTful API design
- Security best practices
- Modular architecture
- Static file serving
- Error handling and logging

Built with ❤️ and a healthy dose of spooky vibes by Haziq Hafizuddin.

---

**Note**: This is a demonstration project. All stories are fictional and for entertainment purposes only.
