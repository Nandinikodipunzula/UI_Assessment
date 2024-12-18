# UI_Assessment

# Dynamic Tree Menu with Content Display and Modal

This project implements a dynamic tree menu using HTML, CSS, and JavaScript. The tree menu supports expandable and collapsible nodes, displays related content upon clicking a tree item, and shows a modal with additional details when a tree item is clicked. This can be used as a navigation component for a web application, offering a smooth user interaction experience.

## Features

- Dynamic Tree Structure: The tree allows for both expandable and collapsible nodes with parent-child relationships.
- Content Display: When a tree item is clicked, its name is displayed in a content area on the right side of the screen.
- Modal Dialog: A modal window is triggered upon clicking a tree item, displaying more details.
- Leaf Node Identification: Leaf nodes (nodes without children) are styled with a circular icon and are not expandable.
- Interactive UI: Tree items can be toggled between expanded and collapsed states, with arrows indicating their current state.

## Project Structure

- `index.html`: Contains the structure and layout for the tree menu, content display, and modal dialog.
- `styles.css`: Contains the styles for the tree menu, modal dialog, and other UI components.
- `script.js`: Contains the JavaScript to handle dynamic interactions such as expanding/collapsing tree items, updating content, and handling modal functionality.

## How to Use

1. Download/Clone the repository:

   ```bash
   git clone <repository-url>
   ```

2. Open the `index.html` file in your browser.

3. Interact with the Tree Menu:

   - Click on a tree item to toggle its child nodes (expand/collapse).
   - When you click on a tree item, the title of the item will appear in the content area on the right.
   - A modal dialog will also appear with the name of the clicked tree item.

4. Leaf Nodes: Click on leaf nodes (nodes without children) to see the related content and trigger the modal dialog.

## Technologies Used

- HTML: Provides the structure of the page, including the tree menu, content area, and modal.
- CSS: Styles the tree menu, modal dialog, and the overall layout for a clean and user-friendly design.
- JavaScript: Handles dynamic interactivity, such as toggling the tree menu, updating content, and displaying the modal.
