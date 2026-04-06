# The Seven Stages of Action

When we interact with a website or an application, we often do so with a specific purpose in mind, such as purchasing a pair of shoes, checking the weather, or sending an email. While these actions might seem instantaneous or instinctual, they involve a complex cognitive process. Don Norman, a pioneer in the field of cognitive science and usability engineering, decomposed this process into what he calls "The Seven Stages of Action." Understanding these stages allows designers to pinpoint exactly where a user might encounter friction and how to smooth the path between a user's intention and their desired outcome.

At the heart of this framework are two major psychological gaps that a user must cross: the Gulf of Execution and the Gulf of Evaluation. The Gulf of Execution represents the distance between a user's goal and the physical actions required to achieve it. The Gulf of Evaluation represents the distance between the system's response and the user’s understanding of whether their goal was met. As web developers and designers, our primary mission is to build bridges across these two gulfs.

## The Gulf of Execution

The Gulf of Execution asks the question: "How do I do it?" It covers the first four stages of the action cycle. When a user looks at a web interface, they need to figure out which buttons to click, which menus to open, and what information to type. If the interface is confusing—perhaps because a button doesn't look clickable or a navigation menu is hidden—the Gulf of Execution becomes a wide chasm, leading to user frustration.

To bridge this gulf, designers rely on affordances and signifiers. For example, a blue, underlined piece of text "affords" clicking because it follows the established signifier for a hyperlink. By making the "how" obvious, we reduce the cognitive load required for the user to move from a thought to an action.

## The Gulf of Evaluation

The Gulf of Evaluation asks the question: "What happened?" This covers the final three stages of the cycle. Once a user performs an action—such as clicking "Submit" on a form—they look for a response. If the page simply reloads without a success message, or if a loading spinner appears indefinitely, the user is left wondering if their action was successful.

Bridging this gulf requires immediate and clear feedback. In web design, this might look like a green "Success" banner, a confirmation email, or a simple change in button color to indicate a state change. Without these signals, the user cannot easily interpret the system's state, leading to repeated clicks or abandonment of the task.

## The Cycle of Action

To better understand how these gulfs manifest, we can break the user's journey into seven distinct stages. While we often think of these as a linear sequence, users frequently jump back and forth between them as they learn a new interface.

### Forming the Goal
The process begins with a high-level objective. This is often abstract, such as "I want to find a new laptop." At this stage, the user isn't thinking about buttons or pixels; they are focused on their own needs.

### Planning the Action
The user translates their goal into a specific plan. They might think, "I will go to an electronics retailer’s website and use the search bar." This is where the user's mental model of how the web works comes into play.

### Specifying the Action Sequence
The plan is further refined into physical movements. The user decides to move their cursor to the search input field, type "MacBook Pro," and press the "Enter" key.

### Performing the Action
The user executes the sequence. They physically interact with the hardware (mouse, keyboard, or touchscreen) to manipulate the interface. This is the final step in the Gulf of Execution.

### Perceiving the State of the World
Once the action is performed, the user looks for a change. They see the screen flicker, a new page load, or a list of search results appear. This is the first step in the Gulf of Evaluation.

### Interpreting the Perception
The user tries to make sense of what they see. They look at the search results and determine if the items listed are indeed laptops or just accessories. They process the visual information provided by the UI.

### Comparing the Outcome with the Goal
Finally, the user asks, "Is this what I wanted?" If the search results show the laptop they were looking for, the goal is satisfied. If the results are empty, the user restarts the cycle with a new plan.

## Practical Application in Web Interfaces

Consider the common task of adding an item to an online shopping cart. If a developer places the "Add to Cart" button in an unconventional location or uses a vague icon, the user struggles at the **Specify** stage. They know what they want to do, but the interface doesn't tell them how.

Once the button is clicked, if the website doesn't provide a visual confirmation (like a sliding side-cart or a badge count update), the user fails at the **Interpret** stage. They might click the button five more times, unintentionally adding five items to their cart. This is a classic failure to bridge the Gulf of Evaluation. 

To prevent these issues, web designers should:
*   Use standard UI patterns to help users **Plan** and **Specify** actions quickly.
*   Ensure interactive elements are visually distinct to aid in **Performing** the action.
*   Provide "Active States" (like button hover or press effects) to help the user **Perceive** the interaction.
*   Display clear success or error messages to help the user **Interpret** and **Compare** the results.

## Common Challenges and Solutions

One of the most frequent challenges in modern web design is "Invisible State." This occurs when a system changes its internal state (e.g., saving a draft) without notifying the user. From the user's perspective, nothing has happened, leaving them stuck in the Gulf of Evaluation. The solution is to always provide a "system status" update. A small "Draft Saved" toast notification bridges this gap perfectly.

Another challenge is "Mode Errors," where an action has different meanings depending on the current state of the interface. If a user tries to type in a search bar but the focus is actually on a keyboard shortcut layer, the **Perform** stage leads to an unexpected outcome. Designers can solve this by providing clear visual cues about which "mode" or "focus" the interface is currently in.

## Summary

Don Norman’s Seven Stages of Action provide a framework for understanding the dialogue between a human and a machine. By viewing web design through the lens of the Gulf of Execution and the Gulf of Evaluation, we can move beyond mere aesthetics and focus on how well our interfaces support human cognition. 

Bridging the Gulf of Execution requires making the possible actions visible and intuitive. Bridging the Gulf of Evaluation requires making the results of those actions immediate and understandable. When both gulfs are bridged, the technology becomes "invisible," allowing the user to focus entirely on their goal rather than the tool they are using to achieve it.

***

**Suggested Engagement:**
Observe your own behavior the next time you use a new mobile app. At which stage do you feel the most hesitation? Is it because you don't know where to click (Execution), or because you aren't sure if your click worked (Evaluation)? Mapping your own frustrations to these seven stages is the first step toward becoming a more empathetic designer.

**Further Reading:**
*   *The Design of Everyday Things* by Don Norman.
*   "The Seven Stages of Action" on the Nielsen Norman Group (NN/g) website for deep dives into usability heuristics.