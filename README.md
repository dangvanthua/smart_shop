
# Smart Shop

Smart Shop is an e-commerce platform built with Java Spring Boot for the backend and Angular for the frontend. It supports various roles such as users, sellers, and admins, and includes features like product variants, JWT authentication, and a recommendation system.

## Features

- **User roles**: User, Admin
- **Authentication**: JWT-based authentication, Google, and Facebook login via OAuth2
- **Database**: MySQL for product and user data

## Tech Stack

- **Backend**: Java 21, Spring Boot 3.3.4
- **Frontend**: Angular
- **Database**: MySQL
- **Authentication**: JWT, OAuth2 (Google/Facebook)

## Setup

### Prerequisites

- Java 21
- Spring Boot 3.3.4
- Node.js and npm for frontend
- Cloudinary account for image uploads

### Architecture

Below is the system architecture diagram for Smart Shop:

![System Architecture](https://drive.google.com/uc?id=1F6FMY3ujxrV2JxN0G02VVEZMSXjB56xA)


### Backend Setup

1. **Clone the repository**:
   ```bash
   git clone git@github.com:dangvanthua/smart_shop.git
   ```

2. **Navigate to the backend directory**:
   ```bash
   cd smartshop-backend
   ```

3. **Build the project**:
   ```bash
   ./mvnw clean install
   ```

4. **Configure the database**: 
   Open `application.properties` or `application.yml` and add the following configuration:
   ```properties
   spring.datasource.url=jdbc:postgresql://localhost:3306/smartshop
   spring.datasource.username=your-username
   spring.datasource.password=your-password
   spring.jpa.hibernate.ddl-auto=update
   spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.MySQL5Dialect
   ```

5. **Run the backend**:
   ```bash
   ./mvnw spring-boot:run
   ```

6. **Navigate to the frontend directory and install dependencies**:
   ```bash
   cd smart-shop
   npm install
   ```

7. **Run the frontend**:
   ```bash
   ng serve
   ```

### Key Changes:
- **Database**: I updated the database description to use PostgreSQL.
- **Configuration**: Added details for configuring PostgreSQL in the `application.yml` or `application.properties` file for the backend setup section.

## Future Plans

- **Integration with Payment Gateway**: Add support for secure online payments (e.g., VNPay, PayPal).
- **Analytics Dashboard**: Provide sellers with insights into sales trends and user activity.
- **Advanced Recommendation System**: Incorporate collaborative filtering or hybrid models.
- **Mobile Application**: Develop a mobile-friendly version or dedicated mobile app.
- **Localization**: Add multi-language and multi-currency support for a global audience.
- **Improved Search Functionality**: Implement full-text search or Elasticsearch for faster, more accurate product discovery.


This should now provide all the necessary information for setting up both the backend and frontend while including PostgreSQL as the database.

## License

This project is licensed under the [Apache License 2.0](LICENSE).  
You may fork this project and use it for personal or commercial purposes. However, any changes must be proposed via Pull Request, and modifications to the original repository are not allowed without explicit permission from the owner.

## Contribution Guidelines

We welcome contributions to improve this project! However, please follow these guidelines:
1. Fork the repository.
2. Make your changes on your own fork.
3. Create a Pull Request to propose your changes to the main repository.
4. All contributions will be reviewed before being merged.

Direct modifications to the original repository are **not permitted**.
