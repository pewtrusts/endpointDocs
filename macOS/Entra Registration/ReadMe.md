# Microsoft Platform Single Sign-On (PSSOe) for Company Portal
# Secure Enclave backed key

- After your Mac is provisioned for PSSOe, macOS will prompt you to register using your Entra ID.  
  

- You'll be prompted for your local macOS user account password (should match your Entra ID password).
  - This is a security step used to determine that you are present and actively using your device.





- Next, you'll need to complete authentication via MFA/Microsoft Authenticator push with number challenge, Passkey enabled on another device, or security key.  

*TWO PICS 

- Upon completion, you'll be shown instructions to set up the device as a Passkey provider for Microsoft Entra ID. 

 
- You must dismiss the dialog or open system settings and remember the path to get to the setting required: 
1. Open System Settings
2. Go to General
3. Autofill & Passwords (Enter local user password if prompted)
4. Under Password Options slide the slider to enable **Use passwords and passkeys from**
6. Slide the slider to enable the Company Portal app

 
- You can confirm the state of the Secure Enclave backed key by opening System Settings > Users & Groups and selecting the “i” next to your account.  
  - Platform Single Sign-on status will show the login, method, and the state of device registration and current presence of SSO tokens for use to obtain authorization for further services gated by Entra ID.
