# CS455 [ Aakash Yadav (210010) ]
- Deployed Game: [Play](https://harshitptl21.github.io/CS455/)

## Assignment 1: Develop a Game
A puzzle game, in which an image is split into 9 parts and the user has to assemble it to form the original image.
- [Problem Statement](https://github.com/harshitptl21/CS455/blob/main/Problem_Statements/Assignment_1.pdf)
- Task/Planning (Details and task assignment is in the [Issues (label:Assignment 1)](https://github.com/harshitptl21/CS455/issues?q=is%3Aissue+label%3A%22Assignment+1%22)
  - Add HTML and CSS file
  - Add game functionalities

## Assignment 2: Code Quality
- [Problem Statement](https://github.com/harshitptl21/CS455/blob/main/Problem_Statements/Assignment_2.pdf)
- Task/Planning (Details and task assignment is in the [Issues (label:Assignment 2)](https://github.com/harshitptl21/CS455/issues?q=is%3Aissue+label%3A%22Assignment+2%22)
  - Add Code Quality Metrics
    - ESLint : Lints and enforces coding standards for JavaScript
    - eslint-plugin-complexity: Checks code complexity
    - Stylelint: Lints and enforces coding standards for HTML
    - JSCPD: Detects code duplicatio across the Game codebase
  - Refactor Code
  - Add Unit Tests
  - Continuous Integration
-Running Locally
 -Install depedencies:
  - npm install
 - Run Code Quality Checkers
    - For JavaScripts and Code Complexity: npm run lint:js
    - For CSS: npm run lint:css
    - For HTML: npm run lint:html
    - For Duplication: npm run check:duplication
  - Unit Test
    - Run: npm run test
    - Report

## Assignment 3 : Conversion to client-server architecture  
- Problem Statement
- Task/Planing(Detais and task assignment is in the [Issue (label: Assignment 3)]
- Report
- Architecture & test pyramid diagram 
- Client-Server Architecture diagram:
- Game Logic Diagram
- Testing Pyramid diagram:
- Components:
 - UI (HTML & CSS):
    - index.html : Sets up the main structure of the game including the timer, score tables, canvas and input fields for
      for the username.
    - style.css: Styles the game, including blurrd elements until a username is entered, and the layout for the canvas, score table, and other UI elements.
 - Game Logic:
    - script.js: Core logic of the puzzle game, including setting up the puzzle, handling events (drag, drop, timer), and shuffling pieces.
 - Backend:
    - get_scores.php: Retrieve scores from the database and sends them to the frontend for display in the score tables.
    - submit_score.php: Submits the user's score and username to the database once the game ends.

- Workflows:
   - User Interactions:
      - User enters their name in the input field.
      - The game starts when the user clicks or touches the canvas.
      - The game logic starts, shuffling the puzzle and initiating the timer.
      - The player moves pieces using mouse or touch events.
    - Game State:
      - Canvas: Displays the puzzle pieces and updates their positions as the user drags and drops them.
      - Timer: Counts down and triggers the game over if time runs out.
    - Database Interactions:
       - Submit Scores: After the game ends, the submit_score.php sends the user's score to the backend and stores it in puzzle_game.db
       - Fetch Scores: On page load, get_scores.php fetches the scores from the database to display in the score tables.

- Testing:
   - karma (jasmine): For Javascript testing
   - phpunit: For php testing
   - Unit test: Tested game logic.
   - Integration test: Tested frontend-server and server-database integration
   - End to End test: Manually tested UI
- Deplyoed Game (client-server architecture) : Play


## Assignment 4 : Performacne Testing and Reliabilty Enhancements 

- Problem Statement
- Task/Planning (Details and task assignment is in the Issues (label:Assignment 4)
- Load Balancer: LB Server
- Primary Server: PS1 PS2
- Backup Server: BS
- Part 1 : Performance Testing
   - Client side (selenium) : Reports test
   - Server-side (k6) : Reports
   - Automate Performance Testing: workflow
- Part 2 : Reliability and Failover Mechanisms
   - Load Balancing: php script
   - Automatic Failover: php script
   

