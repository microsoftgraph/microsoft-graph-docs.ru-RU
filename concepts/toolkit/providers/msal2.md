---
title: Поставщик MSAL2
description: Поставщик MSAL 2 использует msal-browser для регистрации пользователей и приобретения маркеров для использования в Microsoft Graph
ms.localizationpriority: medium
author: amrutha95
ms.openlocfilehash: 80178f379d0f6d9101cec794bc1d0d36ccb640d7
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59143484"
---
# <a name="msal2-provider"></a>Поставщик MSAL2

Поставщик MSAL2 использует [msal-browser](https://github.com/AzureAD/microsoft-authentication-library-for-js/tree/dev/lib/msal-browser) для регистрации пользователей и приобретения маркеров для использования в Microsoft Graph.

Дополнительные дополнительные новости см. [в см. в руберсе "Поставщики услуг".](./providers.md)

## <a name="difference-between-msal2-provider-and-msal-provider"></a>Разница между поставщиком MSAL2 и поставщиком MSAL
Хотя использование аналогично, поставщик MSAL и поставщик MSAL2 построены на разных потоках OAuth. Поставщик MSAL построен на msal.js, которая реализует неявный грант OAuth2.0 [Flow.](/azure/active-directory/develop/v2-oauth2-implicit-grant-flow) Поставщик MSAL2 построен на [msal-браузере,](https://github.com/AzureAD/microsoft-authentication-library-for-js/tree/dev/lib/msal-browser)который реализует код авторизации OAuth 2.0 [](/azure/active-directory/develop/v2-oauth2-auth-code-flow) Flow с PKCE.
Поскольку код авторизации Flow более безопасным, чем неявный грант Flow для веб-приложений, рекомендуется использовать Msal2Provider над MsalProvider. Сведения о проблемах безопасности, связанных с неявным потоком грантов, см. в материале [Недостатки неявного потока.](https://tools.ietf.org/html/draft-ietf-oauth-browser-based-apps-04#section-9.8.6)

Все новые приложения должны использовать поставщика MSAL2 по мере возможности. 

## <a name="get-started"></a>Начало работы

Вы можете инициализировать поставщика MSAL2 в HTML или JavaScript.

### <a name="initialize-in-your-html-page"></a>Инициализация на странице HTML

Инициализация поставщика MSAL2 в HTML является простейшим способом создания нового поставщика. Используйте компонент `mgt-msal2-provider` для набора **клиентских и** других свойств. Это создаст новый экземпляр, который будет использоваться для всех маркеров проверки подлинности и `PublicClientApplication` приобретения.

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
| client-id    | Строковая ID клиента (см. статью Создание ID приложения/клиента). Обязательный.                                                                                                                                                                                                           |
| тип входа   | Переумеление между `redirect` и по умолчанию является `popup` `redirect` значением . Необязательно.                                                                                                                                                                                   |
| scopes       | Строки с разделителями-запятыми для областей, которым пользователь должен предоставить согласие при входе. Необязательный.                                                                                                                                                                                     |
| authority    | Строка Authority — по умолчанию является общим органом. Для однотенантного приложения используйте идентификатор клиента или имя клиента. Например, `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` или `https://login.microsoftonline.com/[your-tenant-id]`. Необязательный. |
| redirect-uri | Строка URI перенаправления — по умолчанию используется текущее окно URI. Необязательно.                                                                                                                                                                                            |
| Подсказка       | Тип запроса для входа, между ```SELECT_ACCOUNT``` и ```CONSENT``` ```LOGIN``` . Значение по умолчанию: ```SELECT_ACCOUNT```. Необязательно.

### <a name="initialize-in-javascript"></a>Инициализация в JavaScript

Вы можете предоставить больше вариантов, инициализируя поставщика в JavaScript.

```ts
    import {Providers} from '@microsoft/mgt-element';
    import {Msal2Provider, Msal2Config, Msal2PublicClientApplicationConfig} from '@microsoft/mgt-msal2-provider';

    // initialize the auth provider globally
    Providers.globalProvider = new Msal2Provider(config: Msal2Config | Msal2PublicClientApplicationConfig);
```

Параметр конструктора можно настроить двумя способами, как описано `Msal2Provider` в следующих разделах.

#### <a name="provide-a-clientid-to-create-a-new-publicclientapplication"></a>Предоставление для `clientId` создания нового `PublicClientApplication`

Этот параметр имеет смысл, когда корпорация Майкрософт Graph набор средств за всю проверку подлинности в вашем приложении.

```ts
interface Msal2Config {
  clientId: string;
  scopes?: string[];
  authority?: string;
  redirectUri?: string;
  loginType?: LoginType; // LoginType.Popup or LoginType.Redirect (redirect is default)
  prompt?: PromptType; // PromptType.CONSENT, PromptType.LOGIN or PromptType.SELECT_ACCOUNT
  sid?: string; // Session ID
  loginHint?: string;
  domainHint?: string;
  options?: Configuration // msal-browser Configuration object
}
```

#### <a name="pass-an-existing-publicclientapplication-in-the-publicclientapplication-property"></a>Передай `PublicClientApplication` существующее `publicClientApplication` в свойстве.

Используйте это, когда ваше приложение использует функции MSAL за пределами возможностей, открытых другими функциями `Msal2Provider` Microsoft Graph набор средств. Это особенно уместно, если фреймворк автоматически мгновенно и предоставляет для вас значение a; например, при использовании `PublicClientApplication` [msal-angular](/azure/active-directory/develop/tutorial-v2-angular). Дополнительные рекомендации см. в примере репо `angular-app` microsoft [Graph набор средств.](https://github.com/microsoftgraph/microsoft-graph-toolkit)

При использовании этого параметра необходимо понимать возможности для столкновений. По своему характеру существует риск, что состояние сеанса может измениться; например, при входе пользователя или согласии на `Msal2Provider` дополнительные области. Убедитесь, что ваше приложение и другие фреймворки реагируют на эти изменения в состоянии, или рассмотрите возможность использования [пользовательского поставщика.](./custom.md)

```ts
interface Msal2PublicClientApplicationConfig {
  publicClientApplication: PublicClientApplication;
  scopes?: string[];
  authority?: string;
  redirectUri?: string;
  loginType?: LoginType; // LoginType.Popup or LoginType.Redirect (redirect is default)
  prompt?: PromptType; // PromptType.CONSENT, PromptType.LOGIN or PromptType.SELECT_ACCOUNT
  sid?: string; // Session ID
  loginHint?: string;
  domainHint?: string;
  options?: Configuration // msal-browser Configuration object
}
```

## <a name="creating-an-appclient-id"></a>Создание идентификатора клиента/приложения

Дополнительные сведения о том, как зарегистрировать приложение и получить клиентский ID, см. в Azure Active Directory [app.](../get-started/add-aad-app-registration.md)

## <a name="migrating-from-msal-provider-to-msal2-provider"></a>Переход от поставщика MSAL к поставщику MSAL2
Чтобы перенести приложение, использующее поставщика MSAL, к поставщику MSAL2:
1. Перейдите на портал Azure по адресу https://portal.azure.com.
1. В меню выберите **Azure Active Directory**.
1. В меню Azure Active Directory выберите **Регистрация приложений**.
1. Выберите регистрацию приложения, используемого в настоящее время. 
1. Перейдите **к проверке подлинности** в левом меню.
1. В **настройках платформы** нажмите кнопку **Добавить платформу** и выберите **одно-страницное приложение.**
1. Удалите все URL-адреса перенаправления, зарегистрированные в **интернете,** и добавьте их в **одностражном приложении.**
1. В коде замените `MSALProvider` `MSAL2Provider` .

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
