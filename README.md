# CSS Cascade Activity

## Solutions

1. **For `<p id="mission">`**
   - **Rules that apply to `color`:**
     - `p { color: black; }`
     - `.text { color: #555; }`
     - `#mission { color: darkorange; }`
   - **Final color:** darkorange
   - **Explanation:** the `#mission` ID selector has higher specificity, so darkorange is used.

2. **For `<p id="team">`**
   - **Rules that apply to `color`:**
     - Inline style: `style="color: darkblue;"`
     - `p { color: black; }`
     - `.text { color: #555; }`
   - **Final color:** darkblue
   - **Explanation:** the inline style has the highest priority.

3. **For `<p id="experience">`**
   - **Rules that apply to `color`:**
     - `p { color: black; }`
     - `#experience { color: darkgray; }`
     - `.text { color: #555; }`
     - `#about p:last-child { color: green; }`
   - **Final color:** green
   - **Explanation:** the `#about p:last-child` selector has the highest specificity.

4. **For `<p id="services-intro">`**
   - **Rules that apply to `color`:**
     - `p { color: black; }`
     - `.intro { color: blue; }`
     - `.text { color: #555; }`
   - **Final color:** blue
   - **Explanation:** the .intro and .class selectors have the same specificity, so the order in which they appear in the CSS determines which one applies.

5. **For `<p id="offer">`**
   - **Rules that apply to `color`:**
     - Inline style: `style="color: darkblue"`
     - `p { color: black; }`
     - `.text { color: #555; }`
     - `#offer { color: darkgreen !important; }`
   - **Final color:** darkgreen
   - **Explanation:** The `!important` in `#offer` overrides all other color rules, so darkgreen is applied.

