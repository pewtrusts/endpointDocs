# userDocs/macOS
## Register with Entra
### Microsoft Platform Single Sign-On (PSSOe) for Company Portal
#### Secure Enclave backed key

### Prepare your Mac for PSSOe
**Setup TouchID (MacBooks only at this time)**

- If you have not already, [follow these steps to setup TouchID on your MacBook Pro](https://support.apple.com/guide/mac-help/use-touch-id-mchl16fbf90a/15.0/mac/15.0) (Not necessary for macOS desktops at this time)

### Register your Mac with PSSOe

- After your Mac is provisioned for PSSOe, userDocs/macOS will prompt you to register using your Entra ID.  
  ![Registration Required - Use your identity provider password to log in to your Mac.](https://github.com/pewtrusts/endpointDocs/blob/main/userDocs/macOS/microsoftEntra/deviceRegistration/Images/PSSOe_SecureEnclave_1.png?raw=true)

  ![Platform Single Sign-on Registration](https://github.com/pewtrusts/endpointDocs/blob/main/userDocs/macOS/microsoftEntra/deviceRegistration/Images/PSSOe_SecureEnclave_2.png?raw=true)

- You'll be prompted for your local userDocs/macOS user account password (should match your Entra ID password).
  - This is a security step used to determine that you are present and actively using your device.
  ![Enter your password to allow this.](https://github.com/pewtrusts/endpointDocs/blob/main/userDocs/macOS/microsoftEntra/deviceRegistration/Images/PSSOe_SecureEnclave_3.png?raw=true)


- Next, you'll need to complete authentication via MFA/Microsoft Authenticator push with number challenge, Passkey enabled on another device, or security key.
  
    ![Entra MFA Prompt](https://github.com/pewtrusts/endpointDocs/blob/main/userDocs/macOS/microsoftEntra/deviceRegistration/Images/PSSOe_SecureEnclave_MFA_1.png?raw=true)

    ![Entra MFA Prompt](https://github.com/pewtrusts/endpointDocs/blob/main/userDocs/macOS/microsoftEntra/deviceRegistration/Images/PSSOe_SecureEnclave_MFA_2.png?raw=true)

- Upon completion, you'll be shown instructions to set up the device as a Passkey provider for Microsoft Entra ID. 
  ![To use your Entra ID passkey, you must enable Company Portal as a Passkey Provider.](https://github.com/pewtrusts/endpointDocs/blob/main/userDocs/macOS/microsoftEntra/deviceRegistration/Images/PSSOe_SecureEnclave_4.png?raw=true)
  - You must dismiss the dialog or open system settings and remember the path to get to the setting required: 
1. Open System Settings and go to General
    ![System Settings - General](https://github.com/pewtrusts/endpointDocs/blob/main/userDocs/macOS/microsoftEntra/deviceRegistration/Images/PSSOe_SecureEnclave_6.png?raw=true)
2. Under Password Options slide the slider to enable **Autofill passwords and Passkeys**
    ![Autofill Passwords and Passkeys](https://github.com/pewtrusts/endpointDocs/blob/main/userDocs/macOS/microsoftEntra/deviceRegistration/Images/PSSOe_SecureEnclave_7.png?raw=true)
3. Slide the slider to enable the Company Portal app
   ![Enable Company Portal](https://github.com/pewtrusts/endpointDocs/blob/main/userDocs/macOS/microsoftEntra/deviceRegistration/Images/PSSOe_SecureEnclave_8.png?raw=true)
   ![Enable Company Portal](https://github.com/pewtrusts/endpointDocs/blob/main/userDocs/macOS/microsoftEntra/deviceRegistration/Images/PSSOe_SecureEnclave_10.png?raw=true)

 
- You can confirm the state of the Secure Enclave backed key by opening System Settings > Users & Groups and selecting the “i” next to your account.  
  - Platform Single Sign-on status will show the login, method, and the state of device registration and current presence of SSO tokens for use to obtain authorization for further services gated by Entra ID.
