The Chef Menu Application was developed to help the chef manage his restaurant's menu by allowing him to add dishes, categorize them by course, and calculate the total price at checkout. Built using React Native, this application provides a simple interface for the chef to organize his dishes and navigate between different views.
2.1 Objectives
The main objectives of the application were:
•	To allow the chef to add 
•	To limit the dish categories (courses) to three specific options: starter, main, and dessert.
•	To enable the selection of dishes for checkout and the total cost calculation.
2.2 Features
The application was designed with the following key features:
1.	Home Screen: Displays the menu and allows the chef to add dishes and select items for checkout.
2.	Add Dish Screen: Allows the chef to enter dish details such as name, description, course, and price.
3.	Course Selection: Limits the course input to predefined options (starter, main, dessert) through manual input validation.
4.	Checkout Screen: Displays selected dishes and their total price.
3.1 Tools and Technologies Used
•	TypeScript: Used to ensure type safety and improve debugging efficiency.
•	React Navigation: Implemented to handle navigation between the home, add dish, and checkout screens.
•	State Management: React's useState hook was used to manage the state locally within each screen, such as the list of dishes and selected items.
•	Error Handling and Validation: Used for input validation and feedback to the chef when adding new dishes.
3.2.1 Home Screen
The Home Screen was designed to list all menu items dynamically and allow the chef to select items for checkout. The following features were included:
•	FlatList: Used to render the menu items.
•	TouchableOpacity: Enabled chefs to select or deselect menu items by tapping on them.
•	Buttons for adding new dishes and proceeding to checkout were added at the bottom of the screen.

3.2.2 Add Dish Screen
In the Add Dish Screen, chef will be able to manually input the dish's details:
•	TextInput fields were used for entering the dish name, description, and price.
•	Input validation was added to ensure only valid courses could be entered. This validation limited the input to three specific courses: starter, main, and dessert.
3.2.3 Checkout Screen
The Checkout Screen summarized the selected dishes and displayed the total price. If no items were selected, an alert would prompt the client to select at least one item before proceeding to checkout. The total price was calculated by summing the prices of all selected dishes.
3.3 Image Backgrounds
To enhance the visual appeal, image backgrounds were added to both the Home Screen and the Add Dish Screen using the ImageBackground component. This gave the app a professional look that aligned with the culinary theme.
3.4 Input Validation and Error Handling
Validation was implemented to ensure that all input fields were correctly filled before adding a dish. Specifically:
•	The price had to be a positive number.
•	The course had to be either "starter," "main," or "dessert."
•	If any field was invalid, an alert would prompt the chef to correct the errors.

4. Challenges Faced
During the development, a few challenges were encountered:
Ensuring Correct Course Input: While initially considering a picker for course selection, the decision to use a text input field with validation provided more flexibility for the chef.
State Management Across Screens: Passing the new dish data between the "Add Dish" and "Home" screens required careful state management using navigation parameters.

5. Testing and Debugging
The application was tested on both Android and iOS simulators to ensure compatibility and functionality. Some of the key aspects tested included:
•	Adding, selecting, and deselecting dishes.
•	Input validation for dish details.
•	Navigation between the home, add dish, and checkout screens.
•	Accurate calculation of the total price.
6. Conclusion
The Chef Menu Application was successfully developed, allowing the chef to easily manage his menus, limit dish categories to predefined courses, and navigate between adding dishes and proceeding to checkout. By using React Native. Further development could involve adding more features like persistent storage or integrating a backend to save the menu items in a database, which would enhance the overall functionality.
