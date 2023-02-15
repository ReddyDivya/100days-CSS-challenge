## Day 5 - Statistics

## Pseudo Elements

### ::before

  - It creates a pseudo-element that is the first child of the selected element. 
  - It is often used to add cosmetic content to an element with the content property. 
  - It is inline by default.

   ### Example
   
     p::before {
        content: "Read this: "; /* adds this to before of the 'p' content */
      }
      
     <p>My name is Donald</p>
     <p>I live in Ducksburg</p> 
     
     Output
     ------
     Read this: My name is Donald
     Read this: I live in Ducksburg

---

## Sass @extend and Inheritance

  - The @extend directive lets you share a set of CSS properties from one selector to another.
  - The @extend directive is useful if you have almost identically styled elements that only differ in some small details.

  ### Example
  
    .button-basic  {
      border: none;
      padding: 15px 30px;
      text-align: center;
      font-size: 16px;
      cursor: pointer;
    }

    .button-report  {
      @extend .button-basic; /* extending .button-basic style to .button-report */
      background-color: red;
    }

    .button-submit  {
      @extend .button-basic;  /* extending .button-basic style to .button-submit */
      background-color: green;
      color: white;
    }

  ### After Compilation it will look like below
  
    .button-basic, .button-report, .button-submit {
      border: none;
      padding: 15px 30px;
      text-align: center;
      font-size: 16px;
      cursor: pointer;
    }

    .button-report  {
      background-color: red;
    }

    .button-submit  {
      background-color: green;
      color: white;
    }

---

## Sass Ampersand

---

## SVG (Scalable Vector Graphics)
    
   - SVG defines vector-based graphics in XML format.
   - SVG defines the graphics in XML format.
   - Every element and every attribute in SVG files can be animated.

  ### SVG circle
  
   - The cx and cy attributes define the x and y coordinates of the center of the circle.
   - If cx and cy are omitted, the circle's center is set to (0,0)
   - The r attribute defines the radius of the circle.
   - stroke - border color
   - fill - background color
   - stroke-width - width of the stroke

  ### Example
   
     <svg width="100" height="100">
      <circle cx="50" cy="50" r="40" stroke="green" stroke-width="4" fill="yellow" />
     </svg>
  
  ### SVG polyline
    
   - The <polyline> element is used to create any shape that consists of only straight lines (that is connected at several points)
   - The points attribute defines the list of points (pairs of x and y coordinates) required to draw the polyline
   - stroke - border color
   - fill - background color
   - stroke-width - width of the stroke
   - points - polyline directions

  ### Example
  
      <svg height="200" width="500">
        <polyline points="20,20 40,25 60,40 80,120 120,140 200,180"
        style="fill:none;stroke:black;stroke-width:3" />
      </svg>

      /* or */

      <svg height="200" width="500">
        <polyline points="10, 40 80,120 120 290" fill="none" stroke="red" stroke-width="14"/>
        Sorry, your browser does not support inline SVG.
      </svg>

  ---  
