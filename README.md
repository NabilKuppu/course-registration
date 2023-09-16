State Management in Course Registration Platform
In this project, we use React.js for building a course-selling platform. State management is essential for tracking and updating key information like remaining credit, total credit hours, and total price. The state is primarily managed within the App component.

States Maintained
Three main states are maintained to manage the core functionality of the platform:

1.remainingCredit: This state is responsible for displaying the remaining credit hours that a user has after adding courses to their cart. It helps users keep track of how many more credits they can allocate.

2.totalCredit: The totalCredit state is used to display the total number of credit hours selected by the user. It reflects the cumulative credit hours of all the courses in the cart.

3.totalPrice: This state is responsible for displaying the total price of the selected courses. Each course may have a different price, and this state keeps track of the overall cost.

#Component Interaction
The core components involved in state management are:

\*App Component: The App component is the top-level component that holds the state. It initializes the remainingCredit, totalCredit, and totalPrice states. It also renders child components and passes relevant data to them via props.

\*Card Component: The Card component represents individual courses that users can select. It handles events like adding courses to the cart and calculating the impact on state. When a user interacts with a course card, the Card component communicates with the App component to update the state.

\*Cart Component: The Cart component is responsible for displaying essential information to the user, such as total credit hours and total price. It receives data from the App component via props and updates its display accordingly.

##Key Features
Here are some key features of the course registration platform:

\*\*Responsive Design: The platform is fully responsive, ensuring a seamless user experience on different devices and screen sizes.

\*\*Preventing Duplicates: Users are prevented from adding duplicate courses to their cart. If they attempt to do so, a notification is displayed to inform them of this restriction.

\*\*Displaying Essential Information: The Cart component displays important information, including the total credit hours, remaining credit hours, and total price. This helps users make informed decisions.

\*\*Error Handling: The platform also provides error handling. If a user enters credit hours less than 0 or greater than 20, alerts are shown to notify them of these invalid inputs.

By following this state management structure and component interaction pattern, developers can easily grasp how the project works and make further enhancements or modifications as needed.
