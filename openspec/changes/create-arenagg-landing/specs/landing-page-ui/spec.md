## ADDED Requirements

### Requirement: Responsive Navigation
The system MUST provide a navigation bar containing links: ARENAGG, MAIN, TOURNAMENTS, RANKING, LOGIN.

#### Scenario: User views navbar on desktop
- **WHEN** the user views the landing page on a screen wider than 768px
- **THEN** the navigation links are displayed horizontally

#### Scenario: User views navbar on mobile
- **WHEN** the user views the landing page on a screen smaller than 768px
- **THEN** the navigation links adapt to remain accessible (e.g. via hamburger menu or scrollable list)

### Requirement: Hero Section with CTA
The landing page MUST display a prominent "Hero" section with a visible Call to Action button.

#### Scenario: User sees CTA
- **WHEN** the user lands on the page
- **THEN** they see an esports-themed background image and a "PARTICIPATE NOW" button

### Requirement: Global Statistics
The page MUST show the global statistics of the platform.

#### Scenario: User views statistics
- **WHEN** the user scrolls below the hero section
- **THEN** they see "TOURNAMENTS HELD: 1213" and "REGISTERED PLAYERS: 7098"

### Requirement: Footer Links
The page MUST include a footer.

#### Scenario: User views footer
- **WHEN** the user reaches the bottom of the page
- **THEN** they see "Politics", "2025 - ArenaGG", and "AboutUs"
