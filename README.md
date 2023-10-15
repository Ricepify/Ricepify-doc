# Ricepify-doc
## Wireframes

[Our Wireframe on Figma](https://www.figma.com/file/3jl0Z7aqlOpdXlEETIpfwH/Ricepify-ProtoType?type=whiteboard&node-id=0-1&t=aXbvgMu1XlnpBNwV-0)
<br>
**Home Page**
![HomePage](./Assest/Screenshot%20(550).png)
<br>
**LogIn**
![LogIn](./Assest/Screenshot%20(553).png)
<br>
**SignUp**
![signUp](./Assest/Screenshot%20(552).png)
<br>
**Home Page For LoggedIn Users**
![Home2](./Assest/Screenshot%20(551).png)
<br>
**About Us**
![About Us](./Assest/Screenshot%20(554).png)
<br>
**UserProfile**
![userProfile](./Assest/Screenshot%20(556).png)
<br>
**Other User Profile**
![otherUsersProfile](./Assest/Screenshot%20(557).png)
<br>
**Saved**
![Search](./Assest/Screenshot%20(559).png)
<br>
**subsctibt**
![Search](./Assest/Screenshot%20(558).png)
<br>
**Details**
![Search](./Assest/Screenshot%20(555).png)


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
7. image
8. bio
9. followersCount
10. followingCount

- Recipe
- >> Define Attributes:
1. RecipeId
2. RecipeTitle
3. RecipeImage
4. RecipeDescription
5. RecipeCategory
6. RecipeArea
7. createdAt

- RecipeComment
- > Define Attributes:
1. id
2. Comment
- Subscrip
1. id
2. email

- InternalRecipeFavoriteEntity
1. id
2. mealId

- ExternalRecipeFavoriteEntity
1. id
2. mealId


> Establish Relationships:
SiteUserEntity:

One-to-Many with RecipeEntity: A user can have multiple recipes.
One-to-Many with RecipeComment: A user can post multiple comments.
Many-to-Many with itself: A user can follow multiple other users, and can also have multiple followers.
RecipeEntity:

Many-to-One with SiteUserEntity: A recipe belongs to one user.
One-to-Many with RecipeComment: A recipe can have multiple comments.
RecipeComment:

Many-to-One with SiteUserEntity: A comment is posted by one user.
Many-to-One with RecipeEntity: A comment is associated with one recipe.
InternalRecipeFavoriteEntity and ExternalRecipeFavoriteEntity:

Many-to-One with SiteUserEntity: A favorite recipe is associated with one user.

## Database Diagram:

![ERD](./Assest/Screenshot%20(560).png)
















