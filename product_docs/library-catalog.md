# Personal - Physical Media Library

## Background

I have a physical media library consisting of Books, DVDs/BluRays, Games, VHS, and Vinyl. It is hard to remember what all I have since its not all physically on a shelf or easily in sight. I'd like to have a way to collect and visualize my collection in a single location or app.

### User Stories

1. As a user, I want to have a single application that allows me to visualize my physical media collection, so that it can be curated in a catalog.
   1. As a user, I want to store books, so they can be curated in a catalog
   2. As a user, I want to store blu-rays, so they can be curated in a catalog
   3. As a user, I want to store DVDs, so they can be curated in a catalog
   4. As a user, I want to store Games, so  they can be curated in a catalog
   5. As a user, I want to store VHS tapes, so they can be curated in a catalog
   6. As a user, I want to store Vinyl records, so they can be curated in a catalog
2. As a user, I want to scan physical media with my phone camera, so that I can quickly add my items to the catalog.
3. As a user, I want to have a wishlist for each media type (books, dvds, etc...)

### Phase 1

The initial phase 1 will use a Google Sheet as a template for the catalog data. The goal is to standup the initial database and API that serves as the internal platform to the whole product.

1. Focus on user story 1.1 - books only
2. I have a Google Drive document to use as the initial template. The goal is to make the needed update to that file here: https://docs.google.com/spreadsheets/d/1CipEaf8QZk0gVzN3fzJzG5Ctu2b0-BHHgEj2iTvqGuQ/edit?usp=sharing
   1. Create the database needed, but plan for the additions in the full user stories so we don't create tech debt or a blocker.
   2. Create the API needed to manipulate the database
      1. CRUD functionality
      2. This won't be an external API, just internal for the app
      3. Create a postman collection I can use to manually manipulate the database for the books.
3. Create a test plan (unit test, integration if needed) and automation for the tests. I'd like this to work easily via Claude Code, VSCode, and Playwright if possible.

### Phase 2

The focus is on the main advancement needed to easily add items to the catalog: the mobile app portion that allows for the scanning and the backend system to add it.

1. Focus on User Story 2
   1. I want a native mobile app that allows me to scan a books barcode/ISBN with the phone camera.
   2. The app will look up the books information using a publically available source
   3. The app will add the book to the catalog via the internal API created in step one.







