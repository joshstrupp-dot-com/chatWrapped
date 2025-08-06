# Chat Wrapped

A web application that analyzes your ChatGPT conversation export to show you statistics about your usage, including time spent writing and reading, energy consumption estimates, and interesting message insights.

## What it does

Chat Wrapped takes your ChatGPT export zip file and calculates:

- **Time spent writing**: Estimated hours based on your message length (using 200 characters/minute typing rate)
- **Time spent reading**: Estimated hours based on ChatGPT's responses (using 237.5 words/minute reading rate)
- **Energy consumption**: Rough estimate of energy used (0.000010 kWh per character)
- **Comparisons**: Your energy usage equivalent to Tesla miles driven or microwave hours
- **Message insights**: Your longest and shortest messages
- **Date range**: When your conversations took place

## How to use

1. Export your ChatGPT data from your account settings
2. Wait for the email with your `.zip` file
3. Upload the zip file to this application
4. View your personalized "Chat Wrapped" statistics

## Privacy & Security

This application runs entirely in your browser using Pyodide (Python in the browser). Your data never leaves your computer - it's processed locally and only stored in your browser cache.

## Technical Details

- Built with vanilla HTML, CSS, and JavaScript
- Uses Pyodide to run Python code in the browser
- Processes ChatGPT export zip files containing `conversations.json`
- Calculates statistics using pandas for data analysis

## Live Demo

Try it out: [https://joshstrupp-dot-com.github.io/chatWrapped/](https://joshstrupp-dot-com.github.io/chatWrapped/)

## Contributing

This was largely an AI-assisted project, so please do call out any errors you find! Feel free to open issues or submit pull requests.

## License

Open source - feel free to use and modify as needed. 