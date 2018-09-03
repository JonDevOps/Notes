// Alt attributes are mandatory on every img element
// Only use 1 <h1> element per page
// Don't skip heading subsections. Example: don't go from an <h2></h2> to an <h4></h4>
// There should only be 1 <main> element per page, it's meant to surround the information of the central topic of the page and should not include things that will be reapeated throughout other pages.

//<article> - groups independent, self-contained content
//<section> - groups related content
// If you were writing a book the <article> would be the book and the <section> would be the chapters.

//<header> is used to wrap introductory information

// Use the <audio> element to wrap audio in your html, the <audio> element also takes controls as an attribute
// The <source> element is used to link to audio files in the html. It needs a src attribute (to link the audio file) and a type attribute (to specify which type of audio file it is)
/* Example:

<audio controls>
  <source src="audio/something.mp3" type="mpeg">
  <source src="audio/something.ogg" type="mpeg">
</audio>

/*

// The <figure> element is used to wrap a visual display like an image
// The <figcaption> element is used to give a short description of the image
// If a chart was displayed in html with a short description underneath it the chart would be wrapped in <figure> and the description would be the <figcaption>
/* Example:

<figure>
  <img src="images/chart.jpeg" alt="Statistics Chart">
  <figcaption>This is a chart about many statistics</figcaption>
</figure>

*/

// Use the <time> element to semanticaly wrap a date in the html
// The <time> element takes datetime as an attribute and it is used to specify the date for screen readers
/* Example: <p> <time datetime="2016-09-15">Thursday, September 15</time><sup>th</sup>.</p>

// CSS can help you hide data for visually impaired users, for example, if a page is displaying a graph the visually impaired user will need some other form of presentation like a table
/* The following CSS approaches will hide the element from everyone including screen reader users:

display: none;
visibility: hidden;
width: 0px;
height: 0px;

// Instead use this CSS approach

.sr-only {
  position: absolute;
  left: -10000px;
  width: 1px;
  height: 1px;
  top: auto;
  overflow: hidden;
}

*/

// Use the HTML attribute accesskey to give an element a shorcut to access it, this is specially useful for links and button for the visually impaired.
// Example: <a href="#" target="_blank" accesskey="c">Click Here</a>

// The attribute tabindex is used to make an element navigable with the tab key, and it is also used to give any element the ability to use the pseudo CSS selector :focus
// Tab index values that start at 1 will be tabbed first in order and then will start tabbing elements with a value of 0 in HTML order 
// Example: <p tabindex="0">Some Text</p>
