---
title: Создание веб-приложения с помощью Microsoft Graph Toolkit
description: Знакомство с разработкой веб-приложений с помощью Microsoft Graph Toolkit
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: 73e61e9d2c1c453ec67e61dce1f088b5119d1e8d
ms.sourcegitcommit: 7902607a1e5a030d46e907d08e16644a47a47006
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/12/2020
ms.locfileid: "49664018"
---
# <a name="build-a-web-application-with-the-microsoft-graph-toolkit"></a>Создание веб-приложения с помощью Microsoft Graph Toolkit

В этом разделе описывается, как начать работу с Microsoft Graph Toolkit в веб-приложении, написанном на простом JavaScript. Чтобы узнать, как использовать Toolkit в веб-среде, см. статью [Создание веб-приложения (React)](./use-toolkit-with-react.md) или [Создание веб-приложения (Angular)](./use-toolkit-with-angular.md).

Начало работы с Microsoft Graph Toolkit включает:
1. Добавление Microsoft Graph Toolkit в проект.
2. Инициализация поставщика MSAL.
3. Добавление компонентов.
4. Тестирование приложения.

## <a name="add-the-microsoft-graph-toolkit-to-your-project"></a>Добавление Microsoft Graph Toolkit в проект
Используйте Microsoft Graph Toolkit в приложении, обратившись непосредственно к загрузчику (через unpkg) или установив пакет npm.

# <a name="unpkg"></a>[unpkg](#tab/html)
Чтобы использовать Toolkit в загрузчике Microsoft Graph Toolkit, добавьте ссылку в сценарий кода:

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
```
# <a name="npm"></a>[npm](#tab/npm)
Использование Toolkit с помощью модулей ES6 обеспечивает полное управление процессом объединения и позволяет объединить только код, необходимый для приложения. Чтобы использовать модули ES6, добавьте в проект пакет npm:

```cmd
npm install @microsoft/mgt
```

---


> **Примечание**. Если вы ориентируетесь на браузер, например IE11, который изначально не поддерживает веб-компоненты, потребуется [включить полизаполнение](./overview.md#polyfills).

## <a name="initialize-the-msal-provider"></a>Инициализация поставщика MSAL
Поставщики Microsoft Graph Toolkit обеспечивают проверку подлинности и доступ к Microsoft Graph для компонентов. Дополнительные сведения см. в статье [Использование поставщиков](../providers/providers.md). [Поставщик MSAL](../providers/msal.md) использует MSAL.js для входа в систему и получения маркеров. Поставщика MSAL можно инициализировать в HTML-коде или JavaScript.

Чтобы использовать собственную внутреннюю проверку подлинности, используйте [Поставщик прокси-сервера](../providers/proxy.md) вместо поставщика MSAL.

Чтобы инициализировать поставщика, можно использовать HTML-код или JavaScript. 

# <a name="html"></a>[html](#tab/HTML)
Добавьте компонент `mgt-msal-provider` на HTML-страницу и задайте `client-id` для идентификатора клиента приложения.

```html
<mgt-msal-provider client-id="<YOUR_CLIENT_ID"></mgt-msal-provider>
```
# <a name="js"></a>[js](#tab/JavaScript)
Чтобы инициализировать поставщика MSAL в JavaScript, добавьте следующий код в приложение:

```js
import {Providers, MsalProvider} from '@microsoft/mgt'

Providers.globalProvider = new MsalProvider({
    clientId: "<YOUR_CLIENT_ID>"
})
```

---


Идентификатор клиента — это единственное свойство, которое требуется для инициализации поставщика, но вы можете настроить дополнительные параметры. Полный список см. в статье [Поставщик Msal](../providers/msal.md).

### <a name="creating-an-appclient-id"></a>Создание идентификатора клиента/приложения
Чтобы получить идентификатор клиента, вам нужно [зарегистрировать свое приложение](./add-aad-app-registration.md) в Azure AD. 
>**Примечание**. MSAL поддерживает только неявный поток для OAuth. Включите неявный поток в своем приложении на портале Azure (он не включен по умолчанию). В области **Проверка подлинности** найдите раздел **Неявное предоставление** и установите флажки **Маркеры доступа** и **Маркеры идентификаторов**. 

## <a name="add-components"></a>Добавление компонентов
После инициализации поставщика MSAL можно приступить к работе с любыми компонентами Toolkit.

# <a name="html"></a>[html](#tab/HTML)
Ниже приведен рабочий пример с использованием загрузчика Microsoft Graph Toolkit, поставщика MSAL, инициализированного в HTML, и компонента входа в систему:

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal-provider>
<mgt-login></mgt-login>
```

Пример использования модулей ES6, поставщика MSAL, инициализированного в HTML, и компонента входа в систему:

```html
<script type="module" src="node_modules/@microsoft/mgt/dist/es6/index.js"></script>

<mgt-msal-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal-provider>

<mgt-login></mgt-login>
```
# <a name="js"></a>[js](#tab/JavaScript)
Пример использования модулей ES6, поставщика MSAL, инициализированного в JavaScript, и компонента входа в систему:

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

Чтобы протестировать приложение, MSAL требует, чтобы страница была размещена на веб-сервере для перенаправления проверки подлинности. 

Если вы только начинаете работать и хотите поэкспериментировать с, можно использовать [Динамический сервер](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) в Visual Studio Code или на любом похожем сервере облегченной разработки. Скачайте расширение и откройте HTML-файл с помощью динамического сервера. 
> **Примечание.** Убедитесь в том, что **URI перенаправления** в приложении регистрации настроен на порт localhost, на котором размещено приложение. Перейдите в службу регистрации приложения на [портале Azure](https://portal.azure.com), в разделе управления выберите пункт **Проверка подлинности**, и укажите соответствующий **URI перенаправления**.

## <a name="next-steps"></a>Дальнейшие действия
- Ознакомьтесь с пошаговыми инструкциями для [создания простого веб-приложения](https://developer.microsoft.com/microsoft-365/blogs/a-lap-around-microsoft-graph-toolkit-day-2-zero-to-hero/).
- Воспользуйтесь компонентами в [интерактивной среде](https://mgt.dev).
- Задавайте вопросы на сайте [Stack Overflow](https://aka.ms/mgt-question).
- Сообщайте об ошибках и оставляйте запросы на создание функций в [GitHub](https://aka.ms/mgt).