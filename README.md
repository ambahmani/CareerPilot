# CareerPilot – AI-Powered Career Agent

**An AI-powered platform for resume analysis, job discovery, job matching, and application tracking.**

CareerPilot is a full-stack application designed to simplify and organize the job search process. It combines AI-powered resume analysis with job discovery, personalized application documents, and a centralized application tracker.

The project is built with a modular architecture, allowing new job data providers and AI capabilities to be integrated over time.

## Key Features

- **AI Resume Analysis:** Upload PDF or DOCX resumes and extract structured professional information using OpenAI.
- **Career Profile Management:** Review and edit extracted skills, work experience, education, and professional details.
- **AI Job Matching:** Compare a candidate's profile with job descriptions and receive AI-generated matching insights.
- **Tailored Resume Generation:** Generate and customize resumes for specific job opportunities.
- **Cover Letter Generation:** Create personalized cover letters based on job requirements.
- **Job Discovery:** Search for remote job opportunities through the Himalayas Jobs API.
- **Application Tracker:** Save job opportunities and track application progress through different stages.
- **Document Export:** Export generated application documents in PDF and DOCX formats.

## Technology Stack

| Layer | Technologies |
|---|---|
| Frontend | React, Vite, JavaScript |
| Backend | Python, FastAPI |
| Database | PostgreSQL |
| ORM & Migrations | SQLAlchemy, Alembic |
| AI Integration | OpenAI API |
| Job Data | Himalayas Jobs API |
| Containerization | Docker, Docker Compose |

## How It Works

1. Upload a resume.
2. Extract and review the AI-generated career profile.
3. Discover job opportunities or enter a job description manually.
4. Analyze compatibility between the candidate and the job.
5. Generate a tailored resume and cover letter.
6. Save opportunities and manage applications through the tracker.

## System Architecture

```text
                 React + Vite
                      |
                      v
                FastAPI Backend
                      |
          +-----------+-----------+
          |           |           |
          v           v           v
     PostgreSQL   OpenAI API   Job APIs
          |                       |
          v                       v
   Career Profiles          Job Discovery
   Job Matches
   Generated Documents
   Job Applications
```

## Running Locally

**Prerequisites:** Docker, Docker Compose, and an OpenAI API key.

1. Clone the repository.
2. Create a `.env` file based on the project's environment configuration.
3. Configure the required environment variables.
4. Start the application:

```bash
docker compose up -d --build
```

5. Open the frontend:

```text
http://localhost:5173
```

6. Access the backend API documentation:

```text
http://localhost:8000/docs
```

**Security:** Never commit API keys, passwords, `.env` files, or personal resume data to the repository.

## Project Status

**Active Development**

The current version supports resume processing, AI job matching, personalized document generation, job discovery, and manual application tracking.

### Planned Enhancements

- Integration with additional job data providers
- Improved job search filters and duplicate detection
- Job recommendations and matching improvements
- Enhanced analytics and application tracking
- Cloud deployment and scalability improvements

## Project Goals

CareerPilot is developed as a practical full-stack AI engineering project, with an emphasis on:

- Real-world AI integration
- REST API design
- Relational database modeling
- Modular backend architecture
- External API integration
- Containerized application development

## Disclaimer

CareerPilot is an independent software project and is not affiliated with LinkedIn, Indeed, Glassdoor, Adzuna, or Himalayas.

Job availability and accuracy depend on the external data providers. AI-generated results should be reviewed before use.

---

**CareerPilot – Making job searching smarter, more organized, and more efficient.**
