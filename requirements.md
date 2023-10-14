# Software Requirements
## Vision
1. What is the vision of this product? 
 - Ricepify wants to make cooking more fun and easy for everyone. It's like a friendly kitchen where you can find, save, and share yummy recipes. We want to help you discover new dishes and connect with other food lovers.
2. What pain point does this project solve?
 - Have you ever had trouble finding good recipes online? Ricepify solves that. It streamlines the process of finding and sharing culinary creations, offering a user-friendly experience that saves time and reduces the hassle of sifting through numerous sources.
3. Why should you care about our product?

 - If you love cooking or want to learn, Ricepify is your kitchen buddy. You can save your favorite recipes, rate them, and even share your own creations. It's a community of food lovers, here to inspire you and make your cooking journey awesome!


## Scope (In/Out)
> IN
1. User Authentication:

Users can create accounts and log in securely. This ensures a personalized experience and keeps their information safe.
2. Recipe Discovery:

Users can access a diverse collection of culinary creations from trusted external sources through the integrated API.
3. Recipe Interaction:

Users can interact with recipes by rating them, adding them to favorites, and leaving comments.
4. Comment Management:


Users can add, and delete comments on recipes, allowing for meaningful interactions with the community.

5. Personal Recipe Collection:

Users have the ability to create and manage their own collection of favorite recipes for easy access.

6. Effortless Recipe Search:

Users can easily search for recipes by ingredient, cuisine, or creator, streamlining the process of finding specific dishes.

> OUT
1. What will our product **not do**.

Our web application will not include a feature for ordering ingredients or providing e-commerce functionality. We are focused on creating a platform for discovering and sharing recipes, rather than facilitating transactions for purchasing ingredients or kitchen tools

## Minimum Viable Product (MVP):
> MVP functionality will include:

- User Authentication:

Allow users to create accounts, log in, and log out securely.
- Explore External Recipes:

Access a diverse collection of culinary creations from trusted external sources through the integrated API.
- Recipe Interaction:

Users can rate recipes and add them to their favorites.
- Comment Management:

Users can leave comments on recipes.

Effortless Recipe Search:

Users can search for recipes by ingredient, cuisine, or creator.

> Stretch Goals:

- Recipe Sharing on Social Media:

Enable users to share recipes on their social media platforms.
- Advanced Search Filters:

Implement advanced search options, such as dietary restrictions or cooking time.
- Recipe Collections:

Allow users to create and manage collections of recipes based on themes or occasions.
- Email Notifications:

Send users notifications for actions like new comments on their recipes or when they receive likes.


## Functional Requirements

>> Functional Requirements:

1. User Authentication and Authorization:

Users can create accounts, log in, and log out securely.

Users have different levels of access (e.g., regular user).

2. User Profile Management:

Users can update their profile information, including details like name, profile picture, and personal preferences.
3. Recipe Interaction:

Users can rate recipes and add them to their favorites.
Users can leave comments on recipes.
4. Recipe Creation :

Users can create their own recipes.



6. Recipe Search and Discovery:

Users can search for recipes by ingredient, cuisine, or creator.

>> Data Flow:

- User Registration and Authentication:

   - User navigates to the registration page and creates an account.
   - User logs in with their credentials.
- Profile Management:

   - User accesses their profile page and updates information like name and profile picture.
- Recipe Interaction:

   - User browses recipes, selects one, and rates it. They also leave a comment.
- Recipe Creation and Sharing:

   - User decides to share their own recipe, providing details and instructions.
- Recipe Search and Discovery:

  - User searches for recipes by entering ingredients and selects a cuisine preference.
  - 
- External API Integration:

   - The application sends a request to the external recipe API to fetch additional recipes.

- User Logs Out:

   - User logs out when they are done using the application.



## Non-Functional Requirements

>> Non-Functional Requirement 1: Security

Security is paramount to protect user data and ensure the integrity of the platform. This includes safeguarding user accounts, personal information, and any interactions within the application.

### Implementation:

- Secure Authentication: Passwords will be securely hashed and stored using industry-standard cryptographic techniques (e.g., bcrypt).
- HTTPS: The application will utilize HTTPS to encrypt data transmitted between the user's browser and the server, preventing eavesdropping or data tampering.
- Authorization Checks: Proper authorization checks will be implemented to ensure users can only access the functionalities they are permitted to.
- Input Validation: Data input from users will be validated and sanitized to prevent injection attacks (e.g., SQL injection, XSS).

>> Non-Functional Requirement 2: Usability

 Usability focuses on providing an intuitive and user-friendly experience to maximize user satisfaction and engagement.

### Implementation:

- Intuitive User Interface (UI): The UI will be designed with user experience in mind, ensuring clear navigation, consistent layouts, and intuitive controls.
- Responsive Design: The application will be responsive to various screen sizes and devices, providing a seamless experience on both desktop and mobile platforms.
- Accessibility: The platform will adhere to accessibility standards (e.g., WCAG) to ensure it is usable by people with disabilities, including screen readers and assistive technologies.

- User Testing and Feedback Loop: Usability testing will be conducted with real users to gather feedback and make iterative improvements to the interface and interaction flows.

