# jQuery Registration Forms

This repository contains 3 different registration form templates built using jQuery with proper validations. These templates offer a simple and effective way to implement registration forms with client-side validation.

## Features

- Three different registration form templates:
  1. **Bootstrap Style Form**
  2. **Material Design Style Form**
  3. **Custom Style Form**
- Validation for all required fields (e.g., name, email, password).
- Real-time input validation feedback.
- Easy integration into any web project.

## Technologies Used

- jQuery
- HTML5
- CSS3
- Bootstrap (for styling in one of the templates)

## How to Use

1. Clone or download this repository.
2. Open the HTML file of the form template you want to use in a browser.
3. The form will automatically include validation. Enter data in the form fields and submit to test the validation.
4. You can customize the templates by editing the HTML, CSS, or jQuery code as per your needs.

## Example

Here's a quick look at the code for the Bootstrap Style Registration Form:

```html
<!-- Registration Form HTML -->
<form id="registerForm">
  <input type="text" id="name" placeholder="Name" required>
  <input type="email" id="email" placeholder="Email" required>
  <input type="password" id="password" placeholder="Password" required>
  <button type="submit">Register</button>
</form>
```

```javascript
// jQuery validation for the registration form
$(document).ready(function() {
  $('#registerForm').submit(function(e) {
    e.preventDefault();
    // Perform validation here
    if ($('#name').val() === '' || $('#email').val() === '') {
      alert('Please fill in all required fields.');
    } else {
      alert('Form submitted successfully!');
    }
  });
});
