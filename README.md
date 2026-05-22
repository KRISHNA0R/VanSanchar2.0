# VanSanchar - Wildlife Conflict Coordination Platform

VanSanchar is an advanced, real-time platform designed to manage and coordinate wildlife conflicts and reporting. It acts as a bridge between citizens and forest officials, enabling rapid response to wildlife incidents to protect both human communities and endangered animals.

## Key Features

- **Citizen Portal**: Easy-to-use interface for citizens to report wildlife sightings, injured animals, or other forest-related incidents.
- **Officer Portal**: A comprehensive dashboard for forest officials to view, manage, and respond to incidents in real-time.
- **Offline First**: Reports can be filed offline. The app saves the data locally and automatically syncs it to the backend once an internet connection is restored.
- **Mandatory GPS Location**: For accurate tracking, incident reporting enforces capturing the user's real-time GPS coordinates before enabling photo uploads and text descriptions.
- **Interactive Maps & Real-time Alerts**: GIS map integration to display incident hotspots and alert notifications.
- **AI Analytics & Voice Reporting**: Integration with AI analytics for predictive modeling and support for attaching voice messages to reports.

## Tech Stack

- **Frontend**: React, Tailwind CSS, Framer Motion (for animations), Lucide React (for icons)
- **Backend**: Supabase (PostgreSQL, Realtime Subscriptions, Authentication)
- **Mapping**: Leaflet / React-Leaflet
- **Bundler**: Vite

## Setup Instructions

1. Clone the repository:
   ```bash
   git clone https://github.com/KRISHNA0R/VanSanchar_Hackstreet-.git
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Setup Environment Variables:
   Create a `.env` file in the root of the project with your Supabase credentials:
   ```env
   VITE_SUPABASE_URL=your_supabase_url
   VITE_SUPABASE_ANON_KEY=your_supabase_anon_key
   ```

4. Run the development server:
   ```bash
   npm run dev
   ```

## Workflow Highlights

- **OTP Authentication**: Simple login flow (use `123456` to test locally) differentiating between Citizen and Officer roles based on verified credentials.
- **Robust Reporting**: The `ReportScreen` requires GPS coordinates strictly before enabling submission, ensuring quality data.

## License

This project was built during the Hackstreet hackathon.
