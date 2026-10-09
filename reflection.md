# 💭 Reflection: Game Glitch Investigator

Answer each question in 3 to 5 sentences. Be specific and honest about what actually happened while you worked. This is about your process, not trying to sound perfect.

## 1. What was broken when you started?

- What did the game look like the first time you ran it?
- List at least two concrete bugs you noticed at the start  
  (for example: "the hints were backwards").

**Bug Reproduction Log**

Document at least 3 bugs you found. Add rows as needed.

| Input | Expected Behavior | Actual Behavior | Console Output / Error |
|-------|-------------------|-----------------|------------------------|
|Attempts|Attempts should 8|Attempts showed 7|Console Ouput: none/|
|Higher-Lower|"Too High" = GO LOWER, "Too Low" = GO HIGHER|"Too High" = GO HIGHER, "Too Low" = GO LOWER|Console Output: Guess = 3, Secret = 5, GO LOWER|
|New Game|Starts New Game|Game never reset|Console Output: none/|

---

## 2. How did you use AI as a teammate?

- Which AI tools did you use on this project (for example: ChatGPT, Gemini, Copilot)?
- Give one example of an AI suggestion that was correct (including what the AI suggested and how you verified the result).
- Give one example of an AI suggestion you did not accept as written (including what the AI suggested, why you rejected or changed it, and how you verified your version). It does not have to be a suggestion that was wrong: over-engineered, out of scope, harder to read, or a poor fit for this codebase all count.

  Answer: I used AI as a teammate to help solve fixed bug problem 2. I had no idea what to do so I asked Claude Code what was the problem and not write anything and see if it was truly correct. I didn't accept the second swap at lines 45-47 as it wasn't needed when testing out the codes and lines 36-40 were corrected to the right standard of how the code needed to operate as. 

## 3. Debugging and testing your fixes

- How did you decide whether a bug was really fixed?
- Describe at least one test you ran (manual or using pytest)  
  and what it showed you about your code.
- Did AI help you design or understand any tests? How?

 Answer: I was able to decide if it was really fixed was by testing the issue by myself using the app's streamlit service that I was able to function each of my problems seperately. All my debugs and fixes were my doing as testing in my opinion needs to be based within human strength with the following code.  

## 4. What did you learn about Streamlit and state?

- How would you explain Streamlit "reruns" and session state to a friend who has never used Streamlit?

 Answer: With streamlit's reruns and session states, I would describe it as a save-state within a video game. In video games for example when you hit a checkpoint, it creates a save-state for you so you don't go back to the last section. With the coding, when you save, the streamlit will update all your code within the stream and fix the issue by just reloading the page. 

## 5. Looking ahead: your developer habits

- What is one habit or strategy from this project that you want to reuse in future labs or projects?
  - This could be a testing habit, a prompting strategy, or a way you used Git.
- What is one thing you would do differently next time you work with AI on a coding task?
- In one or two sentences, describe how this project changed the way you think about AI generated code.

 Answer: The habit I will use after this project is to stay focuse on yourself, not others. Stay true to yourself and fix issues that you need to do. Sometimes help is great, but to becoming a great programmer, you have to be yourself to flourishing in editing, revising, and creating code. 



The AI's Commit Message: 

Fix hint direction, attempt counter, and new game state; complete reflection

app.py:
- Fix swapped hint messages in check_guess: "Too High" now says
  "Go LOWER!" and "Too Low" now says "Go HIGHER!"
- Start the attempts counter at 0 instead of 1 so the attempt count
  is correct
- Change the new game handling so the game status resets to "playing"

reflection.md:
- Document three bugs found (attempts count, higher/lower hints,
  new game not resetting)
- Answer the reflection questions on AI collaboration, testing,
  Streamlit reruns/session state, and future habits
