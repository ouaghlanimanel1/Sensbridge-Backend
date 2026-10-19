# Sensbridge Backend

## Overview
Backend architecture for the **Sensbridge** mobile application. This repository is organized as a monorepo containing multiple microservices built with **NestJS** and **Python** to handle core API logic, real-time sign language translation, and speech recognition.

## Services Architecture

- **`backend-sensbridge`**: Main NestJS API handling core application business logic, user management, and client endpoints.
- **`backend-sensbridge-pim-asl-translator`**: Python translation service for processing American Sign Language (ASL) data.
- **`signbridge_api`**: Additional service handling sign-language-specific API interactions.
- **`whisper-service`**: Python speech-to-text processing service powered by OpenAI Whisper.

## Technologies Used

- **Frameworks**: NestJS, Node.js, FastAPI / Flask (Python)
- **AI & Processing**: Python, OpenAI Whisper model
- **Communication**: REST APIs / WebSockets

## Getting Started

### Prerequisites

- Node.js (v18 or higher)
- Python (v3.9 or higher)
- npm / pip

### Installation & Running Services

Clone the repository and navigate into the project directory:

```bash
git clone https://github.com/ouaghlanimanel1/Sensbridge-Backend.git
cd Sensbridge-Backend

## Running the NestJS Main API (backend-sensbridge):

Bash
cd backend-sensbridge
npm install
npm run start:dev


## Running Python Services (e.g., whisper-service):

Bash
cd whisper-service
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
pip install -r requirements.txt
python main.py

Mobile Frontend
The Flutter mobile application repository can be found here:
https://github.com/ouaghlanimanel1/Sensbridge-Frontend
