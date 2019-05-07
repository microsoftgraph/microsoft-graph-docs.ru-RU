---
title: Выбор поставщика проверки подлинности Microsoft Graph
description: Сведения о том, как выбрать поставщиков проверки подлинности для конкретного сценария для вашего приложения.
localization_priority: Normal
author: MichaelMainer
ms.openlocfilehash: 5061b38249f31a6eea959ecec94899337bf57326
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33630197"
---
# <a name="choose-a-microsoft-graph-authentication-provider-based-on-oauth-flow"></a>Выбор поставщика проверки подлинности Microsoft Graph на основе процесса OAuth

Поставщики проверки подлинности упрощают извлечение маркера доступа путем абстракции параметров, необходимых для клиентских библиотек проверки подлинности. Поставщики проверки подлинности Microsoft Graph упрощают использование библиотеки проверки подлинности Microsoft (MSAL), предоставляя адаптеры для каждой платформы. Эти адаптеры обрабатывают получение маркера для вашего приложения. Поставщики проверки подлинности Microsoft Graph сопоставляются с процессом предоставления OAuth. Необходимо знать, какой способ предоставления OAuth используется для вашего приложения, чтобы выбрать соответствующий поставщик проверки подлинности для вашего приложения.

## <a name="authorization-code-oauth-flow"></a>Потоки кода авторизации OAuth

Потоки кода авторизации позволяют встроенным и веб-приложениям безопасно получать маркеры в имени пользователя. Для получения дополнительных сведений см [код кода авторизации платформы Microsoft Identity и OAuth 2,0](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-auth-code-flow).

# <a name="ctabcs"></a>[Языках](#tab/CS)

```csharp
IConfidentialClientApplication clientApplication = AuthorizationCodeProvider.CreateClientApplication(clientId, redirectUri, clientCredential);
AuthorizationCodeProvider authProvider = new AuthorizationCodeProvider(clientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[Язык](#tab/Javascript)

В настоящее время код авторизации, учетные данные клиента и потоки OAuth "от имени" требуют реализации настраиваемого поставщика проверки подлинности. Дополнительные сведения см. в разделе [Использование настраиваемого поставщика проверки](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md)подлинности.

# <a name="javatabjava"></a>[Java](#tab/Java)

```java
AuthorizationCodeProvider authProvider = new AuthorizationCodeProvider(
                                                    clientId,
                                                    scopes,
                                                    authorizationCode,
                                                    redirectUri,
                                                    clientSecret);
```

# <a name="androidtabandroid"></a>[Android](#tab/Android)

Неприменимо.

# <a name="objective-ctabobjective-c"></a>[Цель — C](#tab/Objective-C)

Неприменимо.

# <a name="phptabphp"></a>[PHP](#tab/PHP)

Пока недоступно. Поддержка или открытие [запроса функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) , если это важно.

# <a name="rubytabruby"></a>[Ruby](#tab/Ruby)

Пока недоступно. Если это важно, проведите голосование или откройте [запрос функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) .

---

## <a name="client-credential-oauth-flow"></a>Потоки учетных данных клиента OAuth

Поток учетных данных клиента позволяет приложениям службы работать без взаимодействия с пользователем. Доступ зависит от удостоверения приложения. Дополнительные сведения см. [в статье платформа идентификации Майкрософт и процесс учетных данных клиента OAuth 2,0](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow).

# <a name="ctabcs"></a>[Языках](#tab/CS)

```csharp
IConfidentialClientApplication clientApplication = ClientCredentialProvider.CreateClientApplication(clientId, clientCredential);
ClientCredentialProvider authProvider = new ClientCredentialProvider(clientApplication);
```

# <a name="javascripttabjavascript"></a>[Язык](#tab/Javascript)

В настоящее время код авторизации, учетные данные клиента и потоки OAuth "от имени" требуют реализации настраиваемого поставщика проверки подлинности. Дополнительные сведения см. в разделе [Использование настраиваемого поставщика проверки](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md)подлинности.

# <a name="javatabjava"></a>[Java](#tab/Java)

```java
ClientCredentialProvider authProvider = new ClientCredentialProvider(
                                                    clientId,
                                                    scopes,
                                                    clientSecret,
                                                    tenant,
                                                    endpoint);
```

# <a name="androidtabandroid"></a>[Android](#tab/Android)

Неприменимо.

# <a name="objective-ctabobjective-c"></a>[Цель — C](#tab/Objective-C)

Неприменимо.

# <a name="phptabphp"></a>[PHP](#tab/PHP)

Пока недоступно. Поддержка или открытие [запроса функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) , если это важно.

# <a name="rubytabruby"></a>[Ruby](#tab/Ruby)

Пока недоступно. Поддержка или открытие [запроса функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) , если это важно.

---

## <a name="on-behalf-of-oauth-flow"></a>Последовательность OAuth "от имени"

Потоки "от имени" применяются, когда приложение вызывает службу или веб-API, которые в своюмся вызывает API Microsoft Graph. Узнайте больше, прочитав [платформу Microsoft Identity и OAuth 2,0 от имени по поручению](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow)

# <a name="ctabcs"></a>[Языках](#tab/CS)

```csharp
IConfidentialClientApplication clientApplication = OnBehalfOfProvider.CreateClientApplication(clientId, redirectUri, clientCredential);
OnBehalfOfProvider authProvider = new OnBehalfOfProvider(clientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[Язык](#tab/Javascript)

В настоящее время код авторизации, учетные данные клиента и потоки OAuth "от имени" требуют реализации настраиваемого поставщика проверки подлинности. Для получения дополнительных сведений ознакомьтесь [с использованием настраиваемого поставщика проверки](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md) подлинности.

# <a name="javatabjava"></a>[Java](#tab/Java)

Пока недоступно. Если это важно, проведите голосование или откройте [запрос функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) .

# <a name="androidtabandroid"></a>[Android](#tab/Android)

Неприменимо.

# <a name="objective-ctabobjective-c"></a>[Цель — C](#tab/Objective-C)

Неприменимо.

# <a name="phptabphp"></a>[PHP](#tab/PHP)

Пока недоступно. Если это важно, проведите голосование или откройте [запрос функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) .

# <a name="rubytabruby"></a>[Ruby](#tab/Ruby)

Пока недоступно. Если это важно, проведите голосование или откройте [запрос функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) .

---

## <a name="implicit-grant-oauth-flow"></a>Неявный поток предоставления OAuth

Неявный поток предоставления используется в приложениях, основанных на браузерах. Для получения дополнительных сведений см [Microsoft Identity Platform и неявный поток предоставления разрешений](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-implicit-grant-flow).

# <a name="ctabcs"></a>[Языках](#tab/CS)

Неприменимо.

# <a name="javascripttabjavascript"></a>[Язык](#tab/Javascript)

```javascript
const clientId = "your_client_id"; // Client Id of the registered application
const callback = (errorDesc, token, error, tokenType) => {};
// An Optional options for initializing the MSAL @see https://github.com/AzureAD/microsoft-authentication-library-for-js/wiki/MSAL-basics#configuration-options
const options = {
    redirectUri: "Your redirect URI",
};
const graphScopes = ["user.read", "mail.send"]; // An array of graph scopes

// Initialize the MSAL @see https://github.com/AzureAD/microsoft-authentication-library-for-js/wiki/MSAL-basics#initialization-of-msal
const userAgentApplication = new Msal.UserAgentApplication(clientId, undefined, callback, options);
const authProvider = new MicrosoftGraph.MSALAuthenticationProvider(userAgentApplication, graphScopes);

const options = {
    authProvider, // An instance created from previous step
};
const Client = MicrosoftGraph.Client;
const client = Client.initWithMiddleware(options);
```

# <a name="javatabjava"></a>[Java](#tab/Java)

Неприменимо.

# <a name="androidtabandroid"></a>[Android](#tab/Android)

Неприменимо.

# <a name="objective-ctabobjective-c"></a>[Цель — C](#tab/Objective-C)

Неприменимо.

# <a name="phptabphp"></a>[PHP](#tab/PHP)

Неприменимо.

# <a name="rubytabruby"></a>[Ruby](#tab/Ruby)

Неприменимо.

---

## <a name="device-code-oauth-flow"></a>Процесс обработки OAuth кода устройства

Потоки кода устройства позволяют выполнять вход на устройства с помощью другого устройства. Дополнительные сведения см. [в статье платформа идентификации Майкрософт и код устройства OAuth 2,0](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-device-code).

# <a name="ctabcs"></a>[Языках](#tab/CS)

```csharp
IPublicClientApplication clientApplication = DeviceCodeProvider.CreateClientApplication(clientId);
DeviceCodeProvider authProvider = new DeviceCodeProvider(clientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[Язык](#tab/Javascript)

Пока недоступно. Если это важно, проведите голосование или откройте [запрос функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) .

# <a name="javatabjava"></a>[Java](#tab/Java)

Пока недоступно. Поддержка или открытие [запроса функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) , если это важно.

# <a name="androidtabandroid"></a>[Android](#tab/Android)

Неприменимо.

# <a name="objective-ctabobjective-c"></a>[Цель — C](#tab/Objective-C)

Неприменимо.

# <a name="phptabphp"></a>[PHP](#tab/PHP)

Пока недоступно. Если это важно, проведите голосование или откройте [запрос функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) .

# <a name="rubytabruby"></a>[Ruby](#tab/Ruby)

Пока недоступно. Если это важно, проведите голосование или откройте [запрос функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) .

---

## <a name="integrated-windows-flow"></a>Встроенный Windows Flow

Интегрированный поток Windows предоставляет компьютеру Windows способ получить маркер доступа без уведомления при присоединении к домену. Подробнее: встроенная [Проверка подлинности Windows](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Integrated-Windows-Authentication).

# <a name="ctabcs"></a>[Языках](#tab/CS)

```csharp
IPublicClientApplication clientApplication = IntegratedWindowsAuthenticationProvider.CreateClientApplication(clientId);
IntegratedWindowsAuthenticationProvider authProvider = new IntegratedWindowsAuthenticationProvider(clientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[Язык](#tab/Javascript)

Неприменимо.

# <a name="javatabjava"></a>[Java](#tab/Java)

Неприменимо.

# <a name="androidtabandroid"></a>[Android](#tab/Android)

Неприменимо.

# <a name="objective-ctabobjective-c"></a>[Цель — C](#tab/Objective-C)

Неприменимо.

# <a name="phptabphp"></a>[PHP](#tab/PHP)

Неприменимо.

# <a name="rubytabruby"></a>[Ruby](#tab/Ruby)

Неприменимо.

---

## <a name="interactive-flow"></a>Интерактивный процесс

Интерактивный обмен используется приложениями для мобильных устройств (Xamarin и UWP) и приложениями для настольных ПК, чтобы вызывать Microsoft Graph в имени пользователя. Дополнительные сведения см в разделе [получение маркеров в интерактивном режиме](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Acquiring-tokens-interactively).

# <a name="ctabcs"></a>[Языках](#tab/CS)

```csharp
IPublicClientApplication clientApplication = InteractiveAuthenticationProvider.CreateClientApplication(clientId);
InteractiveAuthenticationProvider authProvider = new InteractiveAuthenticationProvider(clientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[Язык](#tab/Javascript)

Пока недоступно. Если это важно, проведите голосование или откройте [запрос функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) .

# <a name="javatabjava"></a>[Java](#tab/Java)

Пока недоступно. Если это важно, проведите голосование или откройте [запрос функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) .

# <a name="androidtabandroid"></a>[Android](#tab/Android)

```java
PublicClientApplication publicClientApplication = new PublicClientApplication(getApplicationContext(), "CLIENT_ID_OF_YOUR_APPLICATION");
MSALAuthenticationProvider msalAuthenticationProvider = new MSALAuthenticationProvider(
    getActivity(),
    getApplication(),
    publicClientApplication,
    scopes);

IGraphServiceClient graphClient =
  GraphServiceClient
    .builder()
    .authenticationProvider(msalAuthenticationProvider)
    .buildClient();
```

# <a name="objective-ctabobjective-c"></a>[Цель — C](#tab/Objective-C)

```objc
NSError *error = nil;
MSALPublicClientApplication *publicClientApplication = [[MSALPublicClientApplication alloc] initWithClientId:@"INSERT-CLIENT-APP-ID" 
error:&error];

MSALAuthenticationProviderOptions *authProviderOptions= [[MSALAuthenticationProviderOptions alloc] initWithScopes:<array-of-scopes-for-which-you-need-access-token>];

 MSALAuthenticationProvider *authenticationProvider = [[MSALAuthenticationProvider alloc] initWithPublicClientApplication:publicClientApplication 
 andOptions:authProviderOptions];
```

# <a name="phptabphp"></a>[PHP](#tab/PHP)

Неприменимо.

# <a name="rubytabruby"></a>[Ruby](#tab/Ruby)

Неприменимо.

---

## <a name="resource-owner-password-credential-grant-oauth-flow"></a>Пароль владельца ресурса. предоставление учетных данных для передачи OAuth

Потоки учетных данных для пароля владельца ресурса позволяют приложению выполнить вход в систему, используя имя пользователя и пароль. Используйте этот поток, только если вы не можете использовать другие потоки OAuth. Для получения дополнительных сведений см [платформа идентификации Майкрософт и учетные данные пароля владельца ресурса OAuth 2,0](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth-ropc)



# <a name="ctabcs"></a>[Языках](#tab/CS)

```csharp
IPublicClientApplication clientApplication = UsernamePasswordProvider.CreateClientApplication(clientId);
UsernamePasswordProvider authProvider = new UsernamePasswordProvider(clientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[Язык](#tab/Javascript)

Пока недоступно. Если это важно, проведите голосование или откройте [запрос функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) .

# <a name="javatabjava"></a>[Java](#tab/Java)

```java
UsernamePasswordProvider authProvider = new UsernamePasswordProvider(
                                                    clientId,
                                                    scopes,
                                                    username,
                                                    password);
```

# <a name="androidtabandroid"></a>[Android](#tab/Android)

Неприменимо.

# <a name="objective-ctabobjective-c"></a>[Цель — C](#tab/Objective-C)

Неприменимо.

# <a name="phptabphp"></a>[PHP](#tab/PHP)

Пока недоступно. Если это важно, проведите голосование или откройте [запрос функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) .

# <a name="rubytabruby"></a>[Ruby](#tab/Ruby)

Пока недоступно. Если это важно, проведите голосование или откройте [запрос функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) .

---

## <a name="next-steps"></a>Дальнейшие действия

* Для поставщиков проверки подлинности требуется идентификатор клиента. Вы захотите [зарегистрировать приложение](https://portal.azure.com/) после настройки поставщика проверки подлинности.
* Сообщите нам, если требуемый потоки OAuth в настоящее время не поддерживается голосованием или открытием [запроса функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests).