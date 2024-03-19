## Prerequisites
- Docker
- Visual Studio Code with the Remote - Containers extension installed.

## Building the Docker Image

1. Clone this repository.
2. Navigate to the directory containing the Dockerfile "D:\Users\yusuf\Desktop\Develop-Standard-Developer-Environment-main\projectt".
3. Run `docker build -t project .`

## Using the Development Environment

1. Open VS Code.
2. Open the Command Palette (Ctrl+Shift+P) and select 'Remote-Containers: Open Folder in Container...'.
3. Choose the folder where this repository is cloned.
4. VS Code will start the container and open the folder inside it.

## Troubleshooting

- If you encounter any issues, ensure Docker is running and you have the necessary permissions to create and manage containers.
