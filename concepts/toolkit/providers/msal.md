---
title: Поставщик MSAL
description: Поставщик MSAL использует MSAL.js для регистрации пользователей и приобретения маркеров для использования в Microsoft Graph
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: e612e11e7b1a26765175ba10097c8e54317e9e1d
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579762"
---
# <a name="msal-provider"></a>Поставщик MSAL

Поставщик MSAL [использует](https://github.com/AzureAD/microsoft-authentication-library-for-js)MSAL.jsдля регистрации пользователей и приобретения маркеров для использования в Microsoft Graph.

Дополнительные дополнительные новости см. [в см. в руберсе "Поставщики услуг".](./providers.md)

## <a name="get-started"></a>Начало работы

Вы можете инициализировать поставщика MSAL в HTML или JavaScript.

### <a name="initialize-in-your-html-page"></a>Инициализация на странице HTML

Инициализация поставщика MSAL в HTML является простейшим способом создания нового поставщика. Используйте компонент `mgt-msal-provider` для набора **клиентских и** других свойств. Это создаст новый экземпляр, который будет использоваться для всех маркеров проверки подлинности и `UserAgentApplication` приобретения.

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
| client-id    | Строковая ID клиента (см. статью Создание ID приложения/клиента). Обязательное.                                                                                                                                                                                                           |
| тип входа   | Переумеление между `redirect` и по умолчанию является `popup` `redirect` значением . Необязательно.                                                                                                                                                                                   |
| scopes       | Строки с разделителями-запятыми для областей, которым пользователь должен предоставить согласие при входе. Необязательный.                                                                                                                                                                                     |
| authority    | Строка Authority — по умолчанию является общим органом. Для однотенантного приложения используйте идентификатор клиента или имя клиента. Например, `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` или `https://login.microsoftonline.com/[your-tenant-id]`. Необязательный. |
| redirect-uri | Строка URI перенаправления — по умолчанию используется текущее окно URI. Необязательный.                                                                                                                                                                                            |
| depends-on   | Строка селектора элементов другого компонента поставщика с более высоким приоритетом. Необязательно. 
| подсказка домена  | Строка запроса расположения домена для переададации в опытом. Необязательно.              
| Подсказка | Выбор типа взаимодействия с пользователем, необходимого для входа в систему. Допустимые параметры: <ul><li>`login` заставляет пользователя вводить учетные данные по запросу </li><li>`none` без интерактивной подсказки</li> <li>`select_account` отправка пользователя в выборщик учетной записи</li><li>`consent` отправка пользователя в диалоговое окно согласия OAuth</li></ul> Дополнительные сведения см. в статье [оперативное ](/azure/active-directory/develop/msal-js-prompt-behavior) поведение MSAL.jsстатье. Необязательно.                                                                                                                                                                            |


### <a name="initialize-in-javascript"></a>Инициализация в JavaScript

Вы можете предоставить больше вариантов, инициализируя поставщика в JavaScript.

```ts
import {Providers, MsalProvider} from '@microsoft/mgt'
import {UserAgentApplication} from "msal";

Providers.globalProvider = new MsalProvider(config: MsalConfig);
```

Параметр конструктора можно настроить двумя способами, как описано `MsalProvider` в следующих разделах.

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

#### <a name="pass-an-existing-useragentapplication-in-the-useragentapplication-property"></a>Передай `UserAgentApplication` существующее `userAgentApplication` в свойстве.

Используйте это, когда ваше приложение использует функции MSAL за пределами возможностей, открытых другими функциями `MsalProvider` Microsoft Graph набор средств. Это особенно уместно, если фреймворк автоматически мгновенно и предоставляет для вас значение a; например, при использовании `UserAgentApplication` [msal-angular](/azure/active-directory/develop/tutorial-v2-angular).

При использовании этого параметра необходимо понимать возможности для столкновений. По своей природе существует риск того, что состояние сеанса может измениться, например, путем входов пользователя или согласия на `MsalProvider` дополнительные области. Убедитесь, что ваше приложение и другие фреймворки реагируют на эти изменения в состоянии, или рассмотрите возможность использования [пользовательского поставщика.](./custom.md)

```ts
interface MsalConfig {
  userAgentApplication: UserAgentApplication;
  scopes?: string[];
  loginType?: LoginType; // LoginType.Popup or LoginType.Redirect (redirect is default)
  loginHint?: string;
}
```

Дополнительные дополнительные MSAL.js и дополнительные возможности, которые можно использовать при инициализации библиотеки MSAL, см. в [документации MSAL.](/azure/active-directory/develop/msal-js-initializing-client-applications)

## <a name="creating-an-appclient-id"></a>Создание идентификатора клиента/приложения

Дополнительные сведения о том, как зарегистрировать приложение и получить клиентский ID, см. в Azure Active Directory [app.](../get-started/add-aad-app-registration.md)
