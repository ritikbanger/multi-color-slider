# Slider with Tooltip (multi-color-slider)

## Overview

This project creates a custom range slider with a dynamic tooltip. The tooltip displays the current value of the slider and moves along with the slider thumb. The project is built using HTML, CSS, and JavaScript.

## Features

- **Custom Range Slider**: A horizontally sliding range input for selecting a numeric value.
- **Dynamic Tooltip**: A tooltip that shows the current value of the slider and follows the slider thumb.
- **Responsive Design**: Ensures the slider looks good on various devices and screen sizes.
- **Customizable Style**: Easy to customize with CSS variables.

## Installation

To use the slider in your project, follow these steps:

1. **Clone or Download the Repository**

   - Clone this repo to your local machine or download the zip file.

2. **Open the File**
   - Open the `old-version.html` file in a web browser to see the slider in action.

Certainly! To add an explanation of the code to the README, you can include sections that describe the structure and functionality of the HTML, CSS, and JavaScript components. Here's how you can enhance the README to include these explanations:

## Code Explanation

### HTML Structure

The HTML consists of a `div` element with the class `slider-container`, which contains:

- An `input` element of type `range`, representing the slider.
- A `div` element with the class `tooltip`, used to show the slider value.

### CSS Styling

- **Font and Body**: The Roboto font is used for styling. The body is styled to center the slider on the page.
- **Slider Container**: The `.slider-container` class defines the positioning and styling of the container holding the slider.
- **Range Input**: Styles for the range input (`input[type="range"]`) include width, cursor style, and color (accent-color).
- **Tooltip**: The `.tooltip` class styles the tooltip, including position, size, color, and transitions for smooth display and hiding.

### JavaScript Functionality

- An event listener is added to the slider input. On the `input` event (as the slider is moved), the following actions occur:
  - The slider value is updated.
  - The `--value` CSS variable is updated to reflect the current value, affecting the accent color of the slider.
  - The `--thumb-pos` CSS variable is updated to move the tooltip along with the slider thumb.
  - The tooltip's `value` attribute is updated with the current value of the slider.

## Customization

You can customize the appearance and behavior of the slider by modifying the CSS and JavaScript code.

- **CSS Variables**: Adjust the colors, sizes, and other properties using the CSS variables defined in the style section.
- **JavaScript Options**: Modify the JavaScript to change how the tooltip behaves or interacts with other elements.

## Browser Compatibility

This slider has been tested on modern web browsers like Chrome, Firefox, and Edge. For full compatibility, ensure your browser supports HTML5, CSS3, and ES6 JavaScript.

## License

This project is open-source and free to use. Feel free to modify and distribute it as per your requirements.

## Contributing

Contributions to enhance the functionality or design of the slider are welcome. Please follow the standard procedures for contributing to open-source projects.
