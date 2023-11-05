# Age-Claculator-
### Hosted Link: https://divyanshrajpoot9.github.io/Age-Claculator-/
### Java Script DOM Manipulation:
The Document Object Model (DOM) is a programming interface for web documents. It provides a structured representation of a web page, allowing you to access and manipulate its elements and content using JavaScript. Here are some basic DOM properties and methods.
document: The document object represents the entire HTML document and serves as the entry point to the DOM. It provides properties and methods to access and modify the document's structure, content, and style.

### Element Selection and Traversal:

  ### getElementById(id): Retrieves an element by its unique id attribute.
  #### getElementsByClassName(className): Returns a collection of elements with a specific class name.
  ####  getElementsByTagName(tagName): Returns a collection of elements with a specific tag name.
  ####  querySelector(selector): Returns the first element that matches the CSS selector.
  ####  querySelectorAll(selector): Returns a list of all elements that match the CSS selector.

1. The code starts by getting references to three HTML elements using their IDs and stores them in the variables `outputYears`, `outputMonths`, and `outputDays`. These elements are expected to be used to display the output of the date difference calculations.

2. It then creates a `Date` object named `currentDate` to represent the current date and time.

3. It retrieves the current year, month, and day from the `currentDate` object and stores them in the variables `year`, `month`, and `day`, respectively.

4. The code also gets a reference to an HTML input element with the ID 'input-date' and a button with the ID 'calculate' using `getElementById`. These will be used to collect the user's input date and trigger the calculation.

5. An event listener is added to the 'calculate' button, which listens for a click event. When the button is clicked, the code within the event listener function is executed.

6. Inside the event listener function:
   - It retrieves the value entered by the user in the 'input-date' input field and converts it into a `Date` object named `inputdateValue`. This allows the code to work with the user's chosen date.

   - It extracts the day, year, and month components from the `inputdateValue` object and stores them in the variables `inputDay`, `inputyear`, and `inputmonth`.

   - It checks if the user's input date is in the future, i.e., greater than the current date. If this condition is met, it displays an alert to the user, indicating that they need to enter a valid date. The `return` statement is used to exit the event listener function, preventing further calculations.

7. After ensuring the input date is valid, the code proceeds to calculate the differences in days, months, and years between the user's input date and the current date. The differences are stored in the variables `fday`, `fmonth`, and `fyear`.

8. To handle cases where the difference in months is negative or the difference in months and days is both negative, the code performs the necessary adjustments to `fyear` and `fmonth`. If `fmonth` is negative, it subtracts 1 from `fyear` and adds 12 to `fmonth`. If `fday` is negative, it calculates the last day of the previous month and adds it to `fday`, while also subtracting 1 from `fmonth`.

9. The code then checks if `fmonth` has become -1 after adjustments, which would indicate a need to wrap around to December and decrement `fyear` by 1. This ensures that the months are represented correctly in the output.

10. Finally, the calculated differences in years, months, and days (`fyear`, `fmonth`, and `fday`) are displayed in their respective HTML elements with IDs 'outputYears', 'outputMonths', and 'outputDays using the `innerText` property.

In summary, this code calculates the difference in years, months, and days between the current date and a user-provided input date, considering edge cases and adjustments as needed, and then displays the results in the specified HTML elements.
![Screenshot 2023-11-05 223503](https://github.com/divyanshrajpoot9/Age-Claculator-/assets/114856467/8a556c18-f069-4200-ae49-7b2875b1717d)
![Screenshot 2023-11-05 223651](https://github.com/divyanshrajpoot9/Age-Claculator-/assets/114856467/5e81c925-47ae-4a75-a8b8-25668198a42a)
![Screenshot 2023-11-05 223526](https://github.com/divyanshrajpoot9/Age-Claculator-/assets/114856467/3f2413b8-da68-4dab-8901-2bf385f7fa8f)
