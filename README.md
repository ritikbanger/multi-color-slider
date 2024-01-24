# Slider with Tooltip (multi-color-slider)

## Video Demonstration

To see a demonstration of the slider with tooltip, you can view the video here:

![see here](https://github.com/ritikbanger/multi-color-slider/blob/main/demo-video.gif)

# old-version.html file

## Overview

This project creates a custom range slider with a dynamic tooltip. The tooltip displays the current value of the slider and moves along with the slider thumb. The project is built using HTML, CSS, and JavaScript.

## Features

- **Custom Range Slider**: A horizontally sliding range input for selecting a numeric value.
- **Dynamic Tooltip**: A tooltip that shows the current value of the slider and follows the slider thumb.
- **Responsive Design**: Ensures the slider looks good on various devices and screen sizes.
- **Customizable Style**: Easy to customize with CSS variables.

## Codepen

![codepen](https://codepen.io/Ritik-Banger/pen/VwRzobv)

## Installation

To use the slider in your project, follow these steps:

1. **Clone or Download the Repository**

   - Clone this repo to your local machine or download the zip file.

2. **Open the File**
   - Open the `old-version.html` file in a web browser to see the slider in action.

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

# new-version.html file

## Overview

This HTML and CSS project demonstrates an interactive slider with a tooltip feature. The slider is styled using advanced CSS properties, including custom properties (`--value`), CSS Grid, Flexbox, and animations. It utilizes new CSS features like `@property`, `anchor-position`, and `view-timeline` to enhance user interaction and design.

## Features

- **Responsive Design**: Flexbox and Grid are used for layout, making the slider responsive to different screen sizes.
- **Dynamic Tooltip**: Displays the current value of the slider in a tooltip that moves with the slider thumb.
- **Advanced CSS Properties**:
  - `@property --value`: A custom property to track the slider's value.
  - `anchor-name` and `view-timeline`: These experimental properties are used in the `::-webkit-slider-thumb` for advanced interactions.

## Codepen

![codepen](https://codepen.io/Ritik-Banger/pen/bGZoNpR)

## Browser Compatibility

- The use of cutting-edge CSS properties (`anchor-name`, `view-timeline`) may have limited support across browsers. Check compatibility on [Can I Use](https://caniuse.com/) for [CSS Anchor Position](https://drafts.csswg.org/css-anchor-position-1/), [Easing Function Linear Function](https://caniuse.com/mdn-css_types_easing-function_linear-function), and [View Timeline](https://caniuse.com/mdn-css_properties_view-timeline).

## How it Works

1. **Slider Movement**: When the user interacts with the slider, the `input` event triggers the `updateTooltipPosition` function in JavaScript.
2. **Tooltip Update**: The tooltip's position and content update according to the slider's current value.

## Code Explanation

- `@font-face`: Loads the "Roboto" font.
- CSS `*` Selector: Ensures consistent box-sizing.
- `.tooltip`: Styled to appear as a floating label, showing the slider's value.
- CSS Custom Properties: `--value` is used for dynamically changing the slider value.
- `@supports (anchor-name: --rad)`: Provides styles for browsers supporting the `anchor-name` property.
- `::-webkit-slider-thumb`: Styles specific to the slider thumb, using experimental properties for more complex interactions.
- `:root`: Defines a timeline scope for the slider.
- `.slider-container`: Contains the slider and tooltip, styled to be visually appealing.
- Keyframe Animation: The `sync` animation gradually changes the `--value` property.
- JavaScript: Listens for slider movements and updates the tooltip position accordingly.

## Installation

To use the slider in your project, follow these steps:

1. **Clone or Download the Repository**

   - Clone this repo to your local machine or download the zip file.

2. **Open the File**
   - Open the `new-version.html` file in a web browser to see the slider in action.

## Note

The use of experimental CSS properties means that this code may not work as intended in all browsers. Always check for browser compatibility and fallbacks when using new CSS features in production environments.

## License

This project is open-source and free to use. Feel free to modify and distribute it as per your requirements.

## Contributing

Contributions to enhance the functionality or design of the slider are welcome. Please follow the standard procedures for contributing to open-source projects.
