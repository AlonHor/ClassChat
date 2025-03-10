# ClassChat

ClassChat is a terminal-based chat application that allows users to communicate within a local network. It includes both client and server components, enabling clients to join chat rooms and exchange messages in real-time.

## Features

- **Client-Server Architecture**: Establishes a connection between a client and a server for message exchange.
- **Message Broadcasting**: Broadcast messages to all connected clients.
- **Private Messaging**: Send private messages between clients using `/msg <name> <message>`.
- **User Join/Leave Notifications**: Notify all clients when a user joins or leaves the chat.
- **Spam Prevention**: Limits the number of messages a user can send in a short period to prevent spam.
- **Server Commands**: The server can execute commands like kicking, banning, and broadcasting messages.

## Usage

### Running the Server

1. Navigate to the directory containing `server.py`.
2. Run the server script:
   ```bash
   python server.py
   ```
3. Follow the prompts to set the maximum participants and the server name.

### Running the Client

1. Navigate to the directory containing `client.py`.
2. Run the client script:
   ```bash
   python client.py
   ```
3. Enter your name when prompted.
4. Choose a room to join from the discovery menu or manually enter a join code.

### Server Commands

- `kick <ip_or_name>`: Kick a client by IP or name.
- `ban <ip_or_name>`: Ban a client by IP or name.
- `unban <ip>`: Unban a client by IP.
- `say <message>`: Broadcast a message to all clients.
- `list`: List all connected clients.
- `tell <ip_or_name> <message>`: Send a private message to a client.
- `clear`: Clear the chat history.
- `exit`: Close the server and disconnect all clients.

## License

This project is licensed under the MIT License.

## Contributing

Contributions are welcome! Feel free to fork it, and please open an issue or submit a pull request for any improvements or bug fixes. This was a collaborative effort between me and [@K9Developer](https://github.com/k9developer), and we'd love to see how others can build on it!

## Acknowledgements

- [Python](https://www.python.org/)
- [keyboard](https://pypi.org/project/keyboard/)
- [pywin32](https://pypi.org/project/pywin32/)
