### invoice-generator description
This project, **invoice-generator**, is a Node.js app for easy invoice generation. Built with Express.js, it includes user authentication, product management, and quotation generation. Structured for maintainability and scalability, it leverages modern web development practices to provide a robust invoicing solution.
### Invoice Generator

This is a full-stack web application built using Node.js, Express.js,and MongoDB. The application allows users to create and download invoices in PDF format.

## Tech Stack

- **NodeJS**
- **ExpressJS**
- **MongoDB**
- **Puppeteer** (for PDF generation)
- **Postman** (for API testing)

## Prerequisites

- Node.js and npm installed
- MongoDB installed and running
- Docker (optional, for containerization)

## Getting Started

### Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/yourusername/invoice-generator.git
    cd invoice-generator
    ```

2. Install dependencies:
    ```sh
    npm install
    ```

3. Create a `.env` file based on the `.env.example`:
    ```sh
    cp .env.example .env
    ```

4. Configure your MongoDB connection string in the `.env` file:
    ```
    MONGO_URI=mongodb://localhost:27017/invoice-generator
    JWT_SECRET=your_jwt_secret
    ```

### Running the Application

1. Start the application:
    ```sh
    npm run start
    ```

2. The application will be running at `http://localhost:3000`.

### API Documentation

The API documentation is available via Swagger. Once the application is running, you can access it at `http://localhost:3000/api`.

### Testing the API with Postman

A Postman collection is included in the repository. Import the `Invoice Generator.postman_collection.json` file into Postman to test the APIs.

### Docker

To run the application in a Docker container:

1. Build the Docker image:
    ```sh
    docker build -t invoice-generator .
    ```

2. Run the Docker container:
    ```sh
    docker run -p 3000:3000 invoice-generator
    ```

### Features

- User authentication with JWT
- Create and manage products
- Generate and download invoices in PDF format
- View generated quotations

### Optional Features

- Generate images of invoices
- Implement CI/CD pipeline for automatic deployment

## License

This project is licensed under the MIT License - see the LICENSE file for details.
