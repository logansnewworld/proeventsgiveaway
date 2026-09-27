# Expo Lead Capture & Prize Giveaway System

A modern, web-based lead capture and live prize draw system designed for exhibition booths and events. Powered by **Supabase** for backend data storage and **Tailwind CSS** for styling.

## Features
- **Visitor Form (`index.html`)**: Mobile-friendly questionnaire accessed via QR code[cite: 2]. Captures contact details, custom user interests, service ratings (1-5), and includes built-in duplicate entry prevention[cite: 2]. Features a strict privacy disclaimer.
- **Admin Prize Ticker (`admin.html`)**: A high-energy rolling ticker tube dashboard that fetches leads from Supabase and allows booth staff to spin and pick winners live[cite: 1].

## Setup & Installation
1. Upload all files (`index.html`, `admin.html`, and `logo.png`) to your GitHub repository root directory.
2. Set up a Supabase project and create a table named `expo_leads` with the following columns:
   - `id` (UUID, Primary Key)
   - `full_name` (Text)
   - `email` (Text)
   - `phone` (Text)
   - `company` (Text)
   - `interests` (Text)
   - `rating` (Integer)
   - `created_at` (Timestamp)
3. Deploy your repository using **GitHub Pages** or any static web hosting provider (like Vercel or Netlify).
4. Generate a QR code pointing to your live `index.html` URL for visitors to scan at your stand!