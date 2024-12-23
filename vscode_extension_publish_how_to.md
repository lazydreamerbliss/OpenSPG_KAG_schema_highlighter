https://code.visualstudio.com/api/working-with-extensions/publishing-extension

1. Create access token in AzureDevops: https://azure.microsoft.com/services/devops/. Upper right corner -> User settings -> Personal access tokens -> New Token:
   - Name: any name you want for the token
   - Organization: All accessible organizations
   - Expiration (optional): set the desired expiration date for the token
   - Scopes: Custom defined:
      - click Show all scopes link below the Scopes section
      - in the Scopes list, scroll to Marketplace and select Manage scope
2. Create a marketplace publisher: https://marketplace.visualstudio.com/manage. The name of the publisher MUST be same as the one in the `publisher` field in the `package.json` file.
3. Verify the token: `vsce login <publisher-name>`
4. Publish the extension: `vsce publish`
