# Plan

A personal planner for study, a side project, the gym and a language course, built around office hours. It runs in the browser, works offline and installs on Android as an app.

## What it does

- Builds each day around work hours, commute and evening classes, and moves things when a day gets too full
- Live "now / next" view, a focus timer with Pomodoro blocks, and a rest timer for the gym
- Quick add in plain English ("gym tomorrow 18:00", "call supervisor fri 10am weekly")
- Habit sheet and goals tracker in a spreadsheet layout, weekly review, streaks

## Private by design

The code here is generic. My own plan (dates, classes, goals) and my progress live in a private repository. The app signs in with a fine-grained GitHub token that can only read and write that one repository, keeps the token on the device, and syncs progress there automatically. Without access to the private repo, the app shows only a sign-in screen.

## Run it

Open `index.html` through any static server, for example `python3 -m http.server`, then visit http://localhost:8000.
