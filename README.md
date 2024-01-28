# css-grid-playlist
Course files for the [CSS Grid playlist](https://www.youtube.com/watch?v=x7tLPhnA06w&list=PL4cUxeGkcC9itC4TxYMzFCfveyutyPOCY&index=1) on The Net Ninja YouTube channel.

See different branches in this repo for each lesson example.

# My Super Brief Lesson Summaries

1. Why use CSS Grid?\
Compare with float, compare with flex.

2. Columns\
`display: grid;`\
`grid-template-columns: repeat(4, 1fr);` - define your columns

3. Rows\
`grid-auto-rows: minmax(150px, auto);` - define max height of each row \
`grid-template-rows: repeat(3, minmax(150px, auto));` - alternative to `grid-auto-rows`. Explicitly define number of rows.\
`grid-gap: 1rem;` - a way to specify space between your columns and rows. Can use `grid-row-gap` or `grid-column-gap` instead if you only want to specify gap between rows or columns respectively.

4. Positioning elements in your CSS Grid (Grid Lines)\
`grid-column: 1 / 3;`\
`grid-row: 2 / 4;`

5. Nested CSS Grids\
Nothing special needed to nest a CSS grid in another - just set up styles for container and items!\
Bonus tip: `grid-column: span 3;` is another way to say `grid-column: 1 / 4;`.

6. Aligning & Justifying Items\
`align-items: start;` - vertical\
`justify-items: end;` - horizontal

7. 12 column grid system\
Example includes an overlay to visualize the grid columns/rows (Note: modern browser devtools can do this for you).

8. Mosaic Layout Example\
Bonus - a simple transform like `transform: rotateZ(45deg) scale(0.7)` can make layouts like this look really cool.

1. Grid Areas\
Give your items in the grid layout names like this: `grid-area: header;`\
Then define your layout in the container element like this:
```
grid-template-areas: 
	"header header header header"
  "aside . main main"
  "nav . main main"
  "section section section section"
  "section section section section"
  "footer footer footer footer";
```

10.  Responsive Grid Example\
Define two `grid-template-area` rules - one for desktop and another for mobile.
 