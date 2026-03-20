# Python Vocabulary — Lesson 3

*Conditionals*

> **How to use this:** Lesson 3 additions only. Add alongside Lessons 1 and 2 terms for a complete reference.

---

| Term | Type | Definition & Example |
|---|---|---|
| **Conditional** | *noun* | A block of code that only runs if a specific condition is true. The fundamental 'if this, then that' structure of programming. `if age >= 18:` |
| **if** | *keyword* | Starts a conditional. Python checks whether the condition is True, and runs the indented block if it is. `if password_length >= 8:` |
| **elif** | *keyword* | Short for 'else if'. Adds another condition to check if the `if` wasn't true. Must come after `if` and before `else`. `elif password_length >= 6:` |
| **else** | *keyword* | The catch-all. Runs if none of the conditions above were true. No condition attached — it covers everything remaining. `else:` |
| **Boolean check** | *noun* | The act of evaluating a condition to True or False. Every `if` statement performs a Boolean check under the hood. Also called a Boolean test. `if is_learning == True:` |
| **== (equal to)** | *operator* | Checks whether two values are equal. Double equals — not to be confused with single `=` which stores a value. `if age == 18:` |
| **!= (not equal to)** | *operator* | Checks whether two values are NOT equal. `if status != 'active':` |
| **> (greater than)** | *operator* | Checks whether the left value is greater than the right. `if score > 90:` |
| **< (less than)** | *operator* | Checks whether the left value is less than the right. `if age < 18:` |
| **>= (greater than or equal to)** | *operator* | Checks whether the left value is greater than or equal to the right. `if len(password) >= 8:` |
| **<= (less than or equal to)** | *operator* | Checks whether the left value is less than or equal to the right. `if price <= 100:` |
| **Indentation** | *noun* | The spaces at the start of a line inside a conditional (or function). Python uses indentation to know which lines belong to which block. Get it wrong and the code breaks or runs unexpectedly. |
