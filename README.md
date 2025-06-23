# weekly-cleaning-rotation-ui

This is a simple and responsive web interface to manage weekly cleaning tasks in a shared apartment. It assigns cleaning duties fairly across 1 to 7 people and visually highlights who is responsible each week.

## Features

- Auto-rotating weekly assignment (Monday to Sunday)
- Circular layout with visual indicator for the current cleaner
- Date range for the assigned cleaning week
- Dropdown to select number of participants (1 to 7)
- Legend mapping persons (P1–P7) to room numbers
- Responsive layout for mobile and desktop
- Bootstrap 5 integration

## Technologies Used

- HTML5
- CSS3
- JavaScript (Vanilla)
- Bootstrap 5

## Usage

1. Open `index.html` in any browser.
2. Use the dropdown to choose the number of people sharing the apartment.
3. The rotation updates automatically based on the current calendar week.
4. Assignments reset every Monday.

## Configuration

- To change the starting week, edit the `baseWeek` variable in the JavaScript section.
- You can customize participant names or room mapping in the `names` array and `.legend` HTML.

## Example Logic

If baseWeek is set to 21 and the current week is 26:
```js
index = (26 - 21) % 7 = 5 → P6 cleans this week
