# Recipe_Finder_Frontend-Website

🍳 Recipe Finder — Interactive Web App

An elegant, responsive, and interactive Recipe Finder web application that lets users search for recipes by ingredients, apply dietary filters (vegetarian/vegan), and save their favorite dishes — all in real time. The app can work both online (with Spoonacular API) or offline in demo mode using built-in data, making it perfect for presentations or portfolio showcases.

🌟 Overview

The Recipe Finder project is a fully functional front-end web application designed with a focus on usability, visual aesthetics, and clean code architecture.
Users can simply enter available ingredients (e.g., “chicken, tomato, garlic”) and discover matching recipes instantly. The system fetches recipes either via the Spoonacular API or from local demo data when API access is unavailable.

It includes features like:

Recipe search with intelligent filtering

Beautiful recipe cards with smooth animations

Favorites management using localStorage

Interactive recipe modal with full details

Dark mode and demo mode toggle

Fully responsive layout for all screen sizes

🧩 Project Structure
📁 Recipe Finder
│
├── index.html        # Main HTML file (structure, layout, meta, components)
├── style.css         # Custom CSS for enhanced styling and UI elements
├── script.js         # JavaScript logic: search, API calls, UI updates, favorites, etc.
└── assets/           # (optional) folder for additional media, if needed

💡 Features Explained
🔍 Smart Recipe Search

Users input one or more ingredients.

Filters allow narrowing down results (vegetarian, vegan, or cuisine type).

Fetches live data using the Spoonacular API when an API key is provided.

Works seamlessly in Demo Mode for offline usage with built-in sample recipes.

🧠 Intelligent Demo Mode

When no API key is added, the app auto-switches to demo mode.

Displays a set of curated recipes from local data (DEMO_RECIPES array).

Ideal for classroom demos, offline presentations, or learning environments.

💾 Favorites Management

Users can save and remove favorite recipes using a heart button.

All favorites persist via browser localStorage.

A dedicated favorites section displays saved items neatly.

🪄 Modal Recipe Details

Clicking “View” on any recipe card opens a modal.

Shows complete ingredients, preparation instructions, and images.

Option to save or remove the recipe from favorites directly from the modal.

🌗 Dark Mode Toggle

Switch between light and dark themes instantly.

Uses smooth transitions for a pleasant user experience.

⚙️ Built-in Filters

Vegetarian / Vegan checkboxes

Cuisine dropdown (Indian, Italian, Chinese, Mexican, American)

Responsive search bar and filters adapt to any device size.

🧰 Technologies Used
Category	Tools / Libraries
Frontend Frameworks	HTML5, CSS3, JavaScript (ES6)
Styling & Layout	Bootstrap 5, Tailwind CSS, Custom CSS
Icons	Font Awesome 6
Animations	AOS (Animate On Scroll)
API Integration	Spoonacular API (optional, requires API key)
Storage	LocalStorage (for favorites)
UI Enhancements	Responsive Navbar, Modals, Dynamic Cards
🧑‍💻 How to Run Locally

Clone or download this repository:

git clone https://github.com/your-username/recipe-finder.git
cd recipe-finder


Open the project in your preferred IDE or code editor (e.g., VS Code).

Run the project:

Simply open index.html in your browser.

No server setup required for demo mode.

For live API mode, follow the next step.

(Optional) Enable Live Recipe Search:

Sign up at Spoonacular API
.

Get your API key.

Open script.js and replace the demo key with your actual key:

const SPOONACULAR_KEY = "YOUR_API_KEY_HERE";


Reload the browser to enable live recipe fetching.

📱 Responsive Design

Fully mobile-first design built using Bootstrap Grid System and Tailwind utilities.

Works seamlessly across:

Mobile phones

Tablets

Laptops and Desktops

🎨 UI Highlights

Modern glass-like card interface with hover animations

Subtle gradient backgrounds and shadows

Minimalist navigation bar with theme toggle

Eye-catching AOS scroll animations for each recipe card

🧠 Code Highlights

Clean modular JavaScript (organized in logical sections)

Uses async/await for smooth API handling

Maintains consistent UI state with clear DOM manipulation

Built-in utility functions for rendering cards, favorites, and modal content

Performance-friendly event listeners and cached references

💾 Data Storage

Favorites are stored locally using:

localStorage.setItem('rf_favorites', JSON.stringify(favorites));


This ensures that user preferences remain saved even after browser reloads.

🔐 API Information

To use the live mode, the application connects to Spoonacular’s RESTful API:

https://api.spoonacular.com/recipes/findByIngredients


Parameters include:

ingredients — user-input ingredients (comma-separated)

number — number of results to fetch

apiKey — your personal API key

🚀 Future Enhancements

Integration with meal planning and nutrition APIs

Advanced shopping list and meal prep mode

Recipe upload and community sharing feature

Integration with Firebase or MongoDB for real-time sync

Progressive Web App (PWA) optimization for offline caching

👨‍🎨 Author

Developed by: [Your Name]
Role: Frontend Developer / Web Designer
Contact: [your.email@example.com
]
GitHub: https://github.com/your-username

🏁 License

This project is released under the MIT License.
You are free to modify, distribute, and use it for both personal and commercial projects with proper attribution.
