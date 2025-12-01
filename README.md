# 
# 🏏 Interactive Cricket Tournament Manager

A web-based application built with vanilla JavaScript to manage cricket tournaments. This tool handles the entire flow of a tournament, from team registration and league stage fixtures to automatic points table calculations and knockout progressions (Semi-Finals & Finals).

## 🚀 Features

- **Dynamic Team Setup:** Accepts a user-defined number of teams (Minimum 4).
- **Round Robin Scheduling:** Automatically generates a "Play-All" fixture list where every team plays every other team once.
- **Interactive Dashboard:**
  - **Manual Result Entry:** Users click to select match winners rather than random simulation.
  - **Live Points Table:** Updates instantly after every match, sorting teams by Points first, then Wins.
- **Automated Knockout Stage:**
  - Automatically identifies the Top 4 teams.
  - Schedules Semi-Finals (Rank 1 vs Rank 4, Rank 2 vs Rank 3).
  - Progresses winners to the Grand Final to declare a Champion.

## 🛠️ Tech Stack

- **HTML5:** Structure and layout.
- **CSS3:** Flexbox for alignment, animations for the champion reveal, and a clean green/white color scheme.
- **JavaScript (ES6):** Core logic for state management, fixture generation algorithms, and DOM manipulation.

## ⚙️ How It Works (The Logic)

### 1. Fixture Generation (Round Robin Algorithm)
The application uses a **Nested Loop** approach to generate unique pairs for the league stage.
