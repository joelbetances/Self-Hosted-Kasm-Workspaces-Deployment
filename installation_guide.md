# Installation Guide

This guide will walk you through the steps to install and configure Kasm Workspaces on your server.

## Prerequisites

- A server with a public IP address
- Basic knowledge of Linux command line
- SSH access to the server

## Steps

1. **Update your server**:
    ```bash
    sudo apt-get update
    sudo apt-get upgrade
    ```

2. **Install Docker and Docker Compose**:
    ```bash
    sudo apt-get install -y docker docker-compose
    ```

3. **Create directories for Kasm configuration**:
    ```bash
    mkdir -p ~/kasm/config
    ```

4. **Copy `kasm.conf` to the configuration directory**:
    ```bash
    cp /path/to/your/kasm.conf ~/kasm/config/kasm.conf
    ```

5. **Download and start Kasm Workspaces using Docker Compose**:
    ```bash
    cd ~/kasm
    wget https://raw.githubusercontent.com/kasmtech/workspaces/main/docker-compose.yml
    sudo docker-compose up -d
    ```

## Client Setup

1. **Access Kasm Workspaces**:
    Open a web browser and navigate to `http://your_server_ip`.

2. **Login**:
    Use the admin credentials set during the configuration to log in.
