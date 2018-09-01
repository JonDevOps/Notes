// Use [att="value"] to select HTML elements by attribute and value
/* Example: 
[type="input"] {
  padding: 10px;
}
*/

// Use :before and :after selectors to change the before and after of an element.
//For the :before and :after selectors to function properly, they must have a defined content property. It usually has content such as a photo or text. When the :before and :after selectors add shapes, the content property is still required, but it's set to an empty string.
/* Example: 

.heart:before {
  content: "";
  background-color: yellow;
  border-radius: 25%;
  position: absolute;
  height: 50px;
  width: 70px;
  top: -50px;
  left: 5px;
}
