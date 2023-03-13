
# Getting Started with Swagger Petstore

## Introduction

This is a sample server Petstore server.  You can find out more about Swagger at [http://swagger.io](http://swagger.io) or on [irc.freenode.net, #swagger](http://swagger.io/irc/).  For this sample, you can use the api key `special-key` to test the authorization filters.

Find out more about Swagger: [http://swagger.io](http://swagger.io)

## Building

Supported Java version is **8+**.

The generated code uses a few Maven dependencies e.g., Jackson, OkHttp,
and Apache HttpClient. The reference to these dependencies is already
added in the pom.xml file will be installed automatically. Therefore,
you will need internet access for a successful build.

* In order to open the client library in Eclipse click on `File -> Import`.

![Importing SDK into Eclipse - Step 1](https://apidocs.io/illustration/java?workspaceFolder=Swagger%20Petstore-Java&workspaceName=SwaggerPetstore&projectName=SwaggerPetstoreLib&rootNamespace=io.swagger.petstore&groupId=SwaggerPetstoreLib&artifactId=swagger-petstore-lib&version=1.0.6&step=import0)

* In the import dialog, select `Existing Java Project` and click `Next`.

![Importing SDK into Eclipse - Step 2](https://apidocs.io/illustration/java?workspaceFolder=Swagger%20Petstore-Java&workspaceName=SwaggerPetstore&projectName=SwaggerPetstoreLib&rootNamespace=io.swagger.petstore&groupId=SwaggerPetstoreLib&artifactId=swagger-petstore-lib&version=1.0.6&step=import1)

* Browse to locate the folder containing the source code. Select the detected location of the project and click `Finish`.

![Importing SDK into Eclipse - Step 3](https://apidocs.io/illustration/java?workspaceFolder=Swagger%20Petstore-Java&workspaceName=SwaggerPetstore&projectName=SwaggerPetstoreLib&rootNamespace=io.swagger.petstore&groupId=SwaggerPetstoreLib&artifactId=swagger-petstore-lib&version=1.0.6&step=import2)

* Upon successful import, the project will be automatically built by Eclipse after automatically resolving the dependencies.

![Importing SDK into Eclipse - Step 4](https://apidocs.io/illustration/java?workspaceFolder=Swagger%20Petstore-Java&workspaceName=SwaggerPetstore&projectName=SwaggerPetstoreLib&rootNamespace=io.swagger.petstore&groupId=SwaggerPetstoreLib&artifactId=swagger-petstore-lib&version=1.0.6&step=import3)

## Installation

The following section explains how to use the SwaggerPetstoreLib library in a new project.

### 1. Starting a new project

For starting a new project, click the menu command `File > New > Project`.

![Add a new project in Eclipse](https://apidocs.io/illustration/java?workspaceFolder=Swagger%20Petstore-Java&workspaceName=SwaggerPetstore&projectName=SwaggerPetstoreLib&rootNamespace=io.swagger.petstore&groupId=SwaggerPetstoreLib&artifactId=swagger-petstore-lib&version=1.0.6&step=createNewProject0)

Next, choose `Maven > Maven Project` and click `Next`.

![Create a new Maven Project - Step 1](https://apidocs.io/illustration/java?workspaceFolder=Swagger%20Petstore-Java&workspaceName=SwaggerPetstore&projectName=SwaggerPetstoreLib&rootNamespace=io.swagger.petstore&groupId=SwaggerPetstoreLib&artifactId=swagger-petstore-lib&version=1.0.6&step=createNewProject1)

Here, make sure to use the current workspace by choosing `Use default Workspace location`, as shown in the picture below and click `Next`.

![Create a new Maven Project - Step 2](https://apidocs.io/illustration/java?workspaceFolder=Swagger%20Petstore-Java&workspaceName=SwaggerPetstore&projectName=SwaggerPetstoreLib&rootNamespace=io.swagger.petstore&groupId=SwaggerPetstoreLib&artifactId=swagger-petstore-lib&version=1.0.6&step=createNewProject2)

Following this, select the *quick start* project type to create a simple project with an existing class and a `main` method. To do this, choose `maven-archetype-quickstart` item from the list and click `Next`.

![Create a new Maven Project - Step 3](https://apidocs.io/illustration/java?workspaceFolder=Swagger%20Petstore-Java&workspaceName=SwaggerPetstore&projectName=SwaggerPetstoreLib&rootNamespace=io.swagger.petstore&groupId=SwaggerPetstoreLib&artifactId=swagger-petstore-lib&version=1.0.6&step=createNewProject3)

In the last step, provide a `Group Id` and `Artifact Id` as shown in the picture below and click `Finish`.

![Create a new Maven Project - Step 4](https://apidocs.io/illustration/java?workspaceFolder=Swagger%20Petstore-Java&workspaceName=SwaggerPetstore&projectName=SwaggerPetstoreLib&rootNamespace=io.swagger.petstore&groupId=SwaggerPetstoreLib&artifactId=swagger-petstore-lib&version=1.0.6&step=createNewProject4)

### 2. Add reference of the library project

The created Maven project manages its dependencies using its `pom.xml` file. In order to add a dependency on the *SwaggerPetstoreLib* client library, double click on the `pom.xml` file in the `Package Explorer`. Opening the `pom.xml` file will render a graphical view on the canvas. Here, switch to the `Dependencies` tab and click the `Add` button as shown in the picture below.

![Adding dependency to the client library - Step 1](https://apidocs.io/illustration/java?workspaceFolder=Swagger%20Petstore-Java&workspaceName=SwaggerPetstore&projectName=SwaggerPetstoreLib&rootNamespace=io.swagger.petstore&groupId=SwaggerPetstoreLib&artifactId=swagger-petstore-lib&version=1.0.6&step=testProject0)

Clicking the `Add` button will open a dialog where you need to specify SwaggerPetstoreLib in `Group Id`, swagger-petstore-lib in `Artifact Id` and 1.0.6 in the `Version` fields. Once added click `OK`. Save the `pom.xml` file.

![Adding dependency to the client library - Step 2](https://apidocs.io/illustration/java?workspaceFolder=Swagger%20Petstore-Java&workspaceName=SwaggerPetstore&projectName=SwaggerPetstoreLib&rootNamespace=io.swagger.petstore&groupId=SwaggerPetstoreLib&artifactId=swagger-petstore-lib&version=1.0.6&step=testProject1)

![Adding sample code](https://apidocs.io/illustration/java?workspaceFolder=Swagger%20Petstore-Java&workspaceName=SwaggerPetstore&projectName=SwaggerPetstoreLib&rootNamespace=io.swagger.petstore&groupId=SwaggerPetstoreLib&artifactId=swagger-petstore-lib&version=1.0.6&step=testProject2)

### 3. Write sample code

Once the `SimpleConsoleApp` is created, a file named `App.java` will be visible in the *Package Explorer* with a `main` method. This is the entry point for the execution of the created project.
Here, you can add code to initialize the client library and instantiate a *Controller* class. Sample code to initialize the client library and using controller methods is given in the subsequent sections.

## Initialize the API Client

**_Note:_** Documentation for the client can be found [here.](doc/client.md)

The following parameters are configurable for the API Client:

| Parameter | Type | Description |
|  --- | --- | --- |
| `environment` | Environment | The API environment. <br> **Default: `Environment.PRODUCTION`** |
| `httpClientConfig` | [`ReadonlyHttpClientConfiguration`](doc/http-client-configuration.md) | Http Client Configuration instance. |
| `oAuthClientId` | `String` | OAuth 2 Client ID |
| `oAuthRedirectUri` | `String` | OAuth 2 Redirection endpoint or Callback Uri |
| `oAuthToken` | `OAuthToken` | Object for storing information about the OAuth token |
| `oAuthScopes` | `List<OAuthScopeEnum>` |  |

The API client can be initialized as follows:

```java
SwaggerPetstoreClient client = new SwaggerPetstoreClient.Builder()
    .httpClientConfig(configBuilder -> configBuilder
            .timeout(0))
    .oAuthScopes(Arrays.asList(OAuthScopeEnum.READPETS, OAuthScopeEnum.WRITEPETS))
    .implicitAuthCredentials("OAuthClientId", "OAuthRedirectUri")
    .environment(Environment.PRODUCTION)
    .build();
```

## Authorization

This API uses `OAuth 2 Implicit Grant`.

## Implicit Grant

Your application must obtain user authorization before it can execute an endpoint call incase this SDK chooses to use *OAuth 2.0 Implicit Grant* to obtain a user's consent to perform an API request on user's behalf. This authorization includes the following steps

This process requires the presence of a client-side JavaScript code on the redirect URI page to receive the *access token* after the consent step is completed.

### 1\. Obtain user consent

To obtain user's consent, you must redirect the user to the authorization page. The `buildAuthorizationUrl()` method creates the URL to the authorization page. You must have initialized the client with scopes for which you need permission to access.

```java
String authUrl = client.getImplicitAuth().buildAuthorizationUrl(); // build auth url
httpServletResponse.sendRedirect(authUrl); // show user the auth page in a browser or by redirection
```

### 2\. Handle the OAuth server response

Once the user responds to the consent request, the OAuth 2.0 server responds to your application's access request by redirecting the user to the redirect URI specified set in `Configuration`.

The redirect URI will receive the *access token* as the `token` argument in the URL fragment.

```
https://example.com/oauth/callback#token=XXXXXXXXXXXXXXXXXXXXXXXXX
```

The access token must be extracted by the client-side JavaScript code. The access token can be used to authorize any further endpoint calls by the JavaScript code.

### Scopes

Scopes enable your application to only request access to the resources it needs while enabling users to control the amount of access they grant to your application. Available scopes are defined in the `OAuthScopeEnum` enumeration.

| Scope Name | Description |
|  --- | --- |
| `READPETS` | read your pets |
| `WRITEPETS` | modify pets in your account |

## List of APIs

* [Pet](doc/controllers/pet.md)
* [Store](doc/controllers/store.md)
* [User](doc/controllers/user.md)

## Classes Documentation

* [Utility Classes](doc/utility-classes.md)
* [HttpRequest](doc/http-request.md)
* [HttpResponse](doc/http-response.md)
* [HttpStringResponse](doc/http-string-response.md)
* [HttpContext](doc/http-context.md)
* [HttpBodyRequest](doc/http-body-request.md)
* [Headers](doc/headers.md)
* [ApiException](doc/api-exception.md)
* [Configuration Interface](doc/configuration-interface.md)
* [HttpClientConfiguration](doc/http-client-configuration.md)
* [HttpClientConfiguration.Builder](doc/http-client-configuration-builder.md)

