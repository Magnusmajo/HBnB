# Detailed Class Diagram for Business Logic Layer
The business logic layer is responsible for encapsulating the business rules and processes of the application. It is the core of the application and is responsible for managing the data and the interactions between the data and the user interface. This layer ensures that the data is processed correctly and that the business rules are enforced consistently throughout the application. It typically includes services, business objects, and other components that handle the application's core functionality.

![class_diagram](https://github.com/user-attachments/assets/2cf10951-67eb-4e23-90a9-2db50cb034a7)


The diagram shows the four key entities in the Business Logic layer: **User**, **Place**, **Review**, and **Amenity**. Each entity has its attributes, methods, and relationships with other entities.

### Entity Descriptions:

- **User**: Represents a user of the application. Attributes include first name, last name, email, password, and a boolean flag for administrator status. Methods include registering, updating the profile, loging and deleting the user.
- **Place**: Represents a place listed on the application. Attributes include title, description, price, latitude, and longitude. The place is associated with the user who created it (owner) and can have multiple amenities. Methods include creating, updating, deleting, and listing places.
- **Review**: Represents a review written by a user for a place. Attributes include rating, comment, and references to the associated place and user. Methods include creating, updating, deleting, and listing reviews by place.
- **Amenity**: Represents an amenity that can be associated with a place. Attributes include name and description. Methods include creating, updating, deleting, and listing amenities.

### Relationships:

- A user can own multiple places (one-to-many).
- A place can have multiple amenities (one-to-many).
- A review is written by a user for a place (many-to-one).
- A place can have multiple reviews (one-to-many).

--

Author: Alexis Rodriguez R.
An Holberton School Project
© 2024 Alexis-Holberton School -- All rights reserved --