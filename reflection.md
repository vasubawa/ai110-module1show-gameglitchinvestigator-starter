# 💭 Reflection: Game Glitch Investigator

Answer each question in 3 to 5 sentences. Be specific and honest about what actually happened while you worked. This is about your process, not trying to sound perfect.

## 1. What was broken when you started?

- What did the game look like the first time you ran it?
- List at least two concrete bugs you noticed at the start  
  (for example: "the hints were backwards").

- Tell's me to go lower when the number range is between 1 and 100 even if I entered 1. So I entered 1 for example and hint would still say to go lower. 
- New game button doesn't seem to work. I entered a correct number, and it just would not start a new game. 
- Hard difficulty was more like medium. Hard was 1:50 vs Medium which was 1:100
---

## 2. How did you use AI as a teammate?

- Which AI tools did you use on this project (for example: ChatGPT, Gemini, Copilot)?
- Give one example of an AI suggestion that was correct (including what the AI suggested and how you verified the result).
- Give one example of an AI suggestion that was incorrect or misleading (including what the AI suggested and how you verified the result).

- Github Copilot
- One of the correct AI suggestion was for the new game button and the difficult range being wrong.
- One incorrect one from the AI I found was input validation. It suggested that the program wasn't verifying if a number was entered or not. I inputted an letter and it was clearly confirming that I did not enter a number. 

 
---

## 3. Debugging and testing your fixes

- How did you decide whether a bug was really fixed?
- Describe at least one test you ran (manual or using pytest)  
  and what it showed you about your code.
- Did AI help you design or understand any tests? How?

- I decided a bug was fixed when pytest passed and manual playthroughs consistently showed the expected behavior.
- I ran unit tests for `check_guess()` (50=Win, 60=Too High, 40=Too Low) which passed after the fix, and I verified UI messages manually.
- Copilot suggested comparison patterns and quick refactors, but I validated every suggestion with tests and manual checks.

## 4. What did you learn about Streamlit and state?

- How would you explain Streamlit "reruns" and session state to a friend who has never used Streamlit?

 - Streamlit reruns the whole app every time you click or type, so values reset unless the app explicitly saves them; in this project we save the secret number, attempts, and score so they persist between interactions.

---

## 5. Looking ahead: your developer habits

- What is one habit or strategy from this project that you want to reuse in future labs or projects?
  - This could be a testing habit, a prompting strategy, or a way you used Git.
- What is one thing you would do differently next time you work with AI on a coding task?
- In one or two sentences, describe how this project changed the way you think about AI generated code.

 - I'll keep writing small unit tests and running them early to catch regressions, and commit small, verifiable changes frequently.
 - Next time I'll prompt AI with stricter constraints and always validate suggestions with tests before applying them.
 - This project taught me to treat AI code as a helpful draft: it speeds up work but requires human verification and testing.
Step 1: Finalize your README

    Open README.md.
    Update the "Demo" section.
    Fill in the "Document Your Experience" section.
    If you completed Challenge 1: Advanced Edge-Case Testing, include a screenshot of your pytest results in the README showing the tests passing.

💡 Tip: You can take a screenshot using your computer's built-in snipping tool or screen capture shortcut.

Step 2: Write Your Reflection

    Open reflection.md.

    Complete the final reflection questions in the file.
    Be honest! If the AI gave you a bad suggestion that you had to reject, explain why. This shows you were in control of the process, not just following the AI blindly.

Step 4: Final Commit and Push

    Use Copilot's Generate Commit Message feature to summarize your final documentation updates.
    Send your completed project to GitHub: 