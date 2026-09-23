# QueueLess

QueueLess is a zero-install hospital patient-flow web application.

The core problem:
OPD patients do not know when they will actually be seen because static tokens do not account for live queue depth, doctor consultation pace, breaks and priority interruptions.

## Core MVP

1. QR-linked patient web interface
2. Digital/live queue
3. Predictive waiting-time ETA
4. Doctor console
5. Real-time queue updates

## Later features

6. Patient journey
7. Hospital navigation
8. Admin dashboard
9. SMS fallback
10. Multi-department queues

## Technology

Frontend:
Next.js
React
Tailwind CSS

Backend:
Python
FastAPI

Database:
PostgreSQL
SQLAlchemy

ML:
Python
scikit-learn
Gradient-boosted regression

Real-time:
WebSockets

## User roles

PATIENT
DOCTOR
ADMIN
RECEPTION

## Important constraints

- Patient should not need to install an app.
- Patient should not need an account for the basic queue view.
- Do not store unnecessary medical information.
- Patient URLs must not expose raw database IDs.
- ETA should be a range, not fake precision.
- ML must have a fallback for new doctors/queues.
- Synthetic data must clearly be identified as synthetic.
- This is a prototype, not a clinical system.

## Original MVP scope

MUST:
Live ETA prediction engine
QR web interface
Doctor toggle console

SHOULD:
SMS fallback

COULD:
Multi-department admin view

WON'T YET:
Indoor AR/BLE navigation