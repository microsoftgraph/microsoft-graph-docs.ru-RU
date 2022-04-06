---
title: Поставщик MSAL
description: Поставщик MSAL использует MSAL.js для регистрации пользователей и приобретения маркеров для использования в Microsoft Graph.
ms.localizationpriority: medium
author: sebastienlevert
ms.openlocfilehash: 08c12c4ba7b105573e7a19a705a804c5c9f92114
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2022
ms.locfileid: "64587041"
---
# <a name="msal-provider"></a>Поставщик MSAL

Поставщик MSAL использует [msal.js](https://github.com/AzureAD/microsoft-authentication-library-for-js) для регистрации пользователей и приобретения маркеров для использования в Microsoft Graph.

Дополнительные дополнительные новости см. [в дополнительных данных.](./providers.md)

## <a name="difference-between-msal2-provider-and-msal-provider"></a>Разница между поставщиком MSAL2 и поставщиком MSAL
Хотя использование аналогично, поставщик MSAL и поставщик MSAL2 построены на разных потоках OAuth. Поставщик MSAL построен на msal.js, которая реализует неявный грант OAuth2.0 [Flow](/azure/active-directory/develop/v2-oauth2-implicit-grant-flow). MsAL2 Provider построен на [msal-browser](https://github.com/AzureAD/microsoft-authentication-library-for-js/tree/dev/lib/msal-browser), который реализует код авторизации OAuth [2.0 Flow](/azure/active-directory/develop/v2-oauth2-auth-code-flow) с PKCE.
Поскольку код авторизации Flow более безопасный, чем неявный грант Flow для веб-приложений, мы рекомендуем использовать поставщика MSAL2 над поставщиком MSAL. Сведения о проблемах безопасности, связанных с неявным потоком грантов, см. в материале [Недостатки неявного потока](https://tools.ietf.org/html/draft-ietf-oauth-browser-based-apps-04#section-9.8.6).

Все новые приложения должны использовать поставщика MSAL2 по мере возможности. Сведения о миграции см. в [msAL2 Provider](./msal2.md).

## <a name="get-started"></a>Начало работы

Вы можете инициализировать поставщика MSAL в HTML или JavaScript.

### <a name="initialize-in-your-html-page"></a>Инициализация на странице HTML

Инициализация поставщика MSAL в HTML является простейшим способом создания нового поставщика. Используйте компонент `mgt-msal-provider` для набора **клиентских и** других свойств. Это создаст новый экземпляр `UserAgentApplication` , который будет использоваться для всех маркеров проверки подлинности и приобретения.

```html
<mgt-msal-provider client-id="<YOUR_CLIENT_ID>"
                   login-type="redirect/popup"
                   scopes="user.read,people.read"
                   redirect-uri="https://my.redirect/uri"
                   authority=""
                   domainHint="mydomain.com"
                   prompt="consent"></mgt-msal-provider>
```

| Атрибут    | Описание                                                                                                                                                                                                                                                           |
|--------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| client-id    | Строковая ID клиента (см. статью Создание ID приложения/клиента). Обязательный аргумент.                                                                                                                                                                                                           |
| тип входа   | Переумеление между `redirect` и `popup` по умолчанию является значением `redirect`. Необязательно.                                                                                                                                                                                   |
| scopes       | Строки с разделителями-запятыми для областей, которым пользователь должен предоставить согласие при входе. Необязательный.                                                                                                                                                                                     |
| authority    | Строка Authority — по умолчанию является общим органом. Для однотенантного приложения используйте идентификатор клиента или имя клиента. Например, `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` или `https://login.microsoftonline.com/[your-tenant-id]`. Необязательный. |
| redirect-uri | Строка URI перенаправления — по умолчанию используется текущее окно URI. Необязательный.                                                                                                                                                                                            |
| depends-on   | Строка селектора элементов другого компонента поставщика с более высоким приоритетом. Необязательно. 
| подсказка домена  | Строка запроса расположения домена для переададации в опытом. Необязательно.              
| Подсказка | Выбор типа взаимодействия с пользователем, необходимого для входа в систему. Допустимые параметры: <ul><li>`login` заставляет пользователя вводить учетные данные по запросу </li><li>`none` без интерактивной подсказки</li> <li>`select_account` отправка пользователя в выборщик учетной записи</li><li>`consent` отправка пользователя в диалоговое окно согласия OAuth</li></ul> Дополнительные сведения см [. в статье ](/azure/active-directory/develop/msal-js-prompt-behavior) MSAL.jsоперативное поведение. Необязательно.                                                                                                                                                                            |


### <a name="initialize-in-javascript"></a>Инициализация в JavaScript

Вы можете предоставить больше вариантов, инициализируя поставщика в JavaScript.

```ts
import {Providers, MsalProvider} from '@microsoft/mgt'
import {UserAgentApplication} from "msal";

Providers.globalProvider = new MsalProvider(config: MsalConfig);
```

Параметр конструктора можно `MsalProvider` настроить двумя способами, как описано в следующих разделах.

#### <a name="provide-a-clientid-to-create-a-new-useragentapplication"></a>Предоставление для `clientId` создания нового `UserAgentApplication`

Этот параметр имеет смысл, Graph набор средств несет ответственность за всю проверку подлинности в вашем приложении.

```ts
interface MsalConfig {
  clientId: string;
  scopes?: string[];
  authority?: string;
  redirectUri?: string;
  loginType?: LoginType; // LoginType.Popup or LoginType.Redirect (redirect is default)
  loginHint?: string
  options?: Configuration; // msal js Configuration object
  domainHint?: string;
  prompt?: string; // "login", "none", "select_account", "consent"
}
```

#### <a name="pass-an-existing-useragentapplication-in-the-useragentapplication-property"></a>Передай существующее `UserAgentApplication` в свойстве `userAgentApplication` .

Используйте это, когда приложение использует функции MSAL `MsalProvider` за пределами того, что выставлено другими функциями Microsoft Graph набор средств. Это особенно уместно, если фреймворк `UserAgentApplication` автоматически моментирует и предоставляет для вас; например, при использовании [msal-angular](/azure/active-directory/develop/tutorial-v2-angular).

При использовании этого параметра необходимо понимать возможности для столкновений. По своей природе существует риск того, `MsalProvider` что состояние сеанса может измениться, например, путем входов пользователя или согласия на дополнительные области. Убедитесь, что ваше приложение и другие фреймворки реагируют на эти изменения в состоянии, или рассмотрите возможность использования [пользовательского поставщика](./custom.md) .

```ts
interface MsalConfig {
  userAgentApplication: UserAgentApplication;
  scopes?: string[];
  loginType?: LoginType; // LoginType.Popup or LoginType.Redirect (redirect is default)
  loginHint?: string;
}
```

Дополнительные дополнительные MSAL.js и дополнительные возможности, которые можно использовать при инициализации библиотеки MSAL, см. в [документации MSAL](/azure/active-directory/develop/msal-js-initializing-client-applications).

## <a name="creating-an-appclient-id"></a>Создание идентификатора клиента/приложения

Дополнительные сведения о том, как зарегистрировать приложение и получить клиентский ID, см. в Azure Active Directory [app](../get-started/add-aad-app-registration.md).
