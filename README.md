  This project is an ASP.NET API that implements OAuth 2.0 authentication using Google .  
It allows users to log in to the system using their Google account securely. 

## Setting up Google Client ID and Client Secret  
To use this project, you need to create your own Google Client ID and Client Secret. Follow these steps:  

1. Go to the [Google Cloud Console](https://console.cloud.google.com/).  
2. Create a new project or select an existing one.  
3. Navigate to **APIs & Services** > **Credentials**.  
4. Click on **Create Credentials** and choose **OAuth 2.0 Client IDs**.  
5. Configure the consent screen and add your application details.  
6. Set the **Redirect URI** to match your API endpoint (e.g., `http://localhost:5000/api/auth/callback`).  
7. Copy the generated **Client ID** and **Client Secret**.  
8. Add them to your `appsettings.json` or as environment variables.  

Example for `appsettings.json`:  
```json
{
  "GoogleAuth": {
    "ClientId": "YOUR_GOOGLE_CLIENT_ID",
    "ClientSecret": "YOUR_GOOGLE_CLIENT_SECRET"
  }
}
