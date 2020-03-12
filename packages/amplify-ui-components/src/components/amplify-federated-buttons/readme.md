# amplify-federated-buttons

<!-- Auto Generated Below -->


## Properties

| Property                | Attribute    | Description                                                                                                                    | Type                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          | Default                        |
| ----------------------- | ------------ | ------------------------------------------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------ |
| `authState`             | `auth-state` | The current authentication state.                                                                                              | `AuthState.ConfirmSignIn or AuthState.ConfirmSignUp or AuthState.CustomConfirmSignIn or AuthState.ForgotPassword or AuthState.Loading or AuthState.ResetPassword or AuthState.SettingMFA or AuthState.SignIn or AuthState.SignOut or AuthState.SignUp or AuthState.SignedIn or AuthState.SignedOut or AuthState.SigningUp or AuthState.TOTPSetup or AuthState.VerifyContact or AuthState.VerifyingAttributes or AuthState.confirmingSignInCustomFlow or AuthState.confirmingSignUpCustomFlow` | `AuthState.SignIn`             |
| `federated`             | --           | Federated credentials & configuration.                                                                                         | `FederatedConfig`                                                                                                                                                                                                                                                                                                                                                                                                                                                                             | `undefined`                    |
| `handleAuthStateChange` | --           | Passed from the Authenticator component in order to change Authentication state e.g. SignIn -> 'Create Account' link -> SignUp | `(nextAuthState: AuthState, data?: object) => void`                                                                                                                                                                                                                                                                                                                                                                                                                                           | `dispatchAuthStateChangeEvent` |


## Dependencies

### Used by

 - [amplify-federated-sign-in](../amplify-federated-sign-in)
 - [amplify-sign-in](../amplify-sign-in)

### Depends on

- [amplify-google-button](../amplify-google-button)
- [amplify-facebook-button](../amplify-facebook-button)
- [amplify-amazon-button](../amplify-amazon-button)
- [amplify-oauth-button](../amplify-oauth-button)
- [amplify-auth0-button](../amplify-auth0-button)

### Graph
```mermaid
graph TD;
  amplify-federated-buttons --> amplify-google-button
  amplify-federated-buttons --> amplify-facebook-button
  amplify-federated-buttons --> amplify-amazon-button
  amplify-federated-buttons --> amplify-oauth-button
  amplify-federated-buttons --> amplify-auth0-button
  amplify-google-button --> amplify-sign-in-button
  amplify-sign-in-button --> amplify-icon
  amplify-facebook-button --> amplify-sign-in-button
  amplify-amazon-button --> amplify-sign-in-button
  amplify-oauth-button --> amplify-sign-in-button
  amplify-auth0-button --> amplify-sign-in-button
  amplify-federated-sign-in --> amplify-federated-buttons
  amplify-sign-in --> amplify-federated-buttons
  style amplify-federated-buttons fill:#f9f,stroke:#333,stroke-width:4px
```

----------------------------------------------

*Built with [StencilJS](https://stenciljs.com/)*