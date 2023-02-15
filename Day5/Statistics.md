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

      


