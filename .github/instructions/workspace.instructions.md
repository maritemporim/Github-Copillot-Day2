---
description: Workspace instructions for the Soc Ops Spring Boot Java project and local development workflow.
---

# Soc Ops Workspace Instructions

## What this repo is
A Spring Boot social bingo game that runs locally from `socops/` with a Thymeleaf UI and no frontend build step.

## Mandatory development checklist
- [ ] Verify Java 21 is installed: `java -version`
- [ ] Run lint or format checks if configured
- [ ] Build the project: `cd socops && ./mvnw clean package`
- [ ] Run tests: `cd socops && ./mvnw test`
- [ ] Start the app: `cd socops && ./mvnw spring-boot:run`
- [ ] Confirm the app responds at `http://127.0.0.1:8080`

## Quick start
1. `cd socops`
2. `./mvnw spring-boot:run`
3. Open `http://127.0.0.1:8080`

## Key files
- `socops/pom.xml`
- `socops/src/main/java/com/socops/SocOpsApplication.java`
- `socops/src/main/java/com/socops/web/BingoRestController.java`
- `socops/src/main/resources/templates/game.html`
- `socops/src/main/resources/static/css/app.css`

## Notes
- The app serves HTML and CSS directly; there is no npm or frontend bundler.
- `BoardAssembler` contains the game board logic and is easy to test in isolation.
- See `.github/instructions/css-utilities.instructions.md` and `.github/instructions/frontend-design.instructions.md` for styling and design guidance.
