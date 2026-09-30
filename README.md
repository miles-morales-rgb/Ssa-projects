# SSA PROJECTS — COMPLETE FRONTEND + ADMIN

This package contains the complete static setup.

## 1. Public website repository

Upload everything inside `public/` to your PUBLIC website repository:

public/
  index.html
  projects.json
  team.json
  server.js

The public `index.html` is configured to fetch the central JSON data from the separate SSA-ADMIN repository.

Before publishing, replace YOUR-USERNAME in `public/index.html` with your real GitHub username.

## 2. SSA-ADMIN repository

Upload everything inside `ssa-admin/` to a separate GitHub repository named `SSA-ADMIN`:

ssa-admin/
  index.html
  projects.json
  team.json
  images/
    projects/
    team/

Put actual project images inside:
images/projects/

Put actual team member images inside:
images/team/

The JSON image paths should match those locations.

## 3. Projects JSON

Each project has:
title
category
location
shortDescription
description
imageUrl
featured
displayOrder

## 4. Team JSON

Each team member has:
name
role
imageUrl
quote
displayOrder

## 5. Admin functions

The admin can:
- Fetch projects from GitHub
- Fetch team members from GitHub
- Add project request
- Remove project request
- Add team member request
- Remove team member request
- Open a Gmail/mail client with structured request details

The admin does not directly write to GitHub. This is intentional: a GitHub write token must never be exposed in browser JavaScript.

## 6. Performance

The public page:
- Renders the main HTML/CSS first.
- Fetches projects.json and team.json asynchronously.
- Fetches both JSON files in parallel.
- Lazy-loads project/team images.
- Delays the heavy hero video until after initial rendering.

## 7. Local preview

In the public folder:

node server.js

Then open:

http://localhost:8000

Do not put passwords, GitHub tokens, API keys, or private credentials in the frontend or JSON files.
