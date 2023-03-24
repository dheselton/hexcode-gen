# hexcode-gen
Simple page to preview hex code colors for use to embed in Clickup tasks

HTML and JS used to generate a background color to the div when hex code is entered. we added a few lines of JavaScript to add a query string to the URL each time the changeColor() function is called, using the pushState() method of the history object. The query string includes the hex code entered by the user, encoded using the encodeURIComponent() function.

We also added some JavaScript to retrieve the saved color from the query string in the URL on page load. If a query string is present, we parse it using the URLSearchParams interface and retrieve the color parameter using the get() method. If a color parameter is found, we set the background color of the #primary-color div and prefill the color input field with the saved color.
