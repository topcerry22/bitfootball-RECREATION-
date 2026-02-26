================================================================================
  BIT FOOTBALL  —  PROGRAM · BUILD · DOMINATE
================================================================================

  A browser-based football strategy game where you program your robots with
  chip sequences, build formations, and battle an AI opponent in real-time
  physics matches. No controllers. No reflexes. Pure tactics.

  Just open bitfootball.html in any modern browser. No install required.

--------------------------------------------------------------------------------
  GETTING STARTED
--------------------------------------------------------------------------------

  1. Open bitfootball.html in Chrome, Firefox, or Edge
  2. Create an account (username + password + team name)
  3. Build your first robot in the Robots screen
  4. Program it with chips in the Program screen
  5. Place it on the field in the Formation screen
  6. Kick off in the Match screen

  Your account saves automatically to your browser's local storage.
  It will still be there next time you open the file.

--------------------------------------------------------------------------------
  THE CORE LOOP
--------------------------------------------------------------------------------

  You don't control your players during a match. Instead, you program them
  BEFORE the game starts. Your robots read their chip sequences like a script
  and execute them in order, looping back to the start when they finish.

  The smarter your program, the better your team plays.

  BUILD ROBOT → PROGRAM CHIPS → SET FORMATION → PLAY MATCH → EARN RP → REPEAT

--------------------------------------------------------------------------------
  ROBOTS
--------------------------------------------------------------------------------

  Each robot has three stats (1–10):

    SPD  Speed    — How fast the robot moves around the pitch
    STR  Strength — How hard it kicks the ball
    INT  Intelligence — How accurately it aims shots and passes

  You can have multiple robots on your team. Each robot gets its own
  independent chip program. Click a robot's emoji to change its icon.
  Robots can be recolored, renamed, and have their stats adjusted at any time.

--------------------------------------------------------------------------------
  CHIPS  —  The Programming System
--------------------------------------------------------------------------------

  Chips are the instructions your robots execute. Drag them from the palette
  into a robot's program sequence. They loop continuously during the match.

  SIX CHIP CATEGORIES:

    🟢 MOVE     Positional and passing chips
                Sprint, Counter Attack, Through Ball, Go to Ball, Wide Run...

    🟠 ATTACK   Shooting and dribbling chips
                Power Shot, Dribble, Spin Dribble, Precision Shot, Volley...
                + 🎯 Shoot at Goal  (fires an immediate aimed shot on contact)
                + 🏃 Go to Enemy Goal  (sprints into the opponent's box)

    🔵 DEFEND   Defensive and clearing chips
                Tackle, High Press, Park the Bus, Interception, Go to Goal...

    🟣 SPECIAL  High-risk high-reward chips
                Turbo Burst, Berserk, Super Shot, Dragon Shot, Golden Touch...

    🩵 SUPPORT  Team tactics chips
                Team Press, Long Ball, False Nine, Possession Hold...

    🩷 TRICK    Unpredictable chaos chips
                Nutmeg Dance, Maradona, Rainbow Flick, Wild Card...

  Each chip has three stat modifiers:
    POW  Kick power multiplier
    SPD  Movement speed bonus
    DEF  Defensive effectiveness

  TIP: Mix categories. An all-attack robot gets outpressed. Balance wins.

--------------------------------------------------------------------------------
  IF / ELSE BLOCKS
--------------------------------------------------------------------------------

  Click "+ IF / ELSE block" in the Program editor to add conditional logic.
  The robot evaluates the condition and runs the THEN or ELSE branch.

  Available conditions:

    score is winning          score is losing           score is a draw
    team has possession       team lost possession
    first half of match       second half of match
    score within 1 goal
    robot speed > 7           robot strength > 7        robot intelligence > 7
    ball is in opponent's half                          ball is in our half
    ball is near enemy goal   teammate is nearby
    a teammate has the ball   enemy is nearby
    50% chance  (random)

  EXAMPLE PROGRAM:
    IF score is losing
      THEN: 🎯 Shoot at Goal → ⚡ Counter Attack
      ELSE: 🤲 Short Pass → 🏃 Sprint
    💥 Power Shot

--------------------------------------------------------------------------------
  FORMATION
--------------------------------------------------------------------------------

  Drag your robots from the sidebar onto your team's half (right side) of the
  pitch. Their position determines their AI role during the match:

    Deepest 20%   →  Goalkeeper
    Deep 20–40%   →  Defender
    Middle 40–68% →  Midfielder
    Forward 68%+  →  Attacker/Forward

  Position matters. A robot placed deep will hold its line and clear danger.
  A robot placed high will press, carry, and shoot.

  Click a placed robot to remove it from the field.

--------------------------------------------------------------------------------
  MATCH
--------------------------------------------------------------------------------

  Select a stadium, weather, and opponent difficulty, then kick off.

  STADIUMS:
    Classic     Standard pitch
    Night       Floodlit atmosphere
    Storm       Slippery rain physics (ball moves faster, kicks less accurate)
    Micro       Smaller arena — chaotic close-quarters
    Mega        Bigger arena — more space, longer runs
    Night Storm Dark + rain combined

  DIFFICULTY:
    🟢 Easy    AI reacts slowly, aims poorly, presses from short range
    🟡 Medium  AI predicts ball movement, moderate pressing
    🔴 Hard    Full boss AI — predictive interception, aggressive pressing,
               dedicated sweeper, harder kicks, tight dribbling, long ball
               counter-attacks, near-perfect aim

  MATCH SPEED:
    Use the speed control to run the match at 1× or 3× (fast-forward).

  The match ends after the time limit. Goals are shown in the log panel.
  The possession bar at the bottom shows real-time ball control.

--------------------------------------------------------------------------------
  RED TEAM AI  (what you're up against)
--------------------------------------------------------------------------------

  The opposing Red Team uses a differentiated boss AI. On Hard difficulty:

    PREDICTIVE INTERCEPTION
      Red players aim at where the ball WILL BE (velocity × 12 ticks ahead),
      not where it currently is. They cut off your passes before they arrive.

    SWEEPER
      The deepest Red defender never presses. They permanently track the
      goal-to-ball line, always standing between the ball and their goal.

    AGGRESSIVE PRESSING
      Red's press radius is 40% wider than Blue's. They swarm faster.

    HARDER KICKS
      Red kicks at 1.22× base power. Their shots are noticeably harder.

    TIGHT DRIBBLING
      Red's ball control is significantly tighter. Harder to dispossess.

    LONG BALL COUNTER-ATTACK
      When a Red defender wins the ball in their own half, they immediately
      launch a long ball to their most advanced forward. Fast transitions.

    FASTER REACTION
      Red reacts 1 tick faster than Blue every decision cycle.

--------------------------------------------------------------------------------
  RANKED & LEAGUES
--------------------------------------------------------------------------------

  Every match result affects your Ranked Points (RP):

    Win   +RP    Loss  -RP    Draw  ±0

  RANK TIERS:
    🪵 Wood       0–200 RP
    🥉 Bronze     200–500 RP
    🥈 Silver     500–900 RP
    🥇 Gold       900–1400 RP
    💠 Platinum   1400–2000 RP
    💎 Diamond    2000–3000 RP
    ⚡ Legend     3000+ RP

  LEAGUES:
    Join a league of up to 8 players. Play matches to earn points.
    League table shows W/D/L, goals for/against, and total points.

--------------------------------------------------------------------------------
  CLANS
--------------------------------------------------------------------------------

  Create or join a clan to represent your team tag in matches.
  Clans have a name, 3-letter tag, color, and icon.

--------------------------------------------------------------------------------
  YOUR ACCOUNT
--------------------------------------------------------------------------------

  Click your username (top-right ⚙) to open your profile:
    - Change your avatar emoji
    - Edit your team name
    - Change your password
    - View your W/D/L record and rank

  Sign out from the profile modal. Your data persists in your browser.
  Accounts are stored locally — they do not sync across devices.

--------------------------------------------------------------------------------
  TIPS & STRATEGIES
--------------------------------------------------------------------------------

  ● The IF "score is losing" condition is your most powerful tool.
    Build aggressive programs that only activate when you need a goal.

  ● Pair "ball is near enemy goal" with 🎯 Shoot at Goal for a robot
    that dribbles patiently then fires when in range.

  ● High STR robots make great defenders — their clearances go further.

  ● High INT robots are your best shooters — they aim for the corners.

  ● High SPD robots work best as forwards or counter-attack runners.

  ● The 🏃 Go to Enemy Goal chip + 🎯 Shoot at Goal is the most
    direct attacking combo. Put it on your fastest attacker.

  ● Against Hard AI: place a defender with 🥅 Go to Goal chip deep in
    your half. They'll guard your goal mouth permanently.

  ● Don't stack all your robots in one position. Spread them so the
    AI's sweeper can't intercept all your runs at once.

  ● On a Storm pitch, reduce kick power chips and use more movement
    chips — the slippery ball travels faster on its own.

--------------------------------------------------------------------------------
  KEYBOARD / CONTROLS
--------------------------------------------------------------------------------

  This game has no keyboard controls during matches.
  Everything is configured before the match through the editor.
  Use mouse/touch to navigate menus, drag chips, and place robots.

--------------------------------------------------------------------------------
  TECHNICAL NOTES
--------------------------------------------------------------------------------

  Built as a single self-contained HTML file.
  No server required. No internet required after download.
  All game state saved to localStorage (key: bf5_acc).
  Physics engine runs at 60fps in normalized 0–1 coordinate space.
  Tested in Chrome 120+, Firefox 121+, Edge 120+.

================================================================================
  BIT FOOTBALL  v1.0  —  Open bitfootball.html to play
================================================================================
