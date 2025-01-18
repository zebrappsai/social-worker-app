# Social Worker Reporting Application Requirements

## 1. Overview
A mobile application designed to streamline the report generation process for social workers after family visits, utilizing voice input and AI-enhanced text processing. The application supports both Hebrew and Arabic interfaces while generating final reports in Hebrew.

## 2. Core Functionality Requirements

### 2.1 Input Methods
- Voice recording capabilities for real-time dictation
- Maximum recording length of 30 minutes in initial phase
- Real-time recording duration display showing:
  - Current recording time
  - Remaining available time in parentheses
  - Clear visual indicator of maximum allowed duration
- Option to upload pre-recorded audio files (within length limits)
- Text input capability as a fallback option
- Support for both Hebrew and Arabic voice input
- Offline recording capability with later synchronization

### 2.2 Language Processing
- Speech-to-text conversion supporting Hebrew and Arabic
- Real-time transcription display during recording
- Automatic language detection for voice input
- Translation capabilities from Arabic to Hebrew
- Text correction and editing capabilities

### 2.3 Report Generation
- AI-enhanced report formatting and structuring
- Converting any reporting style to formal, professional composition:
  - Preserving original information and content
  - Clear and accessible language (not overly formal)
  - Use of accepted professional terminology
  - Logical and readable structure
  - Avoiding flowery or overly complex language
- Learning and Adaptation System:
  - Retention of frequently used professional terms
  - Learning from user corrections and adjustments
  - Building personalized terminology database per user
  - Recognition of preferred phrasing patterns
- Advanced Composition Control:
  - Option to request report rephrasing
  - Specification of required changes (e.g., "less formal", "more concise")
  - Specific instructions for modifying particular sections
  - Composition version history tracking
- Customization Interface:
  - Shortcuts for common phrasing styles
  - Ability to save phrasing preferences as default
  - Capability to mark sections for rephrasing
  - Automatic suggestions for composition improvement
- Professional terminology integration
- Automatic categorization of report sections
- Key points extraction and highlighting
- Required fields validation

### 2.4 User Interface
- Persistent language toggle button (Hebrew/Arabic)
- Intuitive recording controls
- Real-time audio visualization
- Clear recording status indicators
- Draft saving and editing capabilities
- Preview functionality before final generation
- Dark/Light mode support

## 3. Technical Requirements

### 3.1 Performance
- Fast speech-to-text conversion (< 2 seconds delay)
- Efficient report generation (< 30 seconds)
- Smooth audio recording without gaps
- Minimal battery consumption
- Offline functionality for core features

### 3.2 Security
- End-to-end encryption for all data
- Secure authentication system
- Role-based access control
- Data privacy compliance
- Secure cloud storage for reports
- Local data encryption

### 3.3 Integration
- Cloud synchronization capabilities
- Export functionality (PDF, DOC formats)
- Backup and restore features
- API integration for external systems
- Share functionality with access control

## 4. Report Structure Requirements

### 4.1 Required Fields
- Visit date and time
- Family identification details
- Social worker details
- Visit location
- Present family members
- Main observations
- Recommendations
- Follow-up actions
- Risk assessments
- Resource referrals

### 4.2 AI Enhancement Features
- Automatic formatting of unstructured speech
- Professional terminology suggestions
- Grammar and style correction
- Contextual information addition
- Standardized structure enforcement
- Key points summarization
- Action items extraction

## 5. User Management Requirements

### 5.1 User Profiles
- Individual social worker profiles
- Department/Organization affiliation
- Customizable preferences
- Report templates customization
- Personal dictionary for frequent terms
- Historical report access

### 5.2 Administrative Features
- User management dashboard
- Report template management
- Usage statistics and analytics
- Quality assurance tools
- Batch report processing
- System configuration options

## 6. Accessibility Requirements
- Screen reader compatibility
- Voice command support
- Adjustable text sizes
- High contrast mode
- RTL/LTR support
- Keyboard navigation support
- Accessibility compliance

## 7. Data Management Requirements

### 7.1 Storage
- Secure cloud storage
- Local caching
- Automatic backup
- Version control for reports
- File attachment support
- Storage quota management

### 7.2 Report Management
- Search functionality
- Filtering options
- Categorization system
- Archiving capabilities
- Audit trail
- Bulk operations support

## 8. Quality Assurance Requirements
- Spell checking
- Grammar verification
- Professional terminology validation
- Report completeness checking
- Format consistency
- Language quality assessment
- Error detection and correction

## 9. Compliance Requirements
- Data protection regulations
- Social services standards
- Professional ethics guidelines
- Documentation standards
- Accessibility standards
- Security standards

## 10. Support Requirements
- In-app help system
- User documentation
- Training materials
- Technical support system
- Feedback mechanism
- Error reporting system
- Regular updates and maintenance

## 11. Proof of Concept (POC) Requirements

### 11.1 POC Scope
- Demonstration of core functionality flow:
  * Voice recording or audio file upload
  * Speech-to-text conversion
  * Basic text processing and report generation
  * Simple report preview and editing
  * Basic language switching (Hebrew/Arabic UI)

### 11.2 POC Technical Implementation
- Web-based implementation for easy sharing and testing
- Use of free AI services or open models:
  * OpenAI Whisper or similar for speech-to-text conversion
  * Open LLM or OpenAI API for report processing and composition
  * Hebrew and Arabic language support through appropriate AI models
- Additional free services:
  * Browser's built-in WebAudio API for recording
  * Local storage for recordings and drafts
  * Basic client-side processing
  * Client-side language detection
- Hybrid implementation:
  * Client-side UI and management components
  * AI processing on simple server or serverless service
  * API budget management for cost control

### 11.3 POC Features
- Recording and Speech Conversion:
  * Maximum 5-minute recording length for POC phase
  * Basic audio visualizer
  * Play/Pause/Stop controls
  * Recording timer display
  * Audio file upload option
  * AI-powered speech-to-text conversion
  * Conversion progress display
  * Manual editing of converted text

- Advanced Processing and Composition:
  * AI analysis of converted text
  * Converting any reporting style to formal, professional composition:
    - Preserving original information and content
    - Clear and accessible language (not overly formal)
    - Use of accepted professional terminology
    - Logical and readable structure
    - Avoiding flowery or overly complex language
  * Automatic key points identification
  * Automatic adaptation to standard report structure
  * Identification and marking of topics requiring special attention
  * Maintaining professional and objective tone
  * Ensuring consistency in composition throughout the report

- Language Support:
  * Basic Hebrew and Arabic UI elements
  * Language toggle functionality
  * Right-to-left (RTL) support
  * Speech conversion and composition in both languages
  * Automatic translation to Hebrew when needed

- Report Generation:
  * Professional report template
  * AI-enhanced formatting and composition
  * Preview capability
  * Manual editing of output
  * Multiple format downloads
  * Version history tracking

### 11.4 POC Limitations
- Limited offline functionality
- Basic speech recognition accuracy
- Simple text processing without AI enhancement
- Limited template options
- Basic error handling
- No cloud storage or synchronization
- No user authentication
- No data persistence between sessions
- Limited mobile responsiveness
- Limited AI API usage quota
- Potential waiting times for AI processing
- Accuracy dependent on AI model quality
- Language limitations based on available models

### 11.5 POC Success Criteria
- Successful demonstration of:
  * Voice recording and file upload
  * Basic speech-to-text conversion
  * Simple report generation
  * Language switching functionality
  * Basic user interface navigation
- Ability to generate a complete report from voice input
- Support for both Hebrew and Arabic input
- Functional UI in both languages
- Export capability for generated reports
- Learning and Adaptation System:
  * Successful retention of professional terms
  * Gradual improvement in phrasing accuracy
  * Adaptation to user's preferred style
- User Interface:
  * Ease of requesting rephrasing
  * Clarity in customization options
  * Helpful feedback on proposed changes

### 11.6 POC Deployment
- GitHub Pages hosting
- Single-page application (SPA)
- All dependencies included via CDN
- No installation requirements
- Cross-browser compatibility (latest versions)
- Shareable URL for easy access
- README with usage instructions

### 11.7 POC Documentation
- Setup instructions
- Usage guide
- Feature limitations
- Known issues
- Development setup guide
- Testing instructions
- Contribution guidelines