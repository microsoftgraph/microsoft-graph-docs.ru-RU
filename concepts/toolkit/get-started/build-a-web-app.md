---
title: Создание веб-приложения с помощью набора средств Microsoft Graph
description: Приступая к созданию веб-приложения с помощью набора средств Microsoft Graph.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: 6852351e39aa3754ba7458bfe6fe5cd45f5cf635
ms.sourcegitcommit: 3fbc2249b307e8d3a9de18f22ef6911094ca272c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2020
ms.locfileid: "48288533"
---
# <a name="build-a-web-application-with-the-microsoft-graph-toolkit"></a>Создание веб-приложения с помощью набора средств Microsoft Graph

В этом разделе описывается, как приступить к работе с набором инструментов Microsoft Graph в веб-приложении, написанном на Ванилла JavaScript. Если вы хотите узнать, как использовать набор средств с Web Framework, ознакомьтесь со статьей [Использование набора инструментов с Подкликом](./use-toolkit-with-react.md) или [Использование набора инструментов с угловой](./use-toolkit-with-angular.md)страницей.

Начало работы с набором средств Microsoft Graph состоит из следующих этапов:
1. Добавление набора инструментов Microsoft Graph в проект.
2. Инициализация поставщика MSAL.
3. Добавление компонентов.
4. Протестируйте приложение.

## <a name="add-the-microsoft-graph-toolkit-to-your-project"></a>Добавление набора инструментов Microsoft Graph в проект
Вы можете использовать набор средств Microsoft Graph в приложении, обратившись непосредственно к загрузчику (через унпкг) или установив пакет NPM.

### <a name="use-via-mgt-loader"></a>Использование с помощью упр. загрузчиком
Чтобы использовать набор средств с помощью элемента управления "центр управления", добавьте ссылку в скрипт в код:

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
```

### <a name="use-via-npm-es6-modules"></a>Использование через NPM (модули ES6)
Использование набора средств с помощью модулей ES6 даст вам полный контроль над процессом создания пучка и позволяет объединить только код, который требуется для приложения. Чтобы использовать модули ES6, добавьте в проект пакет NPM:

```bash
npm install @microsoft/mgt
```
> **Note**: Если вы используете браузер, например IE11, который не поддерживает встроенные веб-компоненты, вам может потребоваться включить знаки, которые можно [включить](./overview.md#polyfills)в набор.

Теперь вы можете ссылаться на все компоненты набора инструментов в приложении с помощью следующих компонентов:

```html
<script src="node_modules/@microsoft/mgt/dist/es6/components.js"></script>
```
Кроме того, следует ссылаться только на необходимые компоненты и не загружать все остальные. Например, чтобы добавить поставщика MSAL:

```html
<script src="node_modules/@microsoft/mgt/dist/es6/components/providers/mgt-msal-provider.js"></script>
```

## <a name="initialize-the-msal-provider"></a>Инициализация поставщика MSAL
Поставщики набора средств Microsoft Graph обеспечивают проверку подлинности и доступ к Microsoft Graph для компонентов. Чтобы узнать больше, ознакомьтесь со статьей [Использование поставщиков](../providers.md). [Поставщик MSAL](../providers/msal.md) использует MSAL.js для входа пользователей и получения маркеров. Вы можете инициализировать поставщик MSAL в HTML или JavaScript.

Если вы хотите использовать собственную серверную проверку подлинности, используйте [поставщика прокси-сервера](../providers/proxy.md) вместо поставщика MSAL.

Для инициализации поставщика можно использовать HTML-код или код JavaScript. 

### <a name="initialize-in-your-html-page"></a>Инициализация на HTML-странице
Добавьте `mgt-msal-provider` компонент на HTML-страницу и задайте для него значение `client-id` Client ID.

```html
<mgt-msal-provider client-id="<YOUR_CLIENT_ID"></mgt-msal-provider>
```
### <a name="initialize-in-javascript"></a>Инициализация в JavaScript
Чтобы инициализировать поставщик MSAL в коде JavaScript, добавьте в приложение следующий код:

```js
import {Providers, MsalProvider} from '@microsoft/mgt'

Providers.globalProvider = new MsalProvider({
    clientId: "<YOUR_CLIENT_ID>"
})
```
Единственным свойством, необходимым для инициализации поставщика, является идентификатор клиента, но вы можете задать дополнительные параметры. Полный список можно найти в разделе [поставщик Msal](../providers/msal.md).

### <a name="creating-an-appclient-id"></a>Создание идентификатора приложения или клиента
Чтобы получить идентификатор клиента, необходимо [зарегистрировать приложение](../../auth-register-app-v2.md) в Azure AD. 
>**Note**: MSAL поддерживает только неявный поток для OAuth. Не забудьте включить неявный поток в приложении на портале Azure (по умолчанию он не включен). В разделе **Проверка подлинности**найдите раздел **неявный предоставление** и установите флажки для **маркеров доступа** и **маркеров ID**. 

## <a name="add-components"></a>Добавление компонентов
После инициализации поставщика MSAL можно приступить к использованию любого из компонентов набора средств.

Ниже приведен полный рабочий пример с помощью элемента упр-Loader, поставщика MSAL, инициализированного в HTML, и компонента входа:

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal-provider>
<mgt-login></mgt-login>
```

В этом примере используются модули ES6, поставщик MSAL, инициализированный в HTML, и компонент входа:
```html
<script src="node_modules/@microsoft/mgt/dist/es6/components/providers/mgt-msal-provider.js"></script>
<script src="node_modules/@microsoft/mgt/dist/es6/components/mgt-login/mgt-login.js"></script>
<mgt-msal-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal-provider>
<mgt-login></mgt-login>
```

В этом примере используются модули ES6, поставщик MSAL, инициализированный в JavaScript, и компонент входа:

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

## <a name="test-your-app"></a>Тестирование приложения

Чтобы протестировать приложение, для MSAL требуется, чтобы страница была размещена на веб-сервере для перенаправления проверки подлинности. 

Если вы только начинаете работать и хотите поиграть, вы можете использовать [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) в Visual Studio Code или на любом аналогичном сервере облегченного развертывания. Скачайте расширение и откройте HTML-файл с помощью Live Server. 
> **Примечание:** Убедитесь, что **URI перенаправления** в регистрации приложения настроен на порт localhost, на котором размещено приложение. Перейдите к регистрации приложения на [портале Azure](https://portal.azure.com), щелкните **Проверка подлинности** в разделе Управление и добавьте правильный **URI перенаправления**.

## <a name="next-steps"></a>Дальнейшие действия
- Ознакомьтесь с пошаговыми руководствами по [созданию простого веб-приложения](https://developer.microsoft.com/microsoft-365/blogs/a-lap-around-microsoft-graph-toolkit-day-2-zero-to-hero/).
- Опробуйте компоненты в [интерактивная среда](https://mgt.dev).
- Задайте вопрос о [переполнении стека](https://aka.ms/mgt-question).
- Сообщать об ошибках или оставлять запрос на функцию в [GitHub](https://aka.ms/mgt).