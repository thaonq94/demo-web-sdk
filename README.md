# Web SIP Client

A web-based SIP (Session Initiation Protocol) client that enables real-time communication including voice calls, video calls, and instant messaging.

## Features

- **Authentication**
  - SIP account login with username, password, domain, and WebSocket server
  - Secure registration with SIP server

- **Voice Calls**
  - Make and receive voice calls
  - Call controls (answer, reject, hangup)
  - Real-time audio streaming

- **Video Calls**
  - Make and receive video calls
  - Local and remote video display
  - Video call controls

- **Instant Messaging**
  - Real-time text messaging
  - Message history display
  - Message notifications with sound alerts

## Prerequisites

- Modern web browser with WebRTC support
- SIP server with WebSocket support
- Valid SIP account credentials

## Setup

1. Clone the repository
2. Ensure all required files are present:
   - `index.html`
   - `styles.css`
   - `sip-0.20.0.js`
   - `Tingeling.mp3` (notification sound)

3. Configure your SIP server details:
   - Domain
   - WebSocket server URL
   - SIP account credentials

## Usage

1. **Login**
   - Enter your SIP credentials (username, password)
   - Enter your SIP domain
   - Enter WebSocket server URL
   - Click "Login" to register with the SIP server

2. **Making Calls**
   - Enter the target SIP address in the input field
   - Click "Gọi thoại" for voice calls
   - Click "Gọi video" for video calls

3. **Receiving Calls**
   - Incoming calls will show a notification
   - Choose to accept or reject the call
   - For video calls, both local and remote video will be displayed

4. **Messaging**
   - Enter the target SIP address
   - Type your message in the input field
   - Click "Gửi" to send
   - Messages will appear in the chat window
   - Incoming messages will play a notification sound

## Technical Details

- Built using the SIP.js library (version 0.20.0)
- Uses WebRTC for real-time media streaming
- Bootstrap 4.3.1 for UI components
- jQuery for DOM manipulation
- Font Awesome for icons

## Browser Support

- Chrome (recommended)
- Firefox
- Edge
- Safari

## Security Considerations

- Always use HTTPS in production
- Secure your WebSocket connection (WSS)
- Protect your SIP credentials
- Consider implementing additional security measures like SRTP for media encryption

## License

This project is licensed under the MIT License - see the LICENSE file for details. 
