# EcoReceipt
EcoReceipt scans receipts or invoices and instantly estimates the carbon footprint per purchase, shows trends, suggests greener alternatives, and rewards sustainable choices.

https://gemini.google.com/share/042733c6de2c

Project Description

EcoReceipt is a web-based application that helps users understand the carbon footprint of their everyday purchases. By uploading or taking a photo of a receipt, EcoReceipt extracts the items, estimates their CO₂ emissions, and presents a detailed breakdown of environmental impact. Users can track monthly footprints, categorize their purchases, and earn EcoCredits for sustainable choices.

Key Features:

OCR processing of receipts (Google Vision API or Tesseract.js fallback)
Per-item and total carbon footprint estimation
Dashboard showing monthly carbon impact, category breakdowns, and EcoCredits
Support for demo receipts for quick testing
Dockerized full-stack setup for local testing or deployment

Technologies Used

Frontend:
React + Vite — fast, responsive Progressive Web App (PWA)
CSS / Tailwind — styling and responsive layout
Demo assets — sample receipts, animated GIF walkthrough
Backend:
Node.js + Express — REST API for OCR, carbon estimation, and database
OCR:
Google Vision API — cloud-based OCR for high accuracy
Tesseract.js — local fallback for offline / demo mode
Carbon Estimation:
Local JSON lookup — for demo/testing
Climatiq API integration stub — for authoritative emission factors
Database: Supabase (PostgreSQL) — stores users, receipts, receipt items, EcoCredits
Unit Tests — Node.js Mocha/Chai for backend functions
DevOps / Deployment:
Docker + docker-compose — containerized backend and frontend
GitHub Actions CI — test automation and frontend build
Scripts — for creating GitHub repo, pushing code, and drafting releases

Supporting Assets

Designs / Mockups
Demo screenshots and UI previews in frontend/public/demo-receipts/
Animated GIF walkthrough: demo-assets/animated-demo.gif
Documentation
README.md — project overview and setup instructions
docs/narration_storyboard.md — 2–3 minute hackathon demo storyboard and narration script
docs/release_template.md — GitHub release template
RELEASE_NOTES.md — draft release notes and changelog
Database / Infra
Supabase SQL schema: infra/supabase_schema.sql
Local carbon lookup JSON: infra/carbon_lookup.json
Scripts
scripts/create_and_push_repo.sh — automated GitHub repo creation and push
scripts/gh_commands.sh — GitHub CLI commands for repo and release
