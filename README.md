# OIDC Authentication with JavaFX and Okta
## Getting Started

To install this example, run the following commands:

```bash
git clone https://github.com/SidPeddi/Password-Authenticator.git
cd Password-Authenticator
```

### Create an Application in Okta

Log in to your Okta Developer account (or [sign up](https://developer.okta.com/signup/) if you don’t have an account).

1. From the **Applications** page, choose **Add Application**.
2. On the Create New Application page, select **Web**.
3. Give your app a memorable name (e.g., `JavaFX`), then click **Done**.

Copy your issuer (found under **API** > **Authorization Servers**), client ID, and client secret into `src/main/resources/app.properties` as follows:

```properties
oktaDomain={yourOktaDomain}
oktaClientId={yourClientId}
oktaClientSecret={yourClientSecret}
```

**NOTE:** The value of `{yourOktaDomain}` should be something like `dev-123456.okta.com`. Make sure you don't include `-admin` in the value!

After modifying this file, start the JavaFX app and you should be able to authenticate with Okta.

```
./gradlew build run
```
