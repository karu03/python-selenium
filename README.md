# python-selenium

Summary:
Setup:

The script begins by setting up the Chrome WebDriver using the webdriver_manager to install the necessary Chrome driver.
Navigating to the Form:

The Google Form URL is loaded using driver.get().
Function Definition:

A function fill_form() is defined to handle the process of filling out and submitting the form.
Within this function, the XPaths of various form fields are defined to locate the input elements on the form.
Helper Functions:

wait_for_element_to_be_interactable(): This function waits until a specific element is visible and interactable.
scroll_to_element(): This function scrolls the webpage to bring a specific element into view.
Filling the Form:

The script locates each form field by its XPath, scrolls to the element, and then inputs the predefined data (e.g., full name, contact number, email, address, pin code, date of birth, gender, and verification code).
Submitting the Form:

After all fields are filled, the script locates and clicks the "Submit" button.
Post-Submission:

The script waits for a confirmation message indicating that the response has been recorded.
It then captures a screenshot of the submitted response for proof.
Error Handling:

The try block ensures that if any error occurs during the form-filling process, it will be caught and printed.
Finally, the WebDriver is closed using driver.quit() to clean up the resources.
Key Points:
Automation: The script automates the manual task of filling out a Google Form.
Error Handling: Ensures the script handles potential issues gracefully and closes the browser session.
Screenshot: Captures a screenshot of the confirmation message as proof of submission.
Reusability: The helper functions can be reused for other similar tasks involving form filling or web interactions.
This approach is efficient for automating repetitive tasks and can be adapted to other web forms with similar structures by updating the XPaths and input data.
