# CareNexus AI Hospital Assistant

## Project Overview
CareNexus is a Django-based web application for hospital management with an AI-powered assistant. The AI helps patients by suggesting doctors based on symptoms, finding blood donors by group, checking test fees, and verifying doctor availability. Admins have full access to patient data, while patients have limited views for privacy. This project is designed for university demonstrations and future AI-healthcare studies.

## Group Members
- Bashir Alam (Lead Developer - AI Integration & Backend)
- [Group Member 1 Name] - [Role, e.g., Frontend & Testing]
- [Group Member 2 Name] - [Role, e.g., Database & Documentation]

## Key Features
- User Registration & Login (Mobile for patients, password '000' for admin)
- AI Agent (OpenRouter Llama): Suggests doctors based on symptoms, finds blood donors, shows availability
- Role-Based Access: Admins see patient lists/counts, patients see only doctors/donors
- Doctor List View with specialty & schedule
- Blood Bank View with group & contact
- Patient Privacy: No sensitive patient info shared with non-admins

## Technologies Used
- Backend: Django
- AI: OpenRouter API with Llama 3-8b-instruct model (free tier)
- Database: SQLite (default, easy to migrate to PostgreSQL)
- Frontend: HTML/CSS/JS (basic templates with responsive design)
- Other: Requests library for API calls

## Installation & Setup
1. Install Python 3.10+
2. Copy the project folder
3. Open terminal in the folder
4. Set policy: `Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope Process`
5. Activate venv: `.\venv\Scripts\activate`
6. Install packages: `pip install django requests`
7. Migrate DB: `python manage.py makemigrations` then `python manage.py migrate`
8. Run server: `python manage.py runserver`
9. Open browser: http://127.0.0.1:8000/
10. API Key: Get from https://openrouter.ai/settings/keys and update in core/views.py

## Usage
- Register as patient with mobile number.
- Login as patient or admin ('000' for admin).
- Use AI agent to query: "হার্টের সমস্যা" → Doctor suggestion.
- "AB+ রক্ত চাই" → Matching donors.
- Admin can see patient count/list.

## Future Improvements
- Add bed management (department-wise available beds).
- Integrate test fees and outdoor/indoor services.
- Enhance AI for symptom-based recommendations and English fallback if Bengali not understood.
- Deploy on cloud (Heroku or Vercel) for online access.

## Contributing
- Clone the repo.
- Create a branch: `git checkout -b your-feature`
- Commit changes: `git commit -m "Added new feature"`
- Push: `git push origin your-feature`
- Open a Pull Request.

## License
MIT License - Feel free to use and modify.

## Acknowledgments
- Inspired by AI-healthcare projects.
- Thanks to OpenRouter for free API.
- Special thanks to Grok for development assistance.
=======

