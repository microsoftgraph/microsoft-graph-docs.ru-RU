---
title: Поставщик MSAL
description: Поставщик MSAL использует MSAL. js для входа пользователей и получения маркеров для использования с Microsoft Graph.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: b66fd9a640c6baa84767e1ab08821b80384a5464
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2019
ms.locfileid: "35243077"
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
                   authority=""></mgt-msal-provider>
```

>**Примечание:** `login-type` и `authority` являются необязательными.

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

Сведения о том, как зарегистрировать приложение и получить идентификатор клиента, можно найти в разделе [Регистрация краткого руководства по работе с приложением](https://docs.microsoft.com/en-us/azure/active-directory/develop/quickstart-register-app).

>**Примечание:** MSAL поддерживает только неявный поток для OAuth. Не забудьте включить неявный поток в приложении на портале Azure (по умолчанию он не включен). В **разделе Проверка**подлинности найдите раздел неявный **предоставление** и установите флажки для **маркеров доступа** и **маркеров ID**.
