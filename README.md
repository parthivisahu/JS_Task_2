# JS_Task_2
# JavaScript File for Navigating Between Pages

This JavaScript file provides functionality to navigate from one web page to another. It allows you to move from the previous page to the next page using JavaScript.

## Usage

1. Include the JavaScript file in your HTML document using the `<script>` tag:

   ```html
   <script src="navigation.js"></script>
   ```

2. Create HTML elements such as buttons or links that trigger the navigation action:

   ```html
   <button onclick="goToPreviousPage()">Previous</button>
   <button onclick="goToNextPage()">Next</button>
   ```

   Alternatively, you can attach event listeners to elements programmatically in your JavaScript code.

3. In your JavaScript code or within a `<script>` tag, use the provided functions to navigate between pages:

   ```javascript
   function goToPreviousPage() {
     history.back();
   }

   function goToNextPage() {
     history.forward();
   }
   ```

   The `goToPreviousPage()` function uses the `history.back()` method to navigate to the previous page in the browser's history. The `goToNextPage()` function uses the `history.forward()` method to navigate to the next page, if available.

## Example

HTML:

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Page Navigation Example</title>
    <script src="navigation.js"></script>
  </head>
  <body>
    <h1>Page 1</h1>
    <button onclick="goToPreviousPage()">Previous</button>
    <button onclick="goToNextPage()">Next</button>

    <script>
      function goToPreviousPage() {
        history.back();
      }

      function goToNextPage() {
        history.forward();
      }
    </script>
  </body>
</html>
```

JavaScript (navigation.js):

```javascript
function goToPreviousPage() {
  history.back();
}

function goToNextPage() {
  history.forward();
}
```

When you click the "Previous" button, it will navigate to the previous page in the browser's history. Similarly, clicking the "Next" button will navigate to the next page if available.

Please note that the availability of the previous and next pages in the history depends on the user's browsing context. If there are no previous or next pages, the respective button click will have no effect.

You can customize the HTML elements and their event handlers according to your specific requirements and design.
