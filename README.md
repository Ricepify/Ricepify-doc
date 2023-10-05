# Ricepify-doc
## Wireframes
**Home Page**
![HomePage](./Assest/Screenshot%20(512).png)
<br>
**LogIn**
![LogIn](./Assest/Screenshot%20(513).png)
<br>
**SignUp**
![signUp](./Assest/Screenshot%20(514).png)
<br>
**Home Page For LoggedIn Users**
![Home2](./Assest/Screenshot%20(515).png)
<br>
**About Us**
![About Us](./Assest/Screenshot%20(516).png)
<br>
**UserProfile**
![userProfile](./Assest/Screenshot%20(517).png)
<br>
**Other User Profile**
![otherUsersProfile](./Assest/Screenshot%20(518).png)
<br>
**Search**
![Search](./Assest/Screenshot%20(519).png)

## User Stories
 1. User authentication for a secure and personalized experience.
 2. Exploring a diverse collection of culinary creations sourced from trusted third party API.
 3. User Handle the recipes and interactive with it (rate, add to fav, comment).
     - Adding, updating, and deleting recipe comments.
     - Creating and managing a personal collection of favorite recipes.
4. Users sharing his own recipes with other users.
5. Recipe of the Day , Highlight a "Recipe of the Day" or "Featured Recipe" prominently on the home page
6. Search for recipes, Effortlessly searching for any recipe by ingredient, cuisine, or creator

## Software Requirements
[Software Requirements](./requirements.md)

## Domain Modeling
> Identify Entities:

- SiteUser
>> Define Attributes:
1. id
2. UserName
3. FirstName
4. LastName
5. Email
6. Password

- Recipe
- >> Define Attributes:
1. RecipeId
2. RecipeTitle
3. RecipeImage
4. RecipeDescription
5. RecipeCategory
6. RecipeArea

- RecipeInteraction
- > Define Attributes:
1. RecipeInteractionId
2. Comment
3. Rate

> Establish Relationships:
- SiteUser:

One-to-Many with Recipe: One SiteUser can have multiple recipes.
One-to-Many with RecipeInteraction: One SiteUser can have multiple recipe interactions.
- Recipe:

Many-to-One with SiteUser: Many recipes can belong to one SiteUser.
One-to-Many with RecipeInteraction: One recipe can have multiple recipe interactions.
- RecipeInteraction:

Many-to-One with Recipe: Many interactions can belong to one recipe.
Many-to-One with SiteUser: Many interactions can belong to one SiteUser.

> Create a Diagram:
![ERD](./Assest/Screenshot%202023-09-29%20204857.png)
> 



## Make an Database Schema Diagram














