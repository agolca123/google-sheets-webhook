# Google Tag Manager Webhook Integration

This project facilitates the automatic transmission of specific data from Google Tag Manager (GTM) to a designated webhook URL. This integration enables user interactions or other events to be integrated with external systems.

## Getting Started

This guide provides step-by-step information for running the project on your local machine.

### Prerequisites

- Google Tag Manager Account
- [Webhook URL](https://webhook.site/)

### Installation

1. **Create a Webhook URL:**
   - Create your webhook URL using [Google Apps Script](https://script.google.com/) or another method.
   - Back up your webhook URL and keep it for use in this project.

2. **Google Tag Manager:**
   - Log into your GTM account and create a new 'Tag.'
   - Update the created tag with the content of this project file.

3. **Data Transmission:**
   - Add the data parameters you wish to be transmitted as WebhookProperties.

## Usage

Send your interactions or other data from GTM to the specified webhook URL. By adding data parameters and values to the `webhookProperties` section, you can dynamically control what is transmitted.

For example:

```javascript
webhookProperties: [
  {column1: 'Property Name 1', column2: 'Property Value 1'}, 
  {column1: 'Property Name 2', column2: 'Property Value 2'}
]
```

### Testing

Use test codes to check the stable operation of your project.

## Troubleshooting

- **GTMOnSuccess Not Being Called:** Check the network tab and logs, and examine any CORS errors.
  
## Contributing

Feel free to send pull requests for making improvements to the project.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
