# LLM Interfaces for Databases

Welcome to the LLM Interfaces for Databases project! This README provides instructions on how to set up and run the application using Docker.

## Prerequisites

Before running the application, please ensure you have the following:

1. **Database File**: Place the `isrecon_all.duckdb` file in the root directory of the repository.
2. **API Keys**: The application uses locally stored API Keys for LLama and Open AI. These have to be generated by the user of the application. If you would like to avoid that, please contact the team and we are happy to provide them.
3. **Docker**

## Running the Application

Follow these steps to start the application:

1. **Start Docker Daemon**
   - Make sure your Docker Daemon is running on your machine.

2. **Build the Docker Image**
   - Open your terminal and navigate to the root directory of the repository.
   - Run the following command to build the Docker image:
     ```bash
     docker build -t app .
     ```
   - This command will create a Docker image tagged as `app`.

3. **Run the Docker Container**
   - After the image is built, run the following command to start the application:
     ```bash
     docker run -p 8501:8501 -v /path/to/local/directory:/app app
     ```
   - This command will create and start a Docker container from the `app` image.
   - The 'directory' folder is where your DuckDB database must be placed.

## Additional Information

For any questions or issues, please feel free to reach out to the project maintainers.

---

Enjoy using the LLM Interfaces for Databases!
