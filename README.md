[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](/LICENSE)
[![Twitter: elbruno](https://img.shields.io/twitter/follow/elbruno.svg?style=social)](https://twitter.com/elbruno)
![GitHub: elbruno](https://img.shields.io/github/followers/elbruno?style=social)

## Description

**AltTextImageGeneratorWinForm** is a Windows Forms application designed to generate alt text descriptions for images. This tool is particularly useful for creating image descriptions for applications like X/Twitter, BlueSky, PowerPoint, and other platforms where alt text is needed to improve accessibility. 

The application processes an image file, generates a descriptive alt text, and saves it to a text file. Additionally, it copies the generated alt text to the clipboard for easy pasting.

## Requirements

- [.NET 9.0 SDK](https://dotnet.microsoft.com/download/dotnet/9.0) or later
- [Ollama](https://ollama.com/) installed locally
- [Llama3.2-vision model](https://ollama.com/library/llama3.2-vision) downloaded and configured in Ollama

### Installing .NET 9.0 SDK

You can download and install the .NET 9.0 SDK from the official [.NET website](https://dotnet.microsoft.com/download/dotnet/9.0).

### Installing Ollama

To install Ollama, follow the instructions provided on the [Ollama website](https://ollama.com/).

### Downloading the Llama3.2-vision Model

After installing Ollama, download the [Llama3.2-vision model](https://ollama.com/library/llama3.2-vision) by following the instructions on the Ollama website or using the Ollama CLI.

## Detailed Description of the Functionality

The main functionality of the AltTextImageGeneratorWinForm application is implemented in the `Program.cs` file. Below is a detailed description of its key components:

1. **Main Entry Point**:
   - The `Main` method initializes the application with high DPI mode, visual styles, and compatible text rendering.
   - It checks for command-line arguments to determine the image file location or display help information.
   - If a valid image file location is provided, it generates the alt text for the image, saves it to a text file, and copies the alt text to the clipboard.

2. **ShowHelp Method**:
   - Displays usage information and options for the application.

3. **GenerateAltTextForImageAsync Method**:
   - Uses the OllamaChatClient to communicate with the Llama3.2-vision model.
   - Sends the image file to the model and requests an alt text description.
   - Returns the generated alt text.

4. **GetMediaType Method**:
   - Determines the media type of the image based on its file extension.
   - Supports JPEG, PNG, and GIF formats.

### Example Usage

To use the application, run the following command in the terminal:


## Resources

- [Deploy a .NET Aspire project to Azure Container Apps using the Azure Developer CLI (in-depth guide)](https://learn.microsoft.com/dotnet/aspire/deployment/azure/aca-deployment-azd-in-depth)

- [Aspiring .NET Applications with Azure OpenAI](https://learn.microsoft.com/shows/azure-developers-dotnet-aspire-day-2024/aspiring-dotnet-applications-with-azure-openai)

### Video Recordings

[![Run eShopLite Semantic Search in Minutes with .NET Aspire & GitHub Codespaces 🚀](./images/90ytrunfromcodespaces.png)](https://youtu.be/T9HwjVIDPAE)