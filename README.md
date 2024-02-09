# Key Vault Configuration Demo with .NET

## Description

This project demonstrates how to use Azure Key Vault to store and retrieve secrets in a .NET application. The secrets are stored in the Key Vault and accessed by the .NET application using the `Azure.Identity` library. The secrets are then used in the application.

This is demonstrated in a detailed YouTube video, go check it out

[![Secure your .NET application with Azure Key Vault](https://img.youtube.com/vi/Mi6ups54bSU/0.jpg)](https://youtu.be/Mi6ups54bSU)

Also check out the Blog post: [Secure On-Premise .NET Application with Azure Key Vault](https://mdbouk.com/secure-on-premise-net-application-with-azure-key-vault/)

## Project Structure

- `KeyVaultYouTubeDemo/`: Contains the .NET application that uses Azure Key Vault to store and retrieve secrets.
- `KeyVaultYouTubeDemo/KeyVaultExtensions.cs`: Contains the extension method to add Key Vault configuration to the `IConfigurationBuilder`.
- `KeyVaultYouTubeDemo/Program.cs`: Contains the main entry point of the application.

## How to Use

1. Create a new Azure Key Vault in the Azure Portal
2. Add a new secret to the Key Vault
3. To use it with Client Secret Credentials: Create Azure AD App Registration and grant it access to the Key Vault
   1. Create a new Azure AD App Registration
   2. Grant the App Registration access to the Key Vault
   3. Create a new Client Secret for the App Registration
   4. Update the `appsettings.json` file with the Tenant ID, Client ID, and Client Secret
4. To use it with Managed Identity: Grant the Managed Identity access to the Key Vault
   1. Grant the Managed Identity access to the Key Vault
   2. Update the `appsettings.json` file with the Key Vault name
5. Run the application

## Note

### Update 1: Using Managed Identity

Note that I have updated the application to use Managed Identity to access the Key Vault. This is demonstrated in the YouTube video.

### Update 2: Using Client Secret Credentials

Another change was to use Client Secret Credentials to access the Key Vault. This is demonstrated in the Blog post: [Secure On-Premise .NET Application with Azure Key Vault](https://www.mdbouk.com//)

If you have any more comment, please do share them in the comment section of the YouTube video.

## License

This project is licensed under the terms of the [LICENSE](LICENSE) file.
