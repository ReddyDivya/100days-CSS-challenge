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

      


