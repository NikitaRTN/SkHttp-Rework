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
- **Java**: 21+

## Installation

1. Download the latest release from the [Releases](https://github.com/NikitaRTN/SkHttp-Rework/releases) page
2. Place the `SkHttp-x.x.jar` file in your server's `plugins` folder
3. Restart your server
4. The plugin will automatically check for compatibility and disable itself if requirements are not met

## Version Compatibility

This plugin automatically validates version compatibility on startup:

- **Minecraft Version**: Must be 1.21.4 or higher
- **Skript Version**: Must be 2.11.0 or higher

If your server doesn't meet these requirements, the plugin will disable itself and display an error message.

## Building from Source

1. Clone the repository:
   ```bash
   git clone https://github.com/NikitaRTN/SkHttp.git
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

## The source code

If you want to change the code or view its contents, go to [Code](https://github.com/NikitaRTN/SkHttp-Rework) page.

## Changelog

### Version 1.6
- Updated compatibility for Minecraft 1.21.4+
- Updated compatibility for Skript 2.11+
- Added automatic version validation
- Improved dependency management
- Fixed Discord Webhooks integration
