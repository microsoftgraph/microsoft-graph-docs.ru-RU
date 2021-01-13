---
title: Поставщик MSAL
description: Поставщик MSAL использует MSAL.js для регистрации пользователей и получения маркеров для использования с Microsoft Graph
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: d3b3d82ae3c60080beaaff7f39a1324022d3ab2a
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2020
ms.locfileid: "49659176"
---
# <a name="msal-provider"></a>Поставщик MSAL

Поставщик MSAL использует [MSAL.js](https://github.com/AzureAD/microsoft-authentication-library-for-js) для регистрации пользователей и получения маркеров для использования с Microsoft Graph.

Дополнительные узнать см. [в поставщиках.](./providers.md)

## <a name="get-started"></a>Начало работы

Вы можете инициализировать поставщика MSAL в HTML или JavaScript.

### <a name="initialize-in-your-html-page"></a>Инициализация на HTML-странице

Инициализация поставщика MSAL в HTML является простейшим способом создания нового поставщика. Используйте `mgt-msal-provider` компонент, чтобы установить **ид клиента и** другие свойства. При этом будет создаваться новый экземпляр, который будет использоваться для проверки подлинности `UserAgentApplication` и получения маркеров.

```html
<mgt-msal-provider client-id="<YOUR_CLIENT_ID>"
                   login-type="redirect/popup"
                   scopes="user.read,people.read"
                   redirect-uri="https://my.redirect/uri"
                   authority=""></mgt-msal-provider>
```

| Атрибут    | Описание                                                                                                                                                                                                                                                           |
|--------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| client-id    | Строка ИД клиента (см. статью "Создание ИД приложения/клиента"). Обязательный.                                                                                                                                                                                                           |
| тип входа   | Enumeration between `redirect` and - default value is `popup` `redirect` . Необязательное свойство.                                                                                                                                                                                   |
| scopes       | Разделенные запятой строки для областей, на которые пользователь должен согласиться при входе. Необязательное свойство.                                                                                                                                                                                     |
| authority    | Строка "Полномочия" — по умолчанию является общим органом. Для приложений с одним клиентом используйте свой ИД клиента или имя клиента. Например, `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` или `https://login.microsoftonline.com/[your-tenant-id]` . Необязательное свойство. |
| redirect-uri | Строка URI перенаправления — по умолчанию используется URI текущего окна. Необязательное свойство.                                                                                                                                                                                            |
| зависит от   | Строка селектора элементов другого компонента поставщика с более высоким приоритетом. Необязательное свойство.                                                                                                                                                                                      |

### <a name="initialize-in-javascript"></a>Инициализация в JavaScript

Вы можете предоставить дополнительные параметры, инициализируя поставщика в JavaScript.

```ts
import {Providers, MsalProvider} from '@microsoft/mgt'
import {UserAgentApplication} from "msal";

Providers.globalProvider = new MsalProvider(config: MsalConfig);
```

Параметр конструктора можно настроить двумя способами, как описано `MsalProvider` в следующих разделах.

#### <a name="provide-a-clientid-to-create-a-new-useragentapplication"></a>Предоставление a `clientId` для создания нового `UserAgentApplication`

Этот вариант имеет смысл, если набор средств Graph отвечает за всю проверку подлинности в вашем приложении.

```ts
interface MsalConfig {
  clientId: string;
  scopes?: string[];
  authority?: string;
  redirectUri?: string;
  loginType?: LoginType; // LoginType.Popup or LoginType.Redirect (redirect is default)
  loginHint?: string
  options?: Configuration; // msal js Configuration object
}
```

#### <a name="pass-an-existing-useragentapplication-in-the-useragentapplication-property"></a>Передав `UserAgentApplication` существующий объект в `userAgentApplication` свойстве.

Используйте это, когда ваше приложение использует функции MSAL помимо возможностей, которые функциональность microsoft Graph набор средств `MsalProvider` функций. Это особенно целесообразно, если в структуре автоматически делается и предоставляется a для вас, например при использовании `UserAgentApplication` [msal-angular.](https://docs.microsoft.com/azure/active-directory/develop/tutorial-v2-angular)

При использовании этого параметра необходимо понимать возможности для столкновений. По своей природе существует риск того, что состояние сеанса может измениться, например, при входе пользователя или согласии на `MsalProvider` дополнительные области. Убедитесь, что ваше приложение и другие структуры корректно реагируют на эти изменения в состоянии, или рассмотрите возможность использования [настраиваемого поставщика.](/graph/toolkit/providers/custom)

```ts
interface MsalConfig {
  userAgentApplication: UserAgentApplication;
  scopes?: string[];
  loginType?: LoginType; // LoginType.Popup or LoginType.Redirect (redirect is default)
  loginHint?: string;
}
```

Дополнительные MSAL.js и дополнительные параметры, которые можно использовать при инициализации библиотеки MSAL, см. в [документации MSAL.](/azure/active-directory/develop/msal-js-initializing-client-applications)

## <a name="creating-an-appclient-id"></a>Создание приложения или ИД клиента

Дополнительные сведения о том, как зарегистрировать приложение и получить ИД клиента, см. в подстановке ["Создание приложения Azure Active Directory".](../get-started/add-aad-app-registration.md)
