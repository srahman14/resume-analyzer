# Resume Analyzer

A web application that analyzes resumes against job descriptions using AI, providing feedback and scoring. Built with React, TypeScript, and Vite, it leverages Puter.js for file storage, AI processing, and user authentication.

## Features

- **Resume Upload**: Upload PDF resumes for personal feedback
- **AI-Powered Feedback**: Uses AI (current model: Gemini 2.5 Flash) to generate detailed feedback on how well a resume matches a job description (or if no job description is given, the resume is analyzed on its own).
- **Scoring System**: Receive a score based on resume-job fit.
- **User Authentication**: Secure login and authentication via Puter.js.
- **File Storage**: Store resumes and images securely using Puter.js file system.
- **Responsive UI**: Clean, modern interface with Tailwind CSS.

## Tech Stack

- **Frontend**: React, TypeScript, Vite
- **Styling**: Tailwind CSS
- **File Handling**: PDF.js for PDF to image conversion
- **Backend Services**: Puter.js (File Storage, AI, Authentication)
- **Routing**: React Router
- **Build Tool**: Vite

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/srahman14/resume-analyzer.git
   cd resume-analyzer
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Set up Puter.js:
   - Ensure you have a Puter.js account and API keys configured.

4. Run the development server:
   ```bash
   npm run dev
   ```

5. Open your browser to `http://localhost:5173` (or the port specified by Vite).

## Usage

1. **Authentication**: Start by logging in via the Auth page.
2. **Upload Resume**: Go to the Upload page, select a PDF resume, enter job details (company name, job title, description), and submit for analysis.
3. **View Results**: After anlaysis, you will be redirected to the Resume page to view your resume with feedback and scores.
4. **Home**: Overview of past resumes submitted for analysis.

## Routes

- **Home** (`/`): Landing page with an overview of the app.
- **Auth** (`/auth`): User authentication (login/signup).
- **Upload** (`/upload`): Upload and analyze a resume.
- **Resume** (`/resume`): View analyzed resumes and feedback.
- **Wipe** (internal): Route to wipe all user data (used for testing or reset).

## Project Structure

```
resume-analyzer/
├── app/
│   ├── components/
│   ├── lib/
│   ├── routes/
│   │   ├── auth.tsx
│   │   ├── home.tsx
│   │   ├── resume.tsx
│   │   ├── upload.tsx
│   │   └── wipe.tsx
├── constants/
├── public/
├── types/
```

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
