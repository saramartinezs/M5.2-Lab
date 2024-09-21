# Lab 5 - Accessibility

## Overview

For this lab, we were given a web page with many accessibility issues that needed to 
be fixed. The goal was to identify and fix as many as possible. 

### To view the web page: 
1. Clone the repository to your local machine.
2. Open the repository in VSCode. 
3. Use the Live Preview extension available in VSCode to view the webpage. The page can be viewed in a preview window within VSCode or in a web browser using the link found in the preview window. 


## Sources and Credits

- This week's reading: https://developer.mozilla.org/en-US/docs/Learn/Accessibility/What_is_accessibility
- Contrast Checker: https://webaim.org/resources/contrastchecker/

## Accessibility Lab Answers 

### Color
The color contrast between the green background and the black text failed the Web AIM Contrast Checker. The background color had to be changed to one that could properly display the dark text. I chose to use white. 

### Semantic HTML
The "Show Comments" button is not selected when using keyboard navigation. The article text needed a lot of small changes. I added proper h1, h2, h3, and p elements throughout the article. In order to make the navigation menu more accessible, it should be updated with a <nav> element. This easy fix provides much more accessibility. 

### Images 
To provide better accessibility for the images, I provided an alt attribute to provide description of the image. 

### The Audio Player
For the first audio clip, I added a transcript for the audio as another option. 

For the other audio clip, I added a link to it, since the browser doesn't support the audio file. 

### The Forms 
I added an aria-label attribute to the input element that would not be visible to sighted users, but it would still be read by screen readers. 

For the two input elements in the comment form, I placed "Your name" and "Your comment" into a label element with the corresponding "for=" attribute. 

### The Show/Hide Comment Control
In order to have the show/hide comment control button be accessible, I changed it into being a button element, rather than a div. Now, it can be accessed with the tab key and activated using the enter key. 

### The Table 
I added "scope=col" and "scope=row" for the columns and rows of the table. I also added a summary attribute. 

### Other Considerations
Something else that can improve the accessibility is changing the color of a link when it is hovered over. I modified the nav links to change in this way. I also changed the "Related" section's links to remove the underlining when it is hovered over. 

Another addition that could be made is having your own custom audio/video controls. In this week's reading, it mentioned that in many browsers, the controls can't be accessed by a keyboard. Having your own could help mitigate this issue. 