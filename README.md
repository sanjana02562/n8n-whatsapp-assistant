# n8n WhatsApp-Driven Google Drive Assistant

This project is a workflow automation using n8n, which:
- Receives WhatsApp messages using Twilio.
- Parses user inputs like name or file.
- Uploads any media sent via WhatsApp to Google Drive automatically.

## Tools Used
- n8n
- Twilio (for WhatsApp)
- Google Drive API (OAuth2)
- ngrok (for webhook tunneling)
- Docker

## How to Use
1. Run `docker-compose up` to start n8n locally.
2. Setup your Twilio WhatsApp number with the webhook URL from n8n (via ngrok).
3. Authenticate Google Drive from within the n8n node.
4. Test by sending a message to your Twilio number.

## Workflow File
See `whatsapp-assistant-workflow.json`.

## Notes
- This project was created as part of an internship assignment.
