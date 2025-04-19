# KitchenChaos
A Hectic Culinary Coordination Game Inspired by Overcooked

**Project Name:** Kitchen Chaos

**Sub Heading:** A Hectic Culinary Coordination Game Inspired by Overcooked

**Tech Stack:**

- **Engine:** Unity
- **Language:** C# (Standard for Unity development)
- **Key Systems:** Unity Physics (for movement/interaction), Unity Input System, Unity UI (for displaying orders, timers, etc.)

**Project Overview:**

- **Idea & USP:** To recreate the engaging, fast-paced, and often chaotic cooking and order fulfillment gameplay loop popularized by the game "Overcooked" within the Unity engine. The focus was on faithfully implementing the core mechanics of ingredient preparation, cooking, plating, and serving under time pressure.
- **Summary:** Kitchen Chaos is a single-player game where the player controls a chef within various kitchen environments. Orders for specific recipes appear, requiring the player to efficiently gather raw ingredients, transport them to appropriate processing stations (like cutting boards or stoves), perform the required actions (chopping, cooking), combine ingredients correctly onto plates, and serve the finished dishes before time runs out. The gameplay emphasizes task management, spatial awareness, and optimizing workflow within the kitchen layout.
- **Result/Status:** A functional game prototype developed in Unity, successfully implementing the core gameplay mechanics central to "Overcooked," including ingredient handling, processing station interactions, recipe fulfillment, and time-based challenges. Multiplayer features, though potentially planned, were not implemented.

**Key Features:**

- **Ingredient Handling:** Picking up, carrying, and placing various raw food ingredients.
- **Workstation Interaction:** Using specific kitchen stations for processing ingredients (e.g., chopping blocks for cutting vegetables, stoves/pans for cooking).
- **Recipe Fulfillment:** Combining specific processed ingredients onto plates according to presented orders.
- **Order Management & Serving:** Receiving timed orders and delivering completed dishes to a serving counter.
- **Time-Based Challenge:** Core gameplay loop driven by time limits for completing orders, creating pressure and requiring efficiency.
- **Single-Player Task Management:** Requires the player to efficiently juggle multiple tasks and manage sequences of actions alone.

**Challenges and Solutions:**

- **Challenge 1:** Implementing a flexible and robust system for tracking the state of ingredients (raw, chopped, cooked, burnt, plated) and managing interactions between ingredients, players, stations, and plates.
    - **Solution:** Developed state machines or used enums within ingredient scripts to track their current status. Implemented interaction logic using trigger colliders or raycasting, checking compatibility between held items and target stations/plates before allowing an action (e.g., only allowing raw vegetables on a cutting board, only allowing cooked ingredients on a plate). Defined recipes possibly using Scriptable Objects or data structures.
- **Challenge 2:** Creating intuitive and responsive controls for picking up, placing, and interacting with numerous objects in a potentially cluttered kitchen environment.
    - **Solution:** Implemented a detection system (likely raycast or overlap sphere from the player) to identify nearby interactable objects. Provided clear visual feedback for interactable items. Designed the interaction logic to prioritize the object the player is facing or closest to, handling pickup/drop actions cleanly.
- **Challenge 3:** Replicating the specific timing and feel of cooking processes and other actions from the inspiration game ("Overcooked").
    - **Solution:** Used timers and coroutines within Unity scripts to manage the duration of processes like chopping and cooking. Implemented visual feedback (e.g., progress bars, color changes) to indicate process completion or potential issues (like burning food). Tuned action timings through iteration to match the desired fast-paced feel.

**Timeline:**

- Estimated development duration: Approximately 4-8 weeks (for a solo developer focused on implementing the core Overcooked-style mechanics and basic level interactions).

**What I Learned:**

- **Complex State Management:** Designing and implementing systems to track multiple interacting states for game objects (ingredients, stations).
- **Item Interaction Systems:** Building robust systems for player interaction with world objects (picking up, dropping, using stations).
- **Implementing Time-Based Mechanics:** Creating timers, progress indicators, and score systems driven by time constraints.
- **Structuring Gameplay Loops:** Designing the flow of core game actions (fetch, process, combine, deliver) within a level.
- **Unity Engine Proficiency:** Practical application of Unity's physics, input handling, UI elements (for feedback), and C# scripting for complex game logic.
- **Single-Player Task Simulation:** Programming logic that requires the player to manage multiple concurrent or sequential tasks efficiently.
- **Analyzing and Replicating Mechanics:** Breaking down and recreating gameplay systems from an existing, successful game ("Overcooked").

---
