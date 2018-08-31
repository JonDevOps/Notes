// To create a CSS grid use the display property
// Example: display: grid;

// Use the grid-template-columns property to add grids
// The grid-template-columns property takes in values as width, each value represents a column of grids
/* Example: 

.container {
  display: grid;
  grid-template-columns: 50px 50px 50px 50px;
}

/*
// This creates a grid with 4 columns that are 50px each.

// The grid-template-rows property is used to set the rows in a grid
// The grid-template-rows property takes values as row width and each value represents a new row
/* Example: 

.container {
  display: grid;
  grid-template-columns: 50px 50px 50px 50px;
  grid-template-rows: 50px 50px 50px 50px;
}

*/ 

// The grid-template-columns and grid-template-rows take px, em, %, auto and fr as possible values.
// The value auto sets the width or height to the size of its content
// The value fr sets the column or row to a fraction of the available space.
/* Example: 

.container {
  display: grid;
  grid-template-columns: auto 50px 10% 2em 2fr;
} 

*/

// Use the grid-column-gap and grid-row-gap to add space between columns or rows.
/* Example: 

.container {
  display: grid;
  grid-template-columns: auto 50px 1em 10% 1fr;
  grid-template-columns: auto 50px 1em 10% 1fr;
  grid-column-gap: 10px;
  grid-row-gap: 10px;
}

*/

// Use the property grid-gap to add a gap between rows or columns
// if grid-gap has 1 value it will add that to gaps between rows and columns but if it has two it will take the first value as the row gap and the second as the column gap
/* Example: 

.container {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr 1fr;
  grid-template-rows: 1fr 1fr 1fr 1fr;
  grid-gap: 20px 15px;
}

*/

// Use the property grid-column on grid items to specify how many grids a grid item will take
// Grids are made out of column lines and row lines starting from the top as 1, use these as values to specify where it will start and where it will end.
/* Example: 

.item-1 {
  grid-column: 2 / 4; /* This makes the item take 2 grids on the right */
}

*/

// Use grid-row property on grid items to control the amount of rows they take up
// They work just like the example above.
/* Example: 

.item-1 {
  grid-column: 2 / 4;
  grid-row: 2/4; /* This will take the last 2 rows on a 3x3 grid */
}

*/

// Use the justify-self on grid items to align their contents horizontally
// The justify-self property take start, center, and end as values (stretch is it's default value)
/* Example:

.item-1 {
  justify-self: center;
}

*/

// The align-self property is aligns the grid-item's content vertically and is similar to the justify-self property and takes the same values
/* Example: 

.item-1 {
  align-self: end;
}

*/

// Use the justify-items and align-items properties on the grid container to align all of the grids the same way
/* Example:

.container {
  align-items: center;
  justify-items: center;
}

*/

// The property grid-template-areas are used to group grids into an area with a custom name
// Every word in the code represents a cell and every pair of parenthesis represents a row
// In addition you can use a . to designate an empty cell on a grid
/* Example:

.container {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  grid-template-rows: 1fr 1fr 1fr;
  grid-gap: 10px;
  grid-template-areas: 
  "header header header"
  "advert content content"
  "footer footer footer";
}

*/

// The grid-area property causes an item to move to that specific area
/* Example: 

.item-1 {
  grid-area: footer; /* This will cause an the item to take up the whole footer area if there are no other items in that area */
}

*/

// Use the grid-area property to create grid areas on the fly
/* Example:

.item {
  grid-area: 3/1/4/4; /* row line start / column line start / row line end / column line end */
}

*/

// Use the repeat function as a value for the grid-template-rows and grid-template-columns properties
// This makes it so you don't ahve to repeat values manually, it'd be hard to write 100 rows by hand for example
// The first value represent the amount of times the repeat function will be repeated, the second value represents the size of the value
/* Example: 

.container {
  display: grid;
  grid-template-columns: repeat(5, 10px); /* This will make 5 columns 10px wide */
  grid-template-rows: repeat(2, 1fr 20px) 10px; /* This translates into grid-template-rows: 1fr 20px 1fr 20px 10px; */
}

*/

// The minmax function is another value for the grid-template-columns and grid-template-rows properties
// This property sets the first value as the min-width of the cell and the second value as the max-wdith of the cell
/* Example: 

.container {
  grid-template-columns: repeat(3, minmax(90px, 1fr));
  grid-template-columns: repeat(3, 1fr);
}

*/

// auto-fill is an option for the repeat function
// It allows you to automatically insert as many rows or columns of your desired size as possible depending on the size of the container
// It allows you to create complex layouts when conbined with minmax
/* Example: 

.container {
  display: grid;
  grid-template-column: repeat(auto-fill, minmax(90px, 1fr));
  grid-template-rows: repeat(auto-fill, minmax(90px, 1fr));
}

*/

// auto-fit works almost exactly like auto-fill the difference is that auto-fit will stretch the cell to fill the remainding space
/* Example:

.container {
  display: grid;
  grid-template-columns: repeat(auto-fill, mimmax(90px, 1fr));
  grid-template-rows: repeat(auto-fill, minmax(90px, 1fr));
}



