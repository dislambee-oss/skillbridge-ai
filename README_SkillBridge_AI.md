# SkillBridge AI — An Intelligent Job Matching and Skill Gap Analyzer for Students

SkillBridge AI is a student-focused web application concept that helps users compare their stated technical skills with the requirements mentioned in internship and entry-level job descriptions. It aims to summarize matching skills, highlight potential skill gaps, and suggest learning activities.

## Live Demo

[https://jolly-skill-bridge-path.base44.app](https://jolly-skill-bridge-path.base44.app)

## Problem Statement

Students may struggle to translate job descriptions into a focused learning plan. SkillBridge AI is designed to make role requirements easier to interpret by comparing them with a student's skill profile and presenting potential gaps in an understandable way.

## Core Workflow

1. Enter current skills and select a target role.
2. Paste a job or internship description.
3. Identify recognized skills in the description.
4. Compare required skills with the student's profile.
5. Display matched skills, missing skills, and a match indicator when enough requirements are recognized.
6. Suggest learning topics or practice projects for relevant gaps.

## Key Modules

- Student skill profile
- Job-description analyzer
- Skill-match and skill-gap report
- Learning roadmap
- Optional progress tracking and analysis history, depending on the deployed configuration

## Development Platform

The application was developed and hosted using the **Base44 AI app builder**. The specific framework, persistence mechanism, and any AI integrations should be documented only after confirming them from the deployed app or Base44 project settings.

## Methodology

A transparent initial approach is to normalize text, recognize skills from a curated vocabulary, and compare the recognized requirements with the student's declared skills. An illustrative overlap score is:

`Match percentage = matched unique recognized skills / total unique recognized required skills * 100`

This score represents skill overlap only. It is not a probability of getting hired, a verified measure of proficiency, or a guarantee of employability. If a job description contains no recognizable skills, the app should request more detail rather than show a misleading score.

## Documentation

See [`SkillBridge_AI_Mini_Project_Documentation.pdf`](SkillBridge_AI_Mini_Project_Documentation.pdf) for the mini-project report, logical architecture, methodology, scope, validation checklist, limitations, and future enhancements.

## Validation Checklist

Before presenting or publishing the project, verify the following on the live application:

- [ ] Different skill profiles and job descriptions produce input-dependent results.
- [ ] Empty descriptions are handled clearly.
- [ ] Descriptions with no recognized requirements do not produce a misleading score.
- [ ] The matching score and its limitations are explained.
- [ ] Roadmap, progress, history, and persistence features are tested if enabled.
- [ ] The layout works on desktop and mobile screens.
- [ ] Screenshots in the repository are from the actual deployed application.

## Limitations

- Skill matching depends on which skills the analyzer recognizes and how job requirements are written.
- Keyword overlap does not measure practical ability, proficiency, experience, or soft skills.
- The tool does not independently verify job listings, employers, or user-provided skills.
- Persistence and external AI behavior depend on the deployed Base44 configuration.

## Future Improvements

- Evaluate a dedicated ML-based skill extraction or role-matching model on a labelled dataset.
- Add resume parsing, with careful handling of personal data.
- Add verified job-source integrations.
- Improve learning recommendations and progress tracking.
- Export analysis results and compare multiple job descriptions.

## Author Information

- **Student:** [Your Name]
- **Department:** CSE (AI/ML)
- **College:** [Your College Name]
- **Academic Year:** [Your Academic Year]

## Disclaimer

SkillBridge AI is intended as a career-planning aid. Its output should be treated as guidance rather than a hiring decision or a guarantee of employment outcomes.
