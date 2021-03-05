---
title: Поставщик электронных данных
description: Поставщик MSAL для Electron использует msal-node для регистрации пользователей и приобретения маркеров для использования в Microsoft Graph.
localization_priority: Normal
author: amrutha95
ms.openlocfilehash: a9e391f96988f8beaf8395e872a6efa08efca8f5
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471436"
---
# <a name="electron-provider"></a>Поставщик электронных данных

Поставщик Электронный использует [msal-node](https://github.com/AzureAD/microsoft-authentication-library-for-js/tree/dev/lib/msal-node) для регистрации пользователей и приобретения маркеров для использования с Microsoft Graph в приложении Electron.

Дополнительные сведения о поставщиках проверки подлинности см. в статье [Поставщики](./providers.md).

## <a name="get-started"></a>Начало работы
### <a name="install-the-packages"></a>Установка пакетов

```bash
npm install @microsoft/mgt-element @microsoft/mgt-electron-provider
```
Необходимо инициализировать ElectronProvider в процессе рендера (передняя часть) и ElectronAuthenticator в основном процессе (задней части).


### <a name="initializing-electronprovider-in-the-renderer-process-rendererts"></a>Инициализация ElectronProvider в процессе рендера (renderer.ts)

ElectronProvider отвечает за связь с ElectronAuthenticator (в основном процессе) для запроса маркеров доступа и получения сведений о в журнале в состоянии, необходимом для работы компонентов. 

```ts
import {Providers} from '@microsoft/mgt-element';
import {ElectronProvider} from '@microsoft/mgt-electron-provider/dist/Provider';
import '@microsoft/mgt-components';

// initialize the auth provider globally
Providers.globalProvider = new ElectronProvider();
```

### <a name="initializing-electronauthenticator-in-the-main-process-maints"></a>Инициализация ElectronAuthenticator в основном процессе (main.ts)

ElectronAuthenticator отвечает за настройку переменных конфигурации для проверки подлинности MSAL, получения маркеров доступа и связи с ElectronProvider.
Инициализировать электронныйAuthenticator в основном процессе и настроить параметры конфигурации, такие как client-id.

```ts
import { ElectronAuthenticator, MsalElectronConfig } from '@microsoft/mgt-electron-provider/dist/Authenticator'; 

let config: MsalElectronConfig = {
  clientId: '<your_client_id>',
  authority: '<your_authority_url>', //optional
  mainWindow: mainWindow, 
  scopes: ['user.read'] //We recommend pre-consenting all the required scopes on the Azure portal
};

ElectronAuthenticator.initialize(config);
```
 
| Атрибут    | Описание                                                                                                                                                                                                                                                           |
|--------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| clientId    | Строковая ID клиента (см. статью Создание ID приложения/клиента). Обязательный.                                                                                                                                                                                                           |                                                                                                                                                                               |
| scopes       | Разделенные запятой строки для областей, на которые пользователь должен дать согласие при входе. Рекомендуется.                                                                                                                                                                                     |
| authority    | Строка Authority — по умолчанию является общим органом. Для однотенантного приложения используйте идентификатор клиента или имя клиента. Например, `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` или `https://login.microsoftonline.com/[your-tenant-id]`. Необязательный. |                                                                                                                                                                                          |
| mainWindow  | Экземпляр основного BrowserWindow, требуемого проверки подлинности.|
| cachePlugin | Плагин кэша, который вы хотите использовать для сохраняемого хранения маркеров. См. [расширения проверки подлинности Майкрософт для узла.](https://github.com/AzureAD/microsoft-authentication-library-for-js/tree/dev/extensions/msal-node-extensions) Необязательно. | 

>**Примечание:** В настоящее время поставщик не поддерживает инкрементную поддержку. В качестве наилучшей практики обязательно соглашайтесь на все области, которые требуются компонентам.
    
## <a name="create-an-appclient-id"></a>Создание идентификатора клиента/приложения

### <a name="add-new-application-registration-in-azure-active-directory-to-get-a-client-id"></a>Добавьте новую регистрацию приложений в Azure Active Directory, чтобы получить ID клиента

Чтобы создать приложение в Azure Active Directory, добавьте новую регистрацию приложений, а затем настройте имя приложения и перенаправляйте URI.

Создание приложения в Azure Active Directory:

1. Перейдите на [портал Azure.](https://portal.azure.com)
1. В меню выберите **Azure Active Directory**.
1. В меню Azure Active Directory выберите **Регистрация приложений**.
1. В верхнем меню нажмите кнопку **Новая регистрация**.
1. Введите имя приложения; например, `My Electron-App` .
1. Для параметра [Поддерживаемые типы учетных записей](/azure/active-directory/develop/single-and-multi-tenant-apps#who-can-sign-in-to-your-app) выберите **Учетные записи в любом каталоге организации (любой каталог Azure AD — мультитенантный) и персональные учетные записи Майкрософт (например, Skype, Xbox)**.
1. В поле **Перенаправление URI** в отсеве выберите общедоступный **клиент/родной (мобильный &** рабочий стол), а в поле URL-адрес введите `msal://redirect` .
1. Подтвердите изменения, нажав кнопку **Зарегистрировать**.

## <a name="next-steps"></a>Дальнейшие действия

* Ознакомьтесь с пошаговой инструкцией по [построению электронного приложения.](../get-started/build-an-electron-app.md)
* Взгляните на пример [приложения Electron,](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/main/samples/electron-app) которое показывает, как использовать поставщика Электронный.
