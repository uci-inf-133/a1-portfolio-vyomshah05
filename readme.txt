--Readme document for Vyom Shah, vyoms2@uci.edu--

A reminder on academic integrity, as described in the syllabus.

In general, the course staff expects that you will look at code and examples from many online resources as part of the assignments, particularly to resolve syntax and understand frameworks. We expect that you'll use other libraries you find, and will even require it in some assignments. These practices are often critical to the work of developers today. The best developers are adept at interpreting the examples they see, customizing them to their specific situation, and citing their sources so they can find them later. We expect you to do the same.

While learning from examples is encouraged, attempting to pass an existing project or example from the web as your own is not allowed. If you ever have a question about what is or is not appropriate, feel free to ask the course staff!

Talking to classmates about class material, assignment requirements, etc. is a great way to verify ideas and get feedback. But this distinctly does *not* permit attempting to pass off someone else’s code as your own. Talking over ideas and approaches is allowed, but the work that you produce and submit must be your own.

1. How many assignment points do you believe you completed (replace the *'s with your numbers)?

10/10
- 1/1 Readme
- 2/2 Basic HTML content
- 1/1 Basic CSS styling
- 1/1 Advanced feature
- 2/2 Responsive layout
- 1/1 Passes validation checks
- 2/2 Embraces spirit of the assignment

2. What (a) basic features, (b) CSS features, and (c) advanced features did you include in your portfolio?

(a) Basic features

- At least one image with descriptive alt text (hero/profile image + project screenshots)
- Headings + paragraph text (About, Education, Experience)
- Links to external pages (GitHub, LinkedIn, email)
- Multiple sections/pages with navigation (navbar links to sections; if you have multiple .html pages, mention them)
- Semantic HTML tags (header, nav, main, section, footer)

(b) CSS features

- Custom spacing (padding/margins) for readability and layout
- Custom color palette (background, text, accent colors)
- Responsive layout using Flexbox/Grid + media queries (or Bootstrap grid)
- Custom fonts (Google Fonts) with fallbacks
- Button/link hover states and consistent typography scale

(c) Advanced features

- Responsive navigation bar (collapses/reflows on small screens)
- More complex layout (hero section + cards/grid projects + multi-section page)
- Projects displayed as a structured grid of “cards” (includes sliding animation with more information)
- Contact section (mailto link or form)

3. Did you ignore any of the warnings or errors presented by the accessibility checker? If so, why does this not seem like an accessibility concern? If it's useful, you can consolidate your thoughts on multiple warnings/errors if the rationale is similar.

Accessibility (AChecker):

The AChecker tool reported several manual review warnings rather than definite accessibility errors. These warnings are primarily related to automatically generated or script-driven content and do not indicate actual accessibility barriers in this portfolio.

- Text direction warnings (Checks 270, 271 – Success Criterion 1.3.1):
These warnings suggest that a dir attribute or Unicode direction markers may be required. This portfolio contains only left-to-right English text and does not include any bidirectional or right-to-left language content. Therefore, specifying an explicit text direction is unnecessary in this context.
- Script-related color, keyboard, and flashing warnings (Checks 86, 87, 89 – Success Criteria 1.4.1, 2.1.1, 2.3.1):
AChecker flagged the compiled JavaScript file as potentially using color alone, being inaccessible to keyboard users, or causing flicker. These warnings are generic and result from static analysis of the script tag rather than observed behavior. In practice, all interactive elements are standard HTML controls (links and buttons), are keyboard-accessible, do not rely on color alone to convey meaning, and do not include flashing or animated content that could trigger seizures.
- Navigation structure warnings (Checks 28, 262 – Success Criterion 2.4.1):
AChecker noted the possible absence of a “skip to content” link and unmarked link groupings. The page uses a clear semantic navigation bar and section structure, making content order and navigation understandable for screen reader and keyboard users. Given the portfolio's small size and linear structure, a skip link was deemed unnecessary and would not materially improve accessibility.
- Page title warning (Check 54 – Success Criterion 2.4.2):
The document title was flagged as potentially insufficiently descriptive. The title identifies the portfolio by name and purpose and is clear in the context of a personal portfolio website.
- Multiple ways and consistent navigation warnings (Checks 184, 276 – Success Criteria 2.4.5, 3.2.3):
These warnings suggest a missing sitemap and potential navigation inconsistency. The portfolio is a small, single-site application with a consistent navigation bar across all sections, so additional navigation mechanisms such as a sitemap are unnecessary.

Overall, no accessibility warnings were ignored that represent real barriers to users. The site was manually reviewed for readability, keyboard navigation, and clarity, and it adheres to the intent of WCAG Level A/AA guidelines for a personal portfolio.

The W3C CSS Validator reported several warnings related to vendor-specific CSS extensions, including:

- webkit-font-smoothing
- moz-osx-font-smoothing
- webkit-focus-ring-color
- webkit-backdrop-filter
- System font stack entries such as -apple-system

These are intentional, widely adopted vendor extensions used to improve font rendering, focus visibility, and visual effects across modern browsers. They do not affect compliance with standards or accessibility, and are commonly used on production websites.

The HTML was validated with the W3C HTML Validator and passed with no errors or warnings.

4. How long, in hours, did it take you to complete this assignment?

10 hours

5. What online resources did you consult when completing this assignment? (list specific URLs, describe queries to Generative AI, or use of AI-based code completion)

- Vite documentation (build output/base path concepts)
- MDN Web Docs (semantic HTML, accessibility attributes like aria-label)
- Generative AI (ChatGPT): debugging Vite file:// CORS issue and serving the site via python3 http.server.

6. What classmates or other individuals did you consult as part of this assignment? What did you discuss?

None

7. Is there anything special we need to know in order to run your code?

This submission contains a compiled static build (Vite/React output). Due to browser security restrictions, opening index.html directly via file:// may block module scripts. Please serve the site locally from the build folder, vyom-shah-portfolio/dist, where index.html is located. Oftentimes, browsers such as Chrome and Safari will not allow the Vite site to run properly, in which case you can run it on a local host by running the following commands:
`cd vyom-shah-portfolio/dist`
`python3 -m http.server 8000`
In a browser, go to: http://localhost:8000 to access the site.

I have also personally hosted this site on GitHub Pages here: vyomshah05.github.io
The code is exactly the same; I just moved it to a personal directory for the page URL.

Since I used the React framework, the HTML and CSS code are in vyom-shah-portfolio/src/components, with the HTML in the JSX files.
