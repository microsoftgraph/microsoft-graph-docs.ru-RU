---
title: Поставщик MSAL 2
description: Поставщик MSAL 2 использует msal-browser для регистрации пользователей и приобретения маркеров для использования в Microsoft Graph
localization_priority: Normal
author: amrutha95
ms.openlocfilehash: f856c900b0b8aace7a1c2248d2921b39fe0a2c44c6fc9e05c35003c0d0c53d50
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54204917"
---
# <a name="msal-2--provider"></a>Поставщик MSAL 2

Поставщик MSAL 2 использует [msal-browser](https://github.com/AzureAD/microsoft-authentication-library-for-js/tree/dev/lib/msal-browser) для регистрации пользователей и приобретения маркеров для использования в Microsoft Graph.
Дополнительные дополнительные новости см. [в см. в руберсе "Поставщики услуг".](./providers.md)

## <a name="get-started"></a>Начало работы

Вы можете инициализировать поставщика MSAL 2.0 в HTML или JavaScript.

### <a name="initialize-in-your-html-page"></a>Инициализация на странице HTML

Инициализация поставщика MSAL 2 в HTML — самый простой способ создания нового поставщика. Используйте компонент `mgt-msal2-provider` для набора **клиентских и** других свойств. Это создаст новый экземпляр, который будет использоваться для всех маркеров проверки подлинности и `PublicClientApplication` приобретения.

```html
    <mgt-msal2-provider client-id="<YOUR_CLIENT_ID>"
                        login-type="redirect/popup" 
                        scopes="user.read,people.read" 
                        redirect-uri="https://my.redirect/uri" 
                        authority=""> 
    </mgt-msal2-provider> 
```

| Атрибут    | Описание                                                                                                                                                                                                                                                           |
|--------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| client-id    | Строковая ID клиента (см. статью Создание ID приложения/клиента). Обязательный элемент.                                                                                                                                                                                                           |
| тип входа   | Переумеление между `redirect` и по умолчанию является `popup` `redirect` значением . Необязательно.                                                                                                                                                                                   |
| scopes       | Строки с разделителями-запятыми для областей, которым пользователь должен предоставить согласие при входе. Необязательный.                                                                                                                                                                                     |
| authority    | Строка Authority — по умолчанию является общим органом. Для однотенантного приложения используйте идентификатор клиента или имя клиента. Например, `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` или `https://login.microsoftonline.com/[your-tenant-id]`. Необязательный. |
| redirect-uri | Строка URI перенаправления — по умолчанию используется текущее окно URI. Необязательно.                                                                                                                                                                                            |
| Подсказка       | Тип запроса для входа, между ```SELECT_ACCOUNT``` и ```CONSENT``` ```LOGIN``` . Значение по умолчанию: ```SELECT_ACCOUNT```. Необязательно.

### <a name="initialize-in-javascript"></a>Инициализация в JavaScript

Вы можете предоставить больше вариантов, инициализируя поставщика в JavaScript.

```ts
    import {Providers, LoginType} from '@microsoft/mgt-element';
    import {Msal2Provider, PromptType} from '@microsoft/mgt-msal2-provider';

    // initialize the auth provider globally
    Providers.globalProvider = new Msal2Provider({
      clientId: 'REPLACE_WITH_CLIENTID',
      scopes?: string[],
      authority?: string,
      redirectUri?: string,
      loginType?: LoginType, // LoginType.Popup or LoginType.Redirect (redirect is default)
      prompt?: PromptType, // PromptType.CONSENT, PromptType.LOGIN or PromptType.SELECT_ACCOUNT
      sid?: string, // Session ID
      loginHint?: string,
      domainHint?: string,
      options?: Configuration // msal js Configuration object
    });
```

## <a name="creating-an-appclient-id"></a>Создание идентификатора клиента/приложения

Дополнительные сведения о том, как зарегистрировать приложение и получить клиентский ID, см. в Azure Active Directory [app.](../get-started/add-aad-app-registration.md)

## <a name="difference-between-msal2provider-and-msalprovider"></a>Разница между Msal2Provider и MsalProvider
Несмотря на то, что использование очень похоже, MsalProvider и Msal2Provider построены на основе различных потоков OAuth. MsalProvider построен на вершине MSAL.js, которая реализует неявный грант OAuth2.0 [Flow](/azure/active-directory/develop/v2-oauth2-implicit-grant-flow). Msal2Provider построен на основе [msal-browser,](https://github.com/AzureAD/microsoft-authentication-library-for-js/tree/dev/lib/msal-browser)который реализует код авторизации OAuth 2.0 [Flow](/azure/active-directory/develop/v2-oauth2-auth-code-flow) с PKCE.
Код авторизации Flow более безопасный, чем неявный грант Flow для веб-приложений, поэтому рекомендуется использовать MSAL2Provider над MSALProvider. Сведения о проблемах безопасности, связанных с неявным потоком грантов, см. в материале [Недостатки неявного потока.](https://tools.ietf.org/html/draft-ietf-oauth-browser-based-apps-04#section-9.8.6)

## <a name="migrating-from-msal-provider-to-msal-2-provider"></a>Переход от поставщика MSAL к поставщику MSAL 2
Чтобы перенести приложение, использующее поставщика MSAL, к поставщику MSAL 2:
1. Перейдите на портал Azure по адресу https://portal.azure.com.
1. В меню выберите **Azure Active Directory**.
1. В меню Azure Active Directory выберите **Регистрация приложений**.
1. Выберите регистрацию приложения, используемого в настоящее время. 
1. Перейдите **к проверке подлинности** в левом меню.
1. В **настройках платформы** нажмите кнопку **Добавить платформу** и выберите **одно-страницное приложение.**
1. Удалите все URL-адреса перенаправления, зарегистрированные в **интернете,** и добавьте их в **одностражном приложении.**
1. В коде замените MSALProvider на MSAL2Provider.

    Если вы инициализируете поставщика в коде JS/TS, выполните следующие действия:
    
    Замените заявление на ```mgt-msal-provider``` импорт 
    ```ts 
    import {Msal2Provider, PromptType} from '@microsoft/mgt-msal2-provider';
    ```

    Замените инициализацию MsalProvider
    ```ts
    Providers.globalProvider = new Msal2Provider({ 
      clientId: 'REPLACE_WITH_CLIENTID'
      ...
    })
    ```
    Если вы инициализируете поставщика в HTML, замените 
    ```html
    <mgt-msal-provider client-id="" ... ></mgt-msal-provider>
    ``` 
    с 
    ```html
    <mgt-msal2-provider  client-id="" ... ></mgt-msal2-provider>
     ```
    Подробные сведения см. [в материале Initialize на странице HTML.](#initialize-in-your-html-page)
