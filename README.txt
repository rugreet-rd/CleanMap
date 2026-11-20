CLEANMAP V1 — HTML/CSS/JavaScript prototype

FILES
- index.html: page structure and project information
- style.css: responsive styling
- app.js: Leaflet map, pin creation, image compression, cleanup history

RUN
Open index.html in a modern browser with internet access. For reliable browser geolocation, serve it over HTTPS or localhost.

IMPORTANT LIMITATIONS
1. Pins, photos and history are saved only in this browser's localStorage. They are NOT shared with other visitors or uploaded to a server.
2. Google sign-in is a placeholder. Secure Google OAuth requires an authentication provider/backend.
3. A shared public launch needs a database, shared photo storage, access rules and abuse-reporting/security controls.
4. Address lookup uses the public Nominatim reverse-geocoding endpoint. Use it sparingly and follow its usage policy; it is not an unlimited production service.
5. OpenStreetMap tiles require attribution and are subject to the public tile usage policy.
6. Images are resized/re-encoded in the browser to reduce size and strip most source metadata. Production must also validate uploads server-side.
7. The browser's localStorage has limited capacity. Large photos or many records may fill it.

EDIT CONTACT EMAIL
Replace EDIT_EMAIL_HERE in index.html with your email address.

NEXT BACKEND STEP
Connect Supabase or another backend for real Google authentication, shared public data, photo storage, row-level security, abuse reporting and public reads. Never place a privileged service-role key in browser JavaScript.
