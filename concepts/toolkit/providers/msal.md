---
title: Поставщик MSAL
description: Поставщик MSAL использует MSAL. js для входа пользователей и получения маркеров для использования с Microsoft Graph.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 95dfae9954ff098ae9e777c3c330c5f334b8b0aa
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40868494"
---
# <a name="msal-provider"></a>Поставщик MSAL

Поставщик MSAL использует [MSAL. js](https://github.com/AzureAD/microsoft-authentication-library-for-js) для входа пользователей и получения маркеров для использования с Microsoft Graph.

Чтобы узнать больше, ознакомьтесь со статьей [поставщики](../providers.md).

## <a name="get-started"></a>Начало работы

Вы можете инициализировать поставщик MSAL в HTML или JavaScript.

### <a name="initialize-in-your-html-page"></a>Инициализация на HTML-странице

Инициализация поставщика MSAL в HTML является самым простым способом создания нового поставщика. Используйте `mgt-msal-provider` компонент, чтобы задать **идентификатор клиента** и другие свойства. При этом будет создан новый `UserAgentApplication` экземпляр, который будет использоваться для всех проверок подлинности и получения маркеров.

```html
<mgt-msal-provider client-id="<YOUR_CLIENT_ID>"
                   login-type="redirect/popup"
                   scopes="user.read,people.read"
                   authority=""></mgt-msal-provider>
```

| Атрибут | Описание |
| --- | --- | --- |
| Client — ID   | Идентификатор строкового клиента (см. Создание идентификатора приложения или клиента). Обязательный атрибут.|
| Тип входа  | `redirect` Перечисление `popup` между значением и значением `redirect`по умолчанию —. Необязательный атрибут. |
| scopes  | Строки, разделенные запятыми, для областей, которые пользователь должен согласиться на вход в систему. Необязательный атрибут.|
| авторитет  | Строка Authority — значение по умолчанию — общий центр. Необязательный атрибут.|
| зависит от | Строка выбора элемента с другим компонентом поставщика более высокого приоритета. Необязательный атрибут. |

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
  loginType?: LoginType;
  options?: Configuration; // msal js Configuration object
}
```

Необходимо указать `clientId` (чтобы создать новый `UserAgentApplication`).

Дополнительные сведения см. в [документации по MSAL](https://github.com/AzureAD/microsoft-authentication-library-for-js/wiki/MSAL-basics).

## <a name="creating-an-appclient-id"></a>Создание идентификатора приложения или клиента

Сведения о том, как зарегистрировать приложение и получить идентификатор клиента, можно найти в разделе [Регистрация краткого руководства по работе с приложением](/azure/active-directory/develop/quickstart-register-app).

>**Примечание:** MSAL поддерживает только неявный поток для OAuth. Не забудьте включить неявный поток в приложении на портале Azure (по умолчанию он не включен). В разделе **Проверка подлинности**найдите раздел **неявный предоставление** и установите флажки для **маркеров доступа** и **маркеров ID**.
