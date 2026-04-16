
# How to Add Custom Models in VS Code Insider

### Instructions

1. **Install VS Code Insider**
- Download and install VS Code Insider from the official Microsoft repository
- Link: https://code.visualstudio.com/insiders

2. **Access Apollo AI**
- Go to the Apollo AI platform and login your account.
- Link: https://dev-ai.apollotech.co/
- Click on your user profile
- Select 'Settings' > Go to 'Account'
- Copy the API keys from your account settings

3. **Configure Model in VS Code**
- Once VS Code Insider is installed, open the chat panel on the right side
- Click on 'Model' > 'Other Model' > 'Manage Model'
- In the Language Models section, click 'Add Model' and select 'OpenAI Compatible'
- Press 'Enter' on your keyboard and paste the API keys you copied earlier

4. **Update Configuration File**
- Paste the following configuration in the chatLanguageModels.js file:
- Get the model IDs from: https://dev-ai.apollotech.co/api/models

``` json
    "models": [
        {
            "id": "saricles/Qwen3-Coder-Next-NVFP4-GB10",
            "name": "Apollo AI (Qwen3 Coder Next)",
            "url": "https://dev-ai.apollotech.co/api",
            "toolCalling": true,
            "vision": false,
            "maxInputTokens": 128000,
            "maxOutputTokens": 120000
        }
    ]
``` 

## Notes
- Ensure you have the correct API keys from your Apollo AI account
- The model configuration should be compatible with OpenAI's API format
- Check the official Apollo AI documentation for any updates to the configuration format

## References
- Apollo AI Platform: https://dev-ai.apollotech.co/
- API Models List: https://dev-ai.apollotech.co/api/models
