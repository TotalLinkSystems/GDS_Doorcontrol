# GDS_Doorcontrol
🚀 Getting Started

This guide will help you get the GDS DoorControl system up and running using Docker.
🛠️ Prerequisites

Ensure that Docker and Docker Compose are installed on your machine:

    Windows/Mac:
    Install Docker Desktop

    Linux:
    Follow your distribution’s instructions to install Docker and Docker Compose.
    For example, on Ubuntu:

    sudo apt update
    sudo apt install docker.io docker-compose

📦 Installation

    Download the docker-compose.yml file from this repository:
    https://github.com/TotalLinkSystems/GDS_Doorcontrol

    (Optional): Adjust ports in the docker-compose.yml file if needed.

        For example, you may change 8080:8080 to 8081:8080 on the backend.

        Be sure to only change the host-side port (left side of the :).

        Do not change internal container ports unless you also update related environment variables.

    Run the system:

docker-compose up -d

Wait for the containers to finish starting up. You can check the status with:

    docker ps

🌐 Accessing the App

Once the containers are running:

    Open your web browser.

    Go to:
    http://<host-ip>:<frontend-port>
    Example: http://192.168.1.100:80

        ⚠️ Replace <host-ip> with the IP address of the machine running Docker.

    You will be greeted with the login screen.

        Username: admin

        Password: 12345678

    Change the default password immediately:

        Use the side menu to navigate to Admin User

        Change the password and (Optionally) username

🧩 Adding Devices and Users

Once logged in and the password is changed:

    Navigate to Readers to add Grandstream GDS37xx door readers

    Navigate to Users to create and manage door access users

    Navigate to Logs to search logs by door or user
