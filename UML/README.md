# HBnB project
# Author: Alexis Rodríguez R.
# Date: September, 2024

# Description: High-Level Package Diagram
![Package_Diagram](https://github.com/user-attachments/assets/6999f96d-feec-4fb9-8888-dcd5c6354125)

This diagram represents a layered application architecture, which organizes the code into different layers, each with specific responsibilities. Let’s break it down layer by layer:

## Explanation:

### Presentation Layer:
- **User Interface**: It handles the user interactions.
- **API Controllers**: It exposes endpoints for the application functionalities.

### Business Layer:
- **Facade Pattern**: Provides a simplified interface to the complex subsystem in the business logic layer, making it easier for the presentation layer to interact with the business logic.
- **Business Workflow**: Manages business processes and rules that need to be followed.
- **Business Components**: Contains the specific logic for each part of the business.
- **Business Entities**: Represents business data and objects, such as User Service, Place Service, Review Service, Amenity Service, etc.

### Persistence Layer
This layer handles interaction with data sources and is divided into:
- **Data Storage**: It stores the information handled by the entities.
- **Service**: Facilitates communication with other data services.
