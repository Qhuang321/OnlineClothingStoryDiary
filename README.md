[## Design Document](https://mail-team-8anht7w3pbww.atlassian.net/jira/software/projects/PP/boards/2/timeline?selectedIssue=PP-2)
Qinghua Huang

# Introduction

Are you tired of hopping from one store to another in search of the perfect outfit? Look no further! Our team is excited to introduce an innovative solution that will revolutionize your shopping experience. The Online Clothing Shopping App is your one-stop destination for all your fashion needs. With a user-friendly interface and a wide range of clothing options, we aim to provide convenience and style at your fingertips.
Browse and Purchase: Explore a vast selection of clothing items from the comfort of your home. From trendy apparel to timeless classics, find the perfect pieces to elevate your wardrobe.

- Personalized Recommendations: Receive tailored recommendations based on your preferences, previous purchases, and browsing history. Discover new styles that match your unique taste effortlessly.

- Virtual Try-On: Visualize how clothing items will look on you with virtual try-on technology. Simply upload a photo or use your device's camera to see how different garments fit before making a purchase.

- Size Guides and Fit Assistance: Access comprehensive size guides and fit assistance to ensure you choose the right size every time. Say goodbye to ill-fitting clothes with our helpful sizing tools.

- Secure Checkout: Enjoy peace of mind with our secure checkout process. Safely purchase your favorite items with various payment options and encrypted transactions.

- Order Tracking: Stay informed about the status of your orders with real-time tracking. Know exactly when your items will arrive, so you can plan accordingly.

- Customer Support: Receive prompt assistance from our dedicated customer support team. Whether you have questions about products, orders, or returns, we're here to help you every step of the way.

- Exclusive Deals and Promotions: Take advantage of exclusive deals, discounts, and promotions available only to app users. Save money while upgrading your wardrobe with the latest fashion trends.

Experience the convenience of online shopping with the Online Clothing Shopping App. Download now and embark on a seamless shopping journey tailored to your needs and preferences.
# Storyboard

Clothing Online Storyboard


# Functional Requirements

***Requirement 100.0: Search for Clothing Items***

 **Scenario**

As a user in need of specific clothing items, I want to be able to search for clothes based on any part of the name, brand, category, or color, so that I can quickly find what I'm looking for.

 **Dependencies**

Clothing database is available and accessible.

 **Assumptions**

Clothing names, brands, and categories are accurately represented in the database.

**Examples**

1.1

**Given** a database of clothing items is available

**When** I search for "Blue Jeans"

**Then** I should receive at least one result with the following attributes:

Brand: Levi's

Category: Jeans

Color: Blue

1.2

**Given** a database of clothing items is available

**When** I search for "Nike"

**Then** I should receive at least one result with the following attributes:

Brand: Nike

Category: Athletic Wear

And I should receive multiple results with similar attributes for different Nike products.

1.3

**Given** a database of clothing items is available

**When** I search for "xyz123"

**Then** I should receive zero results (an empty list)

***Requirement 101: Save Favorite Clothing Items***

**Scenario**

As a user, I want to be able to save details of my favorite clothing items, including images and descriptions, so that I can easily access them later.

**Dependencies**

Clothing database is available and accessible.

The app has access to the device's camera.

**Assumptions**

Clothing details are accurately represented in the database.

**Examples**

1.1

**Given** a database of clothing items is available

**Given** camera access is granted

**When** I select the clothing item "Black Dress"

Take a photo of the dress and add a description "Perfect for formal occasions"

**Then** when I navigate to my favorites, I should see the "Black Dress" with the added photo and description.

2.1

**Given** a database of clothing items is available

**Given** camera access is granted

**When** I select the clothing item "Adidas Sneakers"

Take a photo of the sneakers and add a description "Great for running"

**Then** when I navigate to my favorites, I should see the "Adidas Sneakers" with the added photo and description.

# Class Diagram

**Class Diagram Description**

Main Activity: The main screen of the app displaying a list of clothing items and options to search and filter.

Clothing Details Activity: A screen that shows detailed information about a selected clothing item.

Retrofit Instance: Bootstrap class required for Retrofit.

# Project Management

This project utilizes GitHub, Jira SAAS, and Confluence for project management and collaboration.

Clothing: Noun class representing a clothing item.

Favorite: Noun class representing a user's favorite clothing item.

IClothingDAO: Interface for Retrofit to find and parse clothing JSON.

IFavoriteDAO: Interface for Room to persist favorite clothing data.

# Scrum Roles

DevOps/Product Owner/Scrum Master: [Qinghua]

Frontend Developer: [Sam]

Backend Developer: [Someone]

# Project Management Information System

We have a dedicated team consisting of experienced developers, code reviewers, a scrum master, and product owners committed to the success of this project.



 
