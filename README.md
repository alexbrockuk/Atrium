# Atrium Project Guide for AI Assistants

## Project Context
Atrium is a closed-access social platform designed for cardiologists to securely discuss topics, share media, and collaborate. The platform uses invite codes to ensure only verified medical professionals can access the system.

## Repository Structure
- `/src/models/` - Database models for users, topics, posts, and attachments
- `/src/routes/` - API endpoints for authentication, discussions, and file uploads
- `/src/static/` - Frontend files including the Vue.js single-page application
- `/src/main.py` - Application entry point and configuration

## Development History
- Initial version: Basic doctor social platform with thread-based discussions
- Current version: Rebranded as "Atrium" with left navigation, topic management, and cardiologist-specific branding

## Customization Points
- Branding and subheading in `src/static/index.html`
- User registration fields in `src/models/user.py` and `src/static/index.html`
- Topic management in `src/routes/discussion.py`
- UI styling in the CSS section of `src/static/index.html`

## Deployment Information
- The platform is deployed at: https://rxlhyimcx8dk.manus.space
- Admin credentials: username: admin, password: admin123
- Initial invite code: DOCTOR123
# Atrium

# Atrium Development Roadmap

## Planned Enhancements
1. **Video Conferencing Integration**
   - Potential technologies: Jitsi Meet, OpenVidu
   - Implementation priority: Medium
   - Status: Researched options, not yet implemented

2. **AI Integration**
   - Potential features: Content analysis, adverse event monitoring
   - Implementation priority: Medium-High
   - Status: Conceptual, awaiting Claude API integration

3. **Transcription Services**
   - For video conversations and meetings
   - Implementation priority: Low
   - Status: Conceptual, dependent on video integration

## Technical Debt
- Current database is SQLite, may need migration to MySQL for production scale
- Authentication system needs email verification for production
- Media storage needs cloud integration for scalability
