---
title: Поставщик MSAL
description: Поставщик MSAL использует MSAL.js для входа пользователей и получения маркеров для использования с Microsoft Graph.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: e66434a1000667891304db5f0cff78c4e8b38152
ms.sourcegitcommit: 7e1993d64cc6d3145ae0ca984fefe74772b6052b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/16/2020
ms.locfileid: "47843158"
---
# <a name="msal-provider"></a>Поставщик MSAL

Поставщик MSAL использует [MSAL.js](https://github.com/AzureAD/microsoft-authentication-library-for-js) для входа пользователей и получения маркеров для использования с Microsoft Graph.

Чтобы узнать больше, ознакомьтесь со статьей [поставщики](../providers.md).

## <a name="get-started"></a>Начало работы

Вы можете инициализировать поставщик MSAL в HTML или JavaScript.

### <a name="initialize-in-your-html-page"></a>Инициализация на HTML-странице

Инициализация поставщика MSAL в HTML является самым простым способом создания нового поставщика. Используйте `mgt-msal-provider` компонент, чтобы задать **идентификатор клиента** и другие свойства. При этом будет создан новый `UserAgentApplication` экземпляр, который будет использоваться для всех проверок подлинности и получения маркеров.

```html
<mgt-msal-provider client-id="<YOUR_CLIENT_ID>"
                   login-type="redirect/popup"
                   scopes="user.read,people.read"
                   redirect-uri="https://my.redirect/uri"
                   authority=""></mgt-msal-provider>
```

| Атрибут    | Описание                                                                                                                                                                                                                                                           |
|--------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Client — ID    | Идентификатор строкового клиента (см. Создание идентификатора приложения или клиента). Обязательно.                                                                                                                                                                                                           |
| Тип входа   | Перечисление между `redirect` `popup` значением и значением по умолчанию — `redirect` . Необязательный параметр.                                                                                                                                                                                   |
| scopes       | Строки, разделенные запятыми, для областей, которые пользователь должен согласиться на вход в систему. Необязательный параметр.                                                                                                                                                                                     |
| авторитет    | Строка Authority — значение по умолчанию — общий центр. Для приложений с одним клиентом используйте идентификатор клиента или имя клиента. Например, `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` или `https://login.microsoftonline.com/[your-tenant-id]` . Необязательный параметр. |
| Redirect — URI | Строка URI перенаправления — по умолчанию используется текущий URI окна. Необязательный параметр.                                                                                                                                                                                            |
| зависит от   | Строка выбора элемента с другим компонентом поставщика более высокого приоритета. Необязательный параметр.                                                                                                                                                                                      |

### <a name="initialize-in-javascript"></a>Инициализация в JavaScript

Вы можете предоставить дополнительные параметры, инициализируя поставщик в JavaScript.

```ts
import {Providers, MsalProvider} from '@microsoft/mgt'
import {UserAgentApplication} from "msal";

Providers.globalProvider = new MsalProvider(config: MsalConfig);
```

где Мсалконфиг:

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

Необходимо указать `clientId` (чтобы создать новый `UserAgentApplication` ).

Дополнительные сведения о MSAL.js и дополнительных параметрах, которые можно использовать при инициализации библиотеки MSAL, приведены в [документации по MSAL](https://docs.microsoft.com/azure/active-directory/develop/msal-js-initializing-client-applications).

## <a name="creating-an-appclient-id"></a>Создание идентификатора приложения или клиента

Сведения о том, как зарегистрировать приложение и получить идентификатор клиента, можно найти в разделе [Регистрация краткого руководства по работе с приложением](/azure/active-directory/develop/quickstart-register-app).

>**Примечание:** MSAL поддерживает только неявный поток для OAuth. Не забудьте включить неявный поток в приложении на портале Azure (по умолчанию он не включен). В разделе **Проверка подлинности**найдите раздел **неявный предоставление** и установите флажки для **маркеров доступа** и **маркеров ID**. Чтобы использовать общий орган, задайте **учетную запись в любом организационном каталоге**. Чтобы использовать определенный клиент, задайте `authority` во время инициализации.
