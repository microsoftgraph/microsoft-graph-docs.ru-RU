---
title: Поставщик MSAL
description: Поставщик MSAL использует MSAL.js для входа пользователей и получения маркеров для использования с Microsoft Graph.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 0edb6fba29c5ee0dcb37199db055761088408be6
ms.sourcegitcommit: 186d738f04e5a558da423f2429165fb4fbe780aa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086615"
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
| Client — ID    | Идентификатор строкового клиента (см. Создание идентификатора приложения или клиента). Обязательный.                                                                                                                                                                                                           |
| Тип входа   | Перечисление между `redirect` `popup` значением и значением по умолчанию — `redirect` . Необязательный атрибут.                                                                                                                                                                                   |
| scopes       | Строки, разделенные запятыми, для областей, которые пользователь должен согласиться на вход в систему. Необязательный атрибут.                                                                                                                                                                                     |
| авторитет    | Строка Authority — значение по умолчанию — общий центр. Для приложений с одним клиентом используйте идентификатор клиента или имя клиента. Например, `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` или `https://login.microsoftonline.com/[your-tenant-id]` . Необязательный атрибут. |
| Redirect — URI | Строка URI перенаправления — по умолчанию используется текущий URI окна. Необязательный атрибут.                                                                                                                                                                                            |
| зависит от   | Строка выбора элемента с другим компонентом поставщика более высокого приоритета. Необязательный атрибут.                                                                                                                                                                                      |

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

Дополнительные сведения о MSAL.js и дополнительных параметрах, которые можно использовать при инициализации библиотеки MSAL, приведены в [документации по MSAL](/azure/active-directory/develop/msal-js-initializing-client-applications).

## <a name="creating-an-appclient-id"></a>Создание идентификатора приложения или клиента

Сведения о том, как зарегистрировать приложение и получить идентификатор клиента, можно найти в статье [Создание приложения Azure Active Directory](../get-started/add-aad-app-registration.md).