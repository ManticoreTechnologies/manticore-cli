# Manticore Service Manager

This script provides an easy way to manage Manticore services, including starting, stopping, installing, uninstalling, and updating them.

## Usage

Place this script in the root directory where you want to manage your services, then run it with one of the following commands:

### Commands

- `status`: Show the status of all managed services.
- `start`: Start all managed services and their daemons.
- `stop`: Stop all managed services and their daemons.
- `restart`: Restart all managed services and their daemons.
- `install`: Install services by running install scripts in each service folder.
- `uninstall`: Uninstall services, remove folders and configurations.
- `update`: Update services by pulling the latest code, reinstalling, and restarting.

### Example

To start all services:

```bash
./manticore-cli.sh start
```

To stop all services:

```bash
./manticore-cli.sh stop
```

To install the services:

```bash
./manticore-cli.sh install
```

To update the services:

```bash
./manticore-cli.sh update
```

## Configuration

Each service will have a default configuration file created if it doesn't exist. The configuration file will be located in `/usr/local/bin/` and will be named based on the service name.

## Requirements

- `git`: To clone and update the repositories.
- `systemctl`: To manage the services.
- `python3`: To run the installation scripts.

## License

This script is provided under the MIT License.
