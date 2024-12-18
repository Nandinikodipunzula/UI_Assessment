# Interactive UI:

This project demonstrates three interactive UI components:

1. Dynamic Tree Menu - A collapsible tree menu with clickable items that update the content on the right side of the screen.
2. Category Search Layout - A sidebar with a search feature to filter categories, where each category dynamically updates the content when clicked.
3. Table of Contents (TOC) - A content area with a search-enabled table of contents that allows users to navigate and view dynamic content by clicking category links.

## Features

### 1. Dynamic Tree Menu

- Collapsible Tree Structure: The tree displays nested items, and users can expand/collapse items to view their children.
- Content Update: When a tree item is clicked, the content on the right side of the page is updated to reflect the clicked item's name.
- Arrow Indicators: Each parent item in the tree menu has arrows indicating whether it can be expanded or collapsed. Leaf nodes (those without children) do not show arrows.
- Modal Dialog (optional): A modal dialog can appear when clicking on a tree item to show additional information about the selected item.

### 2. Category Search Layout

- Sidebar with Search: A search bar allows users to filter through dynamically generated categories.
- Category List: The sidebar contains a list of category buttons. Clicking any category updates the content area with the corresponding information.
- Dynamically Generated Categories: For demonstration purposes, categories are dynamically generated using JavaScript.
- Filter Functionality: As the user types in the search bar, the category buttons update in real-time to show only those that match the search text.

### 3. Table of Contents (TOC)

- Dynamic TOC: A table of contents is populated with dynamically generated category links.
- Searchable TOC: Users can filter through the TOC using a search bar.
- Content Sections: Each category is linked to a section in the content area. Clicking a TOC item scrolls the user to the corresponding content.
- Dummy Content Generation: Content sections are populated with dummy text to simulate real content.

## How It Works

### 1. Dynamic Tree Menu

- The HTML structure defines a nested list (`<ul>` and `<li>`) representing the tree structure.
- JavaScript is used to toggle the visibility of child elements when the user clicks on a parent item. The arrow symbols change based on whether the node is expanded or collapsed.
- The content area is updated dynamically when a user clicks on any item in the tree, displaying the item's name and description.

### 2. Category Search Layout

- Categories are displayed as buttons within the sidebar. JavaScript is used to dynamically generate a large number of categories for demonstration purposes.
- When a category is clicked, the content area is updated with a title and description related to that category.
- The search bar allows the user to filter through the categories. As the user types, categories that do not match the search criteria are hidden, improving the user experience for larger sets of categories.

### 3. Table of Contents (TOC)

- The TOC is dynamically populated with links to different categories. Each link corresponds to a section in the content area.
- The search functionality allows users to filter the TOC by typing in the search bar. Only matching items are displayed.
- Clicking on a TOC link scrolls the user to the associated content section, where they can read more details about the category.

## Code Structure

### HTML Structure

- `<div id="content-container">`: Contains the table of contents (TOC) and content area sections.
- `<div id="toc">`: Contains the search bar and the list of category links in the table of contents.
- `<div id="content-area">`: Displays the dynamic content for the selected category.

### JavaScript Functionality

- Event Listeners: The dynamic behaviors (e.g., toggling the tree menu, filtering categories, updating content, scrolling to TOC sections) are handled by event listeners that trigger functions based on user interactions.
- `filterTOC()`: Filters the table of contents items based on the user's input in the search bar.
- `generateDummyContent()`: Generates dummy content for the category sections in the content area.

### CSS Styling

- Layout: The layout uses Flexbox to divide the page into the TOC and content area.
- TOC Styling: Includes styles for the search bar, category links, and hover effects on links in the TOC.
- Content Area Styling: Ensures the content area is spacious, scrollable, and visually distinct.

## Installation

1. Copy the provided HTML, CSS, and JavaScript code into an HTML file (e.g., `index.html`).
2. Open the HTML file in a modern web browser.
3. Interact with the tree menu, category search layout, or table of contents to view dynamic content.

## Example Usage

### Dynamic Tree Menu Example

- Click on "Root": Expands or collapses child nodes. Updates the content area with "Root".
- Click on "Parent A": Displays information about "Parent A" in the content area.
- Click on "Child A1": Displays information about "Child A1" in the content area.

### Category Search Layout Example

- Use the Search Bar: Type to filter through categories.
- Click on a Category Button: The content area updates to show the selected category's information.

### Table of Contents Example

- Use the TOC Search Bar: Type to filter through categories in the TOC.
- Click on a Category Link in the TOC: The page scrolls to the corresponding content section.

## Customization

- Add More Categories: You can easily add more categories by adding more `<a>` elements inside the `#toc-list` or `<button>` elements inside the `#categoryList`.
- Modify the Tree Structure: Modify the `<ul>` and `<li>` elements to add or remove nodes in the tree menu.
- Modify Dummy Content: You can replace the dummy content with real content by modifying the `generateDummyContent()` function.
