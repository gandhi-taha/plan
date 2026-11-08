# Plan

A personal planner for study, a side project, the gym and a language course, built around office hours. It runs in the browser, works offline and installs on Android as an app.

## What it does

- Builds each day around work hours, commute and evening classes, and moves things when a day gets too full
- Live "now / next" view, a focus timer with Pomodoro blocks, and a rest timer for the gym
- Quick add in plain English ("gym tomorrow 18:00", "call supervisor fri 10am weekly")
- Habit sheet and goals tracker in a spreadsheet layout, weekly review, streaks

## Private by design

The code here is generic. My own plan (dates, classes, goals) is in `vault.json`, encrypted with AES-256-GCM using a key derived from my password (PBKDF2-SHA256, 600,000 rounds). The app asks for the password and decrypts the plan in the browser; the password never leaves the device. Progress stays on the device, with an optional backup file.

## Run it

Open `index.html` through any static server, for example `python3 -m http.server`, then visit http://localhost:8000.
