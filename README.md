# SkHttp

SkHttp is a powerful Skript addon that provides HTTP client functionality, WebSocket support, and web server capabilities for Minecraft servers.

## Features

- **HTTP Client**: Send GET, POST, PUT, DELETE, and other HTTP requests
- **WebSocket Support**: Create WebSocket connections for real-time communication
- **Web Server**: Create HTTP endpoints and handle incoming requests
- **Discord Webhooks**: Easy integration with Discord webhooks
- **JSON Support**: Parse and manipulate JSON data
- **Async Operations**: Non-blocking HTTP operations

## Requirements

- **Minecraft**: 1.21.4+
- **Skript**: 2.11+
- **Java**: 17+

## Installation

1. Download the latest release from the [Releases](https://github.com/Rajnasasd/SkHttp/releases) page
2. Place the `SkHttp-x.x.jar` file in your server's `plugins` folder
3. Restart your server
4. The plugin will automatically check for compatibility and disable itself if requirements are not met

## Version Compatibility

This plugin automatically validates version compatibility on startup:

- **Minecraft Version**: Must be 1.21.4 or higher
- **Skript Version**: Must be 2.11.0 or higher

If your server doesn't meet these requirements, the plugin will disable itself and display an error message.

## Usage Examples

### HTTP Requests

```skript
# Simple GET request
set {_response} to http get "https://api.example.com/data"

# POST request with JSON data
set {_data} to new json object
set json "name" of {_data} to "test"
set {_response} to http post "https://api.example.com/users" with data {_data}
```

### WebSocket

```skript
# Create WebSocket connection
set {_ws} to new websocket "wss://echo.websocket.org"

# Send message
send websocket message "Hello World!" to {_ws}
```

### Web Server

```skript
# Create HTTP endpoint
create endpoint "/api/test" with method "GET":
    respond with "Hello from SkHttp!"
```

### Discord Webhooks

```skript
# Send Discord webhook
send discord webhook to "YOUR_WEBHOOK_URL" with content "Hello Discord!"
```

## Building from Source

1. Clone the repository:
   ```bash
   git clone https://github.com/Rajnasasd/SkHttp.git
   cd SkHttp
   ```

2. Build the plugin:
   ```bash
   ./gradlew shadowJar
   ```

3. The compiled JAR will be in `build/libs/SkHttp-x.x.jar`

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Support

If you encounter any issues or have questions, please open an issue on the [GitHub Issues](https://github.com/Rajnasasd/SkHttp/issues) page.

## Changelog

### Version 1.6
- Updated compatibility for Minecraft 1.21.4+
- Updated compatibility for Skript 2.11+
- Added automatic version validation
- Improved dependency management
- Fixed Discord Webhooks integration

### Previous Versions
See [CHANGELOG.md](CHANGELOG.md) for complete version history.
