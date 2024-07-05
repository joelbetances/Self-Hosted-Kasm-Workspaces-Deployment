# Troubleshooting Guide

This guide provides solutions to common issues encountered during the installation and configuration of Kasm Workspaces.

## Common Issues

### Issue: Kasm container fails to start

- **Solution**: Check the Docker logs for errors:
    ```bash
    sudo docker logs kasm
    ```

### Issue: Unable to access Kasm web interface

- **Solution**: Ensure that the server is running and port 80 is open. Check the Kasm container logs for any errors.

### Issue: Notifications not being sent

- **Solution**: Verify the email settings in the configuration file and ensure that the email server is reachable.
