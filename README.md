# Signal — Fenze Cloud HTML deployment test

An original, single-file HTML/CSS/JS landing page inspired by the modern technical style of TypeSafe AI's Jev site. The on-page decision demo runs local JavaScript heuristics only; it does not call any AI service.

## Local preview

Open `index.html` in a browser, or run `python3 -m http.server 8080` and visit `http://localhost:8080`.

## Deploy with Fenze Cloud

1. Create a new GitHub repository, e.g. `signal-fenze-demo`.
2. Push `index.html` and `README.md` to the repository's `main` branch.
3. In Fenze Cloud, create a new app on `interserver-vps`, choose the repo and the `StaticSite` stack, and set `/` as health path.
4. Assign a Fenze domain only after confirming the requested hostname is supported and routed to this server; otherwise use a custom hostname with DNS pointing to the server.
5. Deploy and verify the app is `Live` and responds over HTTPS.

This is not affiliated with TypeSafe AI or Jev.