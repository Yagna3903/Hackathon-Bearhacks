# CareerCraftAI

A full-stack web application that helps users optimize their professional presence through AI-powered tools.

## Features

- **Resume Analysis & Generation**

  - AI-powered resume analysis
  - Custom resume generation based on job descriptions
  - Keyword extraction and optimization suggestions

- **Portfolio Generation**

  - GitHub profile analysis
  - Custom portfolio website generation
  - One-click deployment options

- **Social Media Content**

  - Platform-specific content generation
  - Hashtag suggestions
  - Post scheduling and management

- **Interview Preparation**
  - Question generation
  - Answer suggestions
  - Mock interview sessions

## Tech Stack

- **Backend**: Python, Flask, OpenAI API
- **Frontend**: Next.js, React, TypeScript
- **Database**: PostgreSQL
- **Styling**: Custom CSS, Tailwind CSS
- **Deployment**: Docker, AWS

## Prerequisites

- Python 3.9+
- Node.js 16+
- PostgreSQL
- OpenAI API key
- GitHub token (for portfolio features)

## Installation

1. Clone the repository:

```bash
git clone https://github.com/yourusername/Personal-Branding-Assistant.git
cd Personal-Branding-Assistant
```

2. Set up the backend:

```bash
# Create virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
cd backend
pip install -r requirements.txt

# Set up environment variables
cp .env.example .env
# Edit .env with your credentials
```

3. Set up the frontend:

```bash
# Install dependencies
cd frontend
npm install

# Set up environment variables
cp .env.example .env.local
# Edit .env.local with your API URL
```

## Running the Application

1. Start the backend server:

```bash
cd backend
python app.py
```

2. Start the frontend development server:

```bash
cd frontend
npm run dev
```

3. Access the application at `http://localhost:3000`

## Environment Variables

### Backend (.env)

```
OPENAI_API_KEY=your_api_key
PERPLEXITY_API_KEY=your_api_key
GITHUB_TOKEN=your_token
DATABASE_URL=your_database_url
```

### Frontend (.env.local)

```
API_URL=http://localhost:5000
```

## Project Structure

```
Personal-Branding-Assistant/
├── backend/
│   ├── app.py                 # Main Flask application
│   ├── services/              # Business logic layer
│   ├── routes/               # API endpoints
│   └── requirements.txt      # Python dependencies
└── frontend/
    ├── app/                  # Next.js application
    ├── components/          # React components
    └── package.json        # Node.js dependencies
```

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- OpenAI for providing the GPT API
- GitHub for the GitHub API
- The Flask and Next.js communities
