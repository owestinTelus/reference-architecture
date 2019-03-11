# Accessibilty standards at TELUS Digital

TELUS is committed to meeting or exceeding the [Web Content Accessibility Guidelines 2.0, level AA (WCAG 2.0 AA)](http://www.w3.org/WAI/intro/wcag). 
 
TELUS' core principle is Customers First, all customers first, regardless of their abilities, devices or screen size. We want our customers to enjoy a great digital experience. Accessibility is at the heart of how digital experiences are designed and coded.
Best practices for making accessible mobile and web apps helps us to meet this principle. These guidelines will help you get make our sites more accessible for everyone. 
 
Accessibility is a legal requirement, mandated by the [Accessibility for Ontarians with Disabilities Act (AODA)](http://www.aoda.ca/) and [Canadian Radio-Television and Telecommunications Commission (CRTC)](http://www.crtc.gc.ca/eng/home-accueil.htm)

## Accessibility guidelines

### Use plain language 
Write short sentences and use familiar words.
Avoid jargon and slang.
If you need to use an abbreviation or acronym that people may not understand, explain what it means on first reference.

### Specify your language
The language attribute helps assistive technology (AT) like screen readers decide which language or voice to use when reading pages content. html lang="en"
If the language changes on the page (e.g. a French quote), the language must be defined for that content fragment. em lang="fr"
### Structure your content 
Processing large amounts of information is a challenge for everyone. Sighted users scan a page quickly looking for headings to get an impression of the content of the page.
People that use assistive technology can navigate web pages headings, lists, and UI elements. Structuring the content correctly ensures that the experience is consistent and understandable.

#### Make sure that titles for pages or screens are unique & representative of the content. 
Titles help users orientate themselves within the website. The <title> is often the first thing users hear or see which helps them confirm that they have arrived at the correct page.

#### Ensure that the reading and focus order is logical
People who use assistive technology follow the natural flow of the page - usually from top to bottom, left to right. The logical order must be consistent and predictable.

#### Use semantic elements to indicate content structure
Use semantic elements - headings, links, lists, roles, and tables appropriately
Assistive technology (AT) relies on the native attributes from semantic HTML to navigate and use digital content.

### User Interface (UI) and assistive technology (AT)
Your user interface should be recognizable, provide clear feedback, as well as, support input from assistive technologies (AT). 

### Make sure that UI elements have visible focus
Interactive UI elements (buttons, links, menus, etc.) need to take focus and be clearly visible when swiped to or tapped on. Focus should not get lost or reset when interacting with UI elements. Examples include modal windows, alert boxes, or accordions.

#### Announce state changes and errors 
UI changes must be indicated visually and have a text-equivalent. Multisensory information ensures that people with different disabilities can perceive the change.

#### Communicate meaning with a combination of attributes
Colour alone is not sufficient to convey meaning or a state change. For example using the colour green only to indicate that a form field is valid. Example: use a green icon or checkmark to communicate the meaning.

#### Communicate the current state
It’s very common for UI elements to have two (or more states), e.g. on/off buttons. The current state should be indicated both visually and in text. Accessible Rich Internet Applications (ARIA) can be used to enhance the accessible experience. However, adding ARIA incorrectly can create new accessibility issues. Using native HTML elements supported with ARIA labels, as needed, to improve the experience.

#### Provide error messages in plain language and move focus to them
Provide error messages in plain language (don’t use jargon or error codes). Also, ensure focus is programmatically moved to the error message. Keep error message close to content so that it is easier to find, in context.

### State changes and errors
UI changes must be indicated visually and have a text-equivalent. Multisensory information ensures that people with different disabilities can perceive the change.

#### Meaning is not conveyed through colour alone
Colour alone is not sufficient to convey meaning or a state change. For example using the colour green only to indicate that a form field is valid.

#### The current state is indicated
It’s very common for UI elements to have two (or more states), e.g. on/off buttons. The current state should be indicated both visually and in text. Using native HTML elements supported with ARIA labels as needed will improve the experience.
#### Provide error messages in plain language and move focus to them
Provide error messages in plain language (don’t use jargon or error codes). Also, ensure focus is programmatically moved to the error messages. Keep error message close to content so that it is easier to find, in context.

### Accessible colours

#### Ensure sufficient colour contrast
At a minimum use the WCAG 2.0 Level AA contrast ratio of at least 4.5:1 for text on a coloured background. Use a ratio of 3:1 for large text (minimum font size 14 pt bold) and to define a change in state (for example hover/focus/selected/current/default).  
However, it’s strongly recommend aiming for a higher ratio of 7:1 given the mobile context: glossy and / or smudge screens, sun glare, lower quality screens on older phones, etc.

#### Do not use colour alone to convey meaning.
Many colours will be perceived as similar by people with colourblindness. Use colour to support other design elements to convey meaning. For example, use red with an ‘x’ to communicate an error, or green with a checkmark to communicate success.

### Tips and tools for testing accessibility 
Testing for accessibility doesn’t need to be complicated. With a few quick tests, you can determine if your web page or application meets basic accessibility standards. Learn the value of automated and manual testing. Simplify your project by setting priorities for accessibility. 

#### Automated vs Manual testing
Automated testing should always be complemented with manual testing. Testing tools can check for most standards, but manual testing is needed to validate if the content is correct or if the tool is easy to use.
For more information about testing, [review the accessibility testing standards](https://drive.google.com/a/telus.com/open?id=123rPQPtiaed0tiazglRFWDXYPNJmfwdYyq8Bx6EaNmE). 

### Accessibility for developers
Developers are responsible for following HTML5 standards to produce well structured code. Regardless of their framework. 
 
* Include automated accessibility in your unit tests (aXe browser plugin)
* Use semantic accessible code as often as possible
* Understand when to use ARIA (Accessible Rich Internet Application)
* Maintain focus management 
* Label UI (user interface) elements consistently
* Ensure that content, event, and status changes are announced to Assistive Technology (AT) 
 
As a developer you will create or implement components and content for TELUS.com.
 
Follow content structure and visual designs
* Ensure that descriptive text and labels are accurate
* Review and resolve accessibility bugs that have been identified through automated testing. 
 
For details about accessibility coding guidelines, [review TELUS Digital’s accessible coding standards](https://drive.google.com/a/telus.com/open?id=1YisZpMeDEAj49LpHe7IwJTR835G-ITx86imPm2YMPu0) 

### Accessibility for testers
Testers are responsible for ensuring that accessibility is part of the end to end (e2e) digital experience. Automated testing is primarily the responsibility of the developer. Developers run automated tools to check their code to resolve easy to spot and easy to fix issues. 
 
As a tester you should focus on the non-automated tests to validate that the automated tests are accurate.
 
* Review keyboard functionality and focus
* Validate colour treatment (colour contrast and colour blindness)
* Test with a screen reader (VoiceOver,  NVDA or JAWS) and other assistive technology such as switch control
 
For details about accessibility test, [review TELUS Digital’s accessible testing standards](https://drive.google.com/a/telus.com/open?id=123rPQPtiaed0tiazglRFWDXYPNJmfwdYyq8Bx6EaNmE) 
