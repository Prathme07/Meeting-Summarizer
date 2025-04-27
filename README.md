# Meeting Summarizer

The **Meeting Summarizer** is a web application designed to help users effortlessly summarize meetings, manage action items, and streamline post-meeting tasks. It leverages AI-powered summarization, speech-to-text transcription, and integrates with Google services for seamless task management.

## Features
- **Audio Transcription**: Convert MP3 audio files into text.
- **Summarization**: Generate concise summaries of meeting transcripts.
- **Action Item Management**: Extract action items from the meeting summary and manage them effectively.
- **Filter Action Items**: Sort and filter action items by assignee.
- **Google Calendar Integration**: Set reminders and sync tasks with Google Calendar.
- **Follow-up Emails**: Automatically generate and send follow-up emails.
- **Google Sign-In**: Easy login using Google accounts.

## Technologies Used
- **Backend**: Python, Flask
- **Frontend**: HTML, CSS, JavaScript
- **AI**: Julep API (GPT-4)
- **Speech Recognition**: SpeechRecognition library
- **Google APIs**: Calendar, Gmail, OAuth

## Setup Instructions

### 1. Clone the Repository
Start by cloning the repository to your local machine:
```
git clone https://github.com/yourusername/meeting-summarizer.git
cd meeting-summarizer

```
2. Create a Virtual Environment
Next, set up a virtual environment for the project:

```
python -m venv venv
source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
```
3. Install Dependencies
Install the required dependencies by running:

```
pip install -r requirements.txt
```
4. Configure Environment Variables
Create a .env file in the root directory of the project and add the following details:

```
JULEP_API_KEY=your_julep_api_key
GOOGLE_CLIENT_ID=your_google_client_id
GOOGLE_CLIENT_SECRET=your_google_client_secret

```
5. Set Up Google OAuth
Go to the Google Cloud Console, create a new project, and enable both the Google Calendar API and Gmail API.

Create OAuth 2.0 credentials (Web application).

Download the credentials file and save it as credentials.json in the root directory of your project.

6. Run the Application
After setting everything up, start the application by running:

```
python app.py
```
Usage Instructions
- Open your browser and navigate to http://localhost:5000.
- Click on "Start Summarizing" to begin the summarization process.
- Sign in with your Google account.
- Upload an MP3 file or paste a transcript manually.
- Click "Summarize" to generate the meeting summary and action items.
- Manage your action items using the following buttons:
- Send Email: Draft and send a follow-up email.
- Set Reminder: Add the task to your Google Calendar.
- Copy: Copy the task details to the clipboard.
- Filter action items by assignee name using the input field.
