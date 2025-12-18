# Client-Onboarding-System-using-n8n

Automated client onboarding system with n8n: form intake, Airtable integration, private client channels, and invoice automation.

## Description
A simple Client Onboarding System designed to automate the entire onboarding process for agencies. This system helps streamline client communication, document transfers, project tracking, and invoicing.

- **Automatic Client Onboarding:** When a client fills out the typeform, their details are automatically added to Airtable.  
- **Private Client Channels:** The system generates a private channel for each client to manage communication and project updates.  
- **Invoice Management:** When a project is completed, an invoice is generated and sent to the client. Once payment is confirmed, the project is automatically marked as completed.  

## Features
- Seamless integration with Airtable for client data management  
- Private client channels for organized communication  
- Automatic invoice generation and payment tracking  
- Fully automated workflow using n8n  

## Tech Stack
- **n8n** – Automation workflows  
- **Airtable** – Client data storage and management  
- **Typeform** – Client input forms
- **Slack** – For client's private channel

## Setup: API Keys & Credentials

Before running the workflow, you'll need to get the following API keys:

- **Typeform API Key**  
  - Available from your [Typeform account](https://www.typeform.com/account/settings) after you create an Account.  
  - Copy it to the n8n credentials section.

- **Airtable API Key**  
  - Obtain from your [Airtable account](https://airtable.com/account).  
  - Add your base ID and table names in n8n.  
  - For a detailed walkthrough, check this YouTube Video: https://youtu.be/64HO3Dlr5T8?si=vLReDu5Mha-nU7Q5

- **Gmail / Google Workspace API Key**  
  - Get credentials from [Google Cloud Console](https://console.cloud.google.com/apis/credentials).  
  - Create OAuth 2.0 client ID and enable Gmail API.  
  - Paste credentials into n8n Gmail node.

- **Slack API Key**  
  - Create a Slack App and Bot via [Slack API](https://api.slack.com/apps).  
  - Give the bot the required permissions (chat:write, channels:manage, etc.).  
  - Copy the Bot Token into the n8n Slack node.  
  - For a visual guide, see this YouTube tutorial:https://www.youtube.com/watch?v=qk5JH6ImK0I

- **Gemini AI API Key**  
  - Get it from your [Gemini AI Studio account](https://gemini.ai/studio).  
  - Paste the key in n8n credentials to use AI functions.

## Running the Workflow

1. **Sign up for n8n**  
   - Create a free account at [n8n.io](https://n8n.io/).

2. **Import the workflow JSON**  
   - Download all workflow `.json` files from this repo.  
   - In your n8n dashboard, go to **Workflow → Import** and paste/upload the JSON files.

3. **Connect credentials**  
   - Make sure all API keys (Typeform, Airtable, Gmail, Slack, Gemini AI) are added in the n8n credentials section.  
   - Without these, the workflow won’t run.

4. **Activate the workflow**  
   - Toggle the workflow **ON** to start automated client onboarding.  
   - Test it by submitting a sample Typeform entry to see the automation in action.
