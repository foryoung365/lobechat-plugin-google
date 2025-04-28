# LobeChat Google Custom Search Plugin

A LobeChat search plugin that uses the [Google Custom Search API](https://developers.google.com/custom-search).

## Setup Steps

1. Create a Google Custom Search Engine
   - Visit [Google Programmable Search Engine](https://programmablesearch.google.com/create)
   - Create a custom search engine
   - Get your search engine ID (cx parameter)

2. Get Google API Key
   - Visit [Google Cloud Console](https://console.cloud.google.com/)
   - Create a project
   - Enable "Custom Search API"
   - Create an API key (key parameter)

3. Configure the Plugin in LobeChat
   - Add this plugin to LobeChat
   - Provide your API key and search engine ID in the configuration page
   - These credentials will be automatically added to each request as secure parameters

## Authentication Method

This plugin uses the following two secure parameters:
- `key`: Your Google API key
- `cx`: Your custom search engine ID

These two parameters are added as query parameters to the API request.

## Limitations

- Google Custom Search API free version is limited to 100 queries per day
- Paid version provides more quota

## Privacy

- Your search queries will be sent to Google
- This plugin does not collect or store your personal data

`(Not affiliated with any of the above entities)` 