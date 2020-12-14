---
title: Создание веб-приложения с помощью microsoft Graph набор средств
description: Начало создания веб-приложения с помощью microsoft Graph набор средств.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: 73e61e9d2c1c453ec67e61dce1f088b5119d1e8d
ms.sourcegitcommit: 7902607a1e5a030d46e907d08e16644a47a47006
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/12/2020
ms.locfileid: "49664018"
---
# <a name="build-a-web-application-with-the-microsoft-graph-toolkit"></a>Создание веб-приложения с помощью microsoft Graph набор средств

В этом разделе описывается, как начать работу с microsoft Graph набор средств в веб-приложении, написанном на javaScript. Если вы хотите узнать, как использовать веб-набор средств с веб-структурой, см. создание веб-приложения [(React)](./use-toolkit-with-react.md) или создание веб-приложения [(Angular).](./use-toolkit-with-angular.md)

Начало работы с microsoft Graph набор средств состоит из следующих этапов:
1. Добавьте microsoft Graph набор средств в свой проект.
2. Инициализация поставщика MSAL.
3. Добавление компонентов.
4. Протестировать приложение.

## <a name="add-the-microsoft-graph-toolkit-to-your-project"></a>Добавление в проект набор средств Microsoft Graph
Вы можете использовать microsoft Graph набор средств в приложении, ссылаясь на загрузчик напрямую (с помощью unpkg) или установив пакет npm.

# <a name="unpkg"></a>[unpkg](#tab/html)
Чтобы использовать набор средств mgt-loader, добавьте ссылку в сценарии в код:

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
```
# <a name="npm"></a>[npm](#tab/npm)
Использование набор средств с помощью модулей ES6 дает полный контроль над процессом пакетизации и позволяет объединить только код, необходимый для вашего приложения. Чтобы использовать модули ES6, добавьте пакет npm в проект:

```cmd
npm install @microsoft/mgt
```

---


> **Примечание.** Если вы нацелились на браузер, такой как IE11, который не поддерживает веб-компоненты по умолчанию, может потребоваться включить [полифайли.](./overview.md#polyfills)

## <a name="initialize-the-msal-provider"></a>Инициализация поставщика MSAL
Поставщики набор средств Microsoft Graph обеспечивают проверку подлинности и доступ к Microsoft Graph для компонентов. Дополнительные см. [в этой теме.](../providers/providers.md) Поставщик [MSAL использует](../providers/msal.md) MSAL.js для регистрации пользователей и получения маркеров. Вы можете инициализировать поставщика MSAL в HTML или JavaScript.

Если вы хотите использовать собственную проверку подлинности [](../providers/proxy.md) на сервере, используйте поставщика прокси-сервера, а не поставщика MSAL.

Вы можете инициализировать поставщика в коде HTML или JavaScript. 

# <a name="html"></a>[html](#tab/HTML)
Добавьте компонент `mgt-msal-provider` на HTML-страницу и задайте для нее код `client-id` клиента приложения.

```html
<mgt-msal-provider client-id="<YOUR_CLIENT_ID"></mgt-msal-provider>
```
# <a name="js"></a>[js](#tab/JavaScript)
Чтобы инициализировать поставщика MSAL в JavaScript, добавьте в приложение следующий код:

```js
import {Providers, MsalProvider} from '@microsoft/mgt'

Providers.globalProvider = new MsalProvider({
    clientId: "<YOUR_CLIENT_ID>"
})
```

---


ИД клиента — это единственное свойство, необходимое для инициализации поставщика, но можно настроить дополнительные параметры. Полный список см. в [списке Msal Provider.](../providers/msal.md)

### <a name="creating-an-appclient-id"></a>Создание приложения или ИД клиента
Чтобы получить ИД клиента, необходимо зарегистрировать приложение [в](./add-aad-app-registration.md) Azure AD. 
>**Примечание.** MSAL поддерживает только неявный поток для OAuth. Обязательно включите неявный поток в приложении на портале Azure (по умолчанию он не включен). В **разделе "Проверка подлинности"** найдите раздел неявного предоставления и выберите для маркеров **доступа** и **маркеров ID** свои почтовые ящики.  

## <a name="add-components"></a>Добавление компонентов
После инициализации поставщика MSAL можно приступить к использованию любого из набор средств компонентов.

# <a name="html"></a>[html](#tab/HTML)
Ниже приводится полный рабочий пример с использованием mgt-loader, поставщика MSAL, инициализированного в HTML, и компонента входа:

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal-provider>
<mgt-login></mgt-login>
```

Это пример использования модулей ES6, поставщика MSAL, инициализированного в HTML, и компонента входа:

```html
<script type="module" src="node_modules/@microsoft/mgt/dist/es6/index.js"></script>

<mgt-msal-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal-provider>

<mgt-login></mgt-login>
```
# <a name="js"></a>[js](#tab/JavaScript)
Это пример использования модулей ES6, поставщика MSAL, инициализированного в JavaScript, и компонента входа:

```js
import {Providers, MsalProvider} from '@microsoft/mgt'

Providers.globalProvider = new MsalProvider({
    clientId: "<YOUR_CLIENT_ID>"
})

function component() {
    const element = document.createElement('div');
    element.innerHTML = '<mgt-login></mgt-login>'
    return element;
}

document.body.appendChild((component()));
```

---


## <a name="test-your-app"></a>Тестирование приложения

Чтобы протестировать приложение, MSAL требует, чтобы страница была на веб-сервере для перенаправления проверки подлинности. 

Если вы только начинаете работу и хотите играть, вы можете использовать [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) в Visual Studio Code или любой другой облегченный сервер разработки. Скачайте расширение и откройте HTML-файл с помощью сервера live. 
> **Примечание.** Убедитесь, что **URI** перенаправления в регистрации приложения установлен на порт localhost, на который находится приложение. Перейдите к регистрации приложения на  [портале Azure,](https://portal.azure.com)выберите "Проверка подлинности под управлением" и добавьте правильный **URI перенаправления.**

## <a name="next-steps"></a>Дальнейшие действия
- Ознакомьтесь с этим пошаговом руководстве по [построению простого веб-приложения.](https://developer.microsoft.com/microsoft-365/blogs/a-lap-around-microsoft-graph-toolkit-day-2-zero-to-hero/)
- Попробуйте компоненты в игровой [области.](https://mgt.dev)
- Задайте вопрос на [сайте Stack Overflow.](https://aka.ms/mgt-question)
- Сообщать об ошибках или оставлять запросы на функции на [GitHub.](https://aka.ms/mgt)