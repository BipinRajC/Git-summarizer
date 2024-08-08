# AI-powered Git-Summarizer

### Overview
In an AI-driven software development landscape, code is being generated faster and more efficiently than ever before. However, this rapid pace can lead to a lack of awareness and understanding of the codebase, especially for managers, peer developers, and learners who need to stay informed about the latest changes. Our project bridges this gap by providing a **subscription-based tool** that utilizes AI to summarize and communicate codebase updates effectively.

This tool allows users to subscribe to any GitHub repository and select a role—Manager, Peer Developer, or Learner—each of which customizes the summary to meet specific needs. The system regularly fetches the latest commits, processes them through an **AI API** to generate a role-specific summary, and sends out these **summaries via email**. This ensures that every team member stays informed and aligned with the project's progress, enhancing both understanding and collaboration.

### Key Features
- _Role-Based Summaries_: Custom summaries tailored for Managers, Peer Developers, and Learners, providing the exact level of detail needed for each role.
- _Automated Updates_: The system automatically fetches the latest commits from GitHub repositories and generates AI-driven summaries.
- _Email Notifications_: Summaries are sent directly to the user's inbox, ensuring they stay up-to-date with minimal effort.
- _Custom Prompts_: Users can customize prompts to tailor the AI-generated summaries to specific needs.
- _User-Friendly Interface_: A simple and intuitive UI for subscribing to repositories and managing preferences.

### Use Cases
- _Managers_: Receive high-level summaries of code changes, focusing on project status and progress.
- _Peer Developers_: Get detailed technical summaries, including dependencies, algorithms, and libraries used.
- _Learners_: Obtain in-depth analysis of code updates, providing an educational resource to learn from high-quality, real-world code.
- _Stand-Up Meeting Replacement_: The tool can replace daily stand-ups by automatically summarizing completed tasks and updates.

### Tech Stack
Our project leverages a robust tech stack to ensure **scalability, efficiency, and seamless user experience**. The backend is built with _**NestJS**_, a powerful _Node.js framework_, coupled with _**MongoDB**_ for storing user subscriptions and repository data. We utilize the _**GitHub API**_ to fetch the latest commits, and _**AI Groq API**_ to generate intelligent, role-specific summaries. For the frontend, _**ReactJS**_ provides a dynamic and responsive user interface, making it easy for users to subscribe and manage their preferences. GitHub Actions streamline our DevOps processes, ensuring continuous integration and deployment, while _**NodeMailer**_ handles automated email delivery, sending customized summaries to users.

### Setup and Installation

1. Clone the Repository
```
git clone https://github.com/BipinRajC/Git-summarizer.git
cd Git-summarizer
```
2. Install Dependencies
```
cd Backend
npm install

cd Frontend
npm install
```
3. Set Up environment Variables
```
MONGO_URI=your_mongo_connection_string
GITHUB_API_TOKEN=your_github_api_token
AI_API_KEY=your_ai_api_key
EMAIL_SERVICE_API_KEY=your_email_service_api_key
```
4. Start Backend Server
```
cd backend
npm run dev
```
5. Start Frontend Server
```
cd frontend
npm start
```

### Usage
Visit the homepage to enter your email and subscribe to a GitHub repository.
Select your role (Manager, Peer Developer, Learner) and customize your preferences.
Sit back and let the system handle the rest! You’ll receive tailored summaries in your inbox based on the latest repository commits.








