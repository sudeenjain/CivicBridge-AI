# CivicBridge AI

An AI-powered multilingual community assistant that improves access to public information and government schemes for underserved communities.

## Overview

CivicBridge AI bridges the information gap between rural and underserved communities and government programs. The platform provides accessible, multilingual support for discovering and applying to government schemes, scholarships, health programs, and job opportunities.

## Key Features

- **Multilingual Support**: English, Hindi, and Kannada language support
- **Voice Interaction**: Speech-based interface for users with limited literacy
- **Low-Bandwidth Optimization**: Designed for areas with limited internet connectivity
- **Personalized Recommendations**: AI-powered scheme matching based on user profiles
- **Step-by-Step Guidance**: Clear application instructions for government programs
- **Multi-Platform Access**: Available via web browsers and Android mobile app
- **Offline Capability**: Access previously viewed information without internet

## Target Users

- Rural students seeking scholarships and educational opportunities
- Farmers looking for agricultural support programs
- Low-income families accessing welfare schemes
- Senior citizens finding health and pension programs
- Job seekers discovering employment opportunities

## Core Capabilities

### Scheme Information Retrieval
Search and browse comprehensive information about government schemes including:
- Eligibility criteria
- Benefits and financial assistance
- Application deadlines
- Required documents
- Submission procedures

### Personalized Recommendations
Get scheme recommendations tailored to your profile based on:
- Age and location
- Income level
- Education and occupation
- Family size
- Special circumstances

### Application Assistance
Receive step-by-step guidance for applying to schemes:
- Document checklists
- Submission locations
- Contact information
- Progress tracking
- Status updates

### Accessibility Features
- Voice-based interaction for hands-free operation
- Screen reader compatibility
- Adjustable text sizes and high-contrast modes
- Keyboard navigation support
- Multiple language options

## Technology Stack

### Frontend
- Web: Responsive web application
- Mobile: Native Android application
- Voice: Speech-to-text and text-to-speech integration

### Backend
- API Gateway for request routing and authentication
- Microservices architecture for scalability
- RESTful APIs for client communication

### Data Storage
- Scheme database with comprehensive program information
- User profile database with encrypted sensitive data
- Content database for multilingual resources

### AI/ML Components
- Recommendation engine for profile-based matching
- Natural language processing for search queries
- Translation services for multilingual support

## Getting Started

### Prerequisites
- Node.js 18+ (for web application)
- Android Studio (for mobile development)
- Database (PostgreSQL recommended)
- Cloud storage for scheme data

### Installation

```bash
# Clone the repository
git clone https://github.com/sudeenjain/CivicBridge-Ai.git
cd civicbridge-ai

# Install dependencies
npm install

# Set up environment variables
cp .env.example .env
# Edit .env with your configuration

# Run database migrations
npm run migrate

# Start development server
npm run dev
```

### Configuration

Create a `.env` file with the following variables:

```
DATABASE_URL=postgresql://user:password@localhost:5432/civicbridge
API_PORT=3000
SPEECH_API_KEY=your_speech_api_key
TRANSLATION_API_KEY=your_translation_api_key
ENCRYPTION_KEY=your_encryption_key
```

## Project Structure

```
civicbridge-ai/
├── .kiro/
│   └── specs/
│       └── civicbridge-ai/
│           ├── requirements.md
│           ├── design.md
│           └── tasks.md
├── src/
│   ├── api/           # API Gateway and routes
│   ├── services/      # Business logic services
│   ├── models/        # Data models
│   ├── utils/         # Utility functions
│   └── config/        # Configuration files
├── web/               # Web frontend
├── mobile/            # Android mobile app
├── tests/             # Test suites
└── docs/              # Documentation
```

## Development

### Running Tests

```bash
# Run all tests
npm test

# Run unit tests
npm run test:unit

# Run property-based tests
npm run test:property

# Run integration tests
npm run test:integration
```

### Code Quality

```bash
# Lint code
npm run lint

# Format code
npm run format

# Type checking
npm run type-check
```

## Deployment

### Web Application

```bash
# Build for production
npm run build

# Deploy to cloud platform
npm run deploy
```

### Mobile Application

```bash
# Build Android APK
cd mobile
./gradlew assembleRelease
```

## API Documentation

API documentation is available at `/api/docs` when running the development server.

Key endpoints:
- `GET /api/schemes` - Search schemes
- `GET /api/schemes/:id` - Get scheme details
- `POST /api/recommendations` - Get personalized recommendations
- `POST /api/profile` - Create/update user profile
- `GET /api/guide/:schemeId` - Get application guide


### Development Workflow

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## Accessibility

CivicBridge AI is committed to accessibility:
- WCAG 2.1 Level AA compliance
- Screen reader support
- Keyboard navigation
- Voice interaction
- Multiple language support
- Low-bandwidth optimization

## Privacy & Security

- All sensitive user data is encrypted at rest
- HTTPS/TLS for data in transit
- No personal data shared with third parties
- Users can delete their data at any time
- Compliance with data protection regulations

## Roadmap

### Phase 1 (Current)
- Core scheme search and recommendations
- English, Hindi, Kannada support
- Web and Android platforms

### Phase 2 (Planned)
- Additional regional languages
- iOS mobile application
- SMS-based interaction for feature phones
- Integration with government portals

### Phase 3 (Future)
- AI chatbot for conversational assistance
- Document upload and verification
- Application status tracking
- Community forums and peer support



## Acknowledgments

- Government data sources and open data initiatives
- Open-source translation and speech recognition libraries
- Community feedback and user testing participants



---

**Mission**: Empowering communities through accessible information and bridging the gap between citizens and government services.
