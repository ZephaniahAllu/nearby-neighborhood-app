# Nearby — Your Neighborhood App

Nearby is a responsive, single-page neighborhood community web app built with HTML, CSS, and vanilla JavaScript.

## Features

- Browse and join neighborhood groups
- Discover community events and RSVP
- Explore event locations using maps and directions
- Receive in-app notifications
- Resident and administrator interfaces
- Optional Google Maps API integration, with basic map and address lookup fallbacks
- Responsive design for desktop and mobile

## Run locally

Open `index.html` in a modern browser. No build step or package installation is required.

For local development, you can also run a static server:

```bash
python -m http.server 8000
```

Then open `http://localhost:8000`.

## Important limitations

This is a **front-end prototype**, not a production multi-user application. The app uses browser storage for data, so changes do not automatically synchronize between different devices or browsers. Role selection in a browser is not secure authentication or authorization. Do not use it to protect administrator functions or sensitive user data.

Google Maps integration is optional. If using a Maps API key, configure appropriate key restrictions and API quotas in Google Cloud; client-side keys are visible to visitors.

## Project structure

```text
nearby-neighborhood-app/
├── index.html   # Complete application: HTML, styles, and JavaScript
├── README.md    # Project documentation
└── .gitignore   # Common local and editor files to exclude
```

## Deployment

This static website can be hosted using GitHub Pages. In the repository, open **Settings → Pages**, select **Deploy from a branch**, then select the `main` branch and `/ (root)`.

## Next steps

To support genuine shared neighborhood data, accounts, and admin permissions, add a backend with authentication, a database, and server-side authorization.
