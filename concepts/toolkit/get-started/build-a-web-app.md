---
title: Создание веб-приложения с помощью Microsoft Graph Toolkit
description: Знакомство с разработкой веб-приложений с помощью Microsoft Graph Toolkit
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: 5eed45974428a2c6daf47d02144741d937e12c91
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579902"
---
# <a name="build-a-web-application-with-the-microsoft-graph-toolkit"></a>Создание веб-приложения с помощью Microsoft Graph Toolkit

В этом разделе описывается, как начать работу с Microsoft Graph Toolkit в веб-приложении, написанном на простом JavaScript. В пошаговом руководстве попробуйте начать работу с модулем [Microsoft Graph набор средств.](/learn/modules/msgraph-toolkit-intro/) Чтобы узнать, как использовать Toolkit в веб-среде, см. статью [Создание веб-приложения (React)](./use-toolkit-with-react.md) или [Создание веб-приложения (Angular)](./use-toolkit-with-angular.md).

Начало работы с Microsoft Graph Toolkit включает:
1. Добавление Microsoft Graph Toolkit в проект.
2. Инициализация поставщика MSAL 2.0.
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

## <a name="initialize-the-msal-20-provider"></a>Инициализация поставщика MSAL 2.0
Поставщики Microsoft Graph Toolkit обеспечивают проверку подлинности и доступ к Microsoft Graph для компонентов. Дополнительные сведения см. в статье [Использование поставщиков](../providers/providers.md). Поставщик [MSAL 2.0](../providers/msal2.md) использует msal-browser для регистрации пользователей и приобретения маркеров. Этот поставщик можно инициализировать в HTML или JavaScript.

> **Примечание.** Если вы в настоящее время используете поставщика MSAL и хотите обновить до поставщика MSAL 2.0, выполните указанные [здесь действия.](../providers/msal2.md#migrating-from-msal-provider-to-msal-2-provider)
Если вы хотите использовать собственную проверку подлинности, используйте поставщика прокси-серверов на месте поставщика MSAL 2.0. [](../providers/proxy.md)

Чтобы инициализировать поставщика, можно использовать HTML-код или JavaScript. 

# <a name="html"></a>[html](#tab/HTML)
Добавьте компонент `mgt-msal2-provider` на HTML-страницу и задайте `client-id` для идентификатора клиента приложения.

```html
<mgt-msal2-provider client-id="<YOUR_CLIENT_ID"></mgt-msal2-provider>
```
# <a name="js"></a>[js](#tab/JavaScript)
Чтобы инициализировать поставщика MSAL в JavaScript, добавьте следующий код в приложение:

```js
import {Providers, Msal2Provider} from '@microsoft/mgt'

Providers.globalProvider = new Msal2Provider({
    clientId: "<YOUR_CLIENT_ID>"
})
```

---


Идентификатор клиента — это единственное свойство, которое требуется для инициализации поставщика, но вы можете настроить дополнительные параметры. Полный список см. в [списке Msal 2.0 Provider](../providers/msal2.md).

### <a name="creating-an-appclient-id"></a>Создание идентификатора клиента/приложения
Чтобы получить идентификатор клиента, вам нужно [зарегистрировать свое приложение](./add-aad-app-registration.md) в Azure AD. 

## <a name="add-components"></a>Добавление компонентов
После инициализации поставщика MSAL 2.0 можно начать использовать любой из набор средств компонентов.

# <a name="html"></a>[html](#tab/HTML)
Ниже приведен рабочий пример с использованием загрузчика Microsoft Graph Toolkit, поставщика MSAL, инициализированного в HTML, и компонента входа в систему:

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal2-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal2-provider>
<mgt-login></mgt-login>
```

Это пример с использованием модулей ES6, поставщика MSAL 2.0, инициализированного в HTML-коде, и компонента Login:

```html
<script type="module" src="node_modules/@microsoft/mgt/dist/es6/index.js"></script>

<mgt-msal2-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal2-provider>

<mgt-login></mgt-login>
```
# <a name="js"></a>[js](#tab/JavaScript)
Это пример с помощью модулей ES6, поставщика MSAL 2.0, инициализированного в JavaScript, и компонента Login:

```js
import {Providers, Msal2Provider} from '@microsoft/mgt'

Providers.globalProvider = new Msal2Provider({
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
- Ознакомьтесь с [пошаговой](/learn/modules/msgraph-toolkit-intro/) инструкцией по началу Graph набор средств Microsoft.
- Воспользуйтесь компонентами в [интерактивной среде](https://mgt.dev).
- Задавайте вопросы на сайте [Stack Overflow](https://aka.ms/mgt-question).
- Сообщайте об ошибках и оставляйте запросы на создание функций в [GitHub](https://aka.ms/mgt).
