---
title: Создание веб-приложения с помощью Microsoft Graph Toolkit
description: Знакомство с разработкой веб-приложений с помощью Microsoft Graph Toolkit
ms.localizationpriority: medium
author: elisenyang
ms.openlocfilehash: 22f5e81f8c382694389ddcffbe5e0f8a77fa55a9
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59103839"
---
# <a name="build-a-web-application-with-the-microsoft-graph-toolkit"></a>Создание веб-приложения с помощью Microsoft Graph Toolkit

В этом разделе описывается, как начать работу с Microsoft Graph Toolkit в веб-приложении, написанном на простом JavaScript. В пошаговом руководстве попробуйте начать работу с модулем [Microsoft Graph набор средств.](/learn/modules/msgraph-toolkit-intro/) Чтобы узнать, как использовать Toolkit в веб-среде, см. статью [Создание веб-приложения (React)](./use-toolkit-with-react.md) или [Создание веб-приложения (Angular)](./use-toolkit-with-angular.md).

Начало работы с Microsoft Graph Toolkit включает:
1. Добавление Microsoft Graph Toolkit в проект.
2. Инициализация поставщика MSAL2.
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

## <a name="initialize-the-msal2-provider"></a>Инициализация поставщика MSAL2
Поставщики Microsoft Graph Toolkit обеспечивают проверку подлинности и доступ к Microsoft Graph для компонентов. Дополнительные сведения см. в статье [Использование поставщиков](../providers/providers.md). Поставщик [MSAL2 использует](../providers/msal2.md) msal-browser для регистрации пользователей и приобретения маркеров. Этот поставщик можно инициализировать в HTML или JavaScript.

> **Примечание.** Если вы в настоящее время используете поставщика MSAL и хотите обновить ее до поставщика MSAL2, выполните указанные [здесь действия.](../providers/msal2.md#migrating-from-msal-provider-to-msal2-provider)
Если вы хотите использовать собственную проверку подлинности, используйте поставщика прокси-серверов [на](../providers/proxy.md) месте поставщика MSAL2.

Чтобы инициализировать поставщика, можно использовать HTML-код или JavaScript. 

# <a name="html"></a>[HTML](#tab/HTML)
Добавьте компонент `mgt-msal2-provider` на HTML-страницу и задайте `client-id` для идентификатора клиента приложения.

```html
<mgt-msal2-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal2-provider>
```
# <a name="javascript"></a>[JavaScript](#tab/JavaScript)
Чтобы инициализировать поставщика MSAL в JavaScript, добавьте следующий код в приложение:

```javascript
import { Providers, Msal2Provider } from '@microsoft/mgt';

Providers.globalProvider = new Msal2Provider({
  clientId: "<YOUR_CLIENT_ID>"
});
```

---

Идентификатор клиента — это единственное свойство, которое требуется для инициализации поставщика, но вы можете настроить дополнительные параметры. Полный список см. в [списке MSAL2 Provider.](../providers/msal2.md)

### <a name="creating-an-appclient-id"></a>Создание идентификатора клиента/приложения
Чтобы получить идентификатор клиента, вам нужно [зарегистрировать свое приложение](./add-aad-app-registration.md) в Azure AD.

## <a name="add-components"></a>Добавление компонентов
После инициализации поставщика MSAL2 можно начать использовать любой из набор средств компонентов.

# <a name="html"></a>[HTML](#tab/HTML)
Ниже приводится полный рабочий пример с использованием mgt-loader, поставщика MSAL2, инициализированного в HTML-коде, и компонента Login:

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal2-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal2-provider>
<mgt-login></mgt-login>
```

Это пример с помощью модулей ES6, поставщика MSAL2, инициализированного в HTML-коде, и компонента Login:

```html
<script type="module" src="node_modules/@microsoft/mgt/dist/es6/index.js"></script>
<mgt-msal2-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal2-provider>
<mgt-login></mgt-login>
```

# <a name="javascript"></a>[JavaScript](#tab/JavaScript)
Это пример с помощью модулей ES6, поставщика MSAL2, инициализированного в JavaScript, и компонента Login:

```javascript
import { Providers, Msal2Provider } from '@microsoft/mgt';

Providers.globalProvider = new Msal2Provider({
  clientId: "<YOUR_CLIENT_ID>"
});

function component() {
  const element = document.createElement('div');
  element.innerHTML = '<mgt-login></mgt-login>';
  return element;
}

document.body.appendChild(component());
```

---

## <a name="test-your-app"></a>Тестирование приложения

Чтобы протестировать приложение, MSAL требует, чтобы страница была размещена на веб-сервере для перенаправления проверки подлинности. 

Если вы только начинаете работать и хотите поэкспериментировать с, можно использовать [Динамический сервер](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) в Visual Studio Code или на любом похожем сервере облегченной разработки. Скачайте расширение и откройте HTML-файл с помощью динамического сервера.
> **Примечание.** Убедитесь в том, что **URI перенаправления** в приложении регистрации настроен на порт localhost, на котором размещено приложение. Перейдите в службу регистрации приложения на [портале Azure](https://portal.azure.com), в разделе управления выберите пункт **Проверка подлинности**, и укажите соответствующий **URI перенаправления**.

## <a name="track-a-users-sign-in-state"></a>Отслеживание знака пользователя в состоянии

Вы можете определить, когда пользователь успешно вписался и соответствующим образом отображает определенные компоненты. Например, отобразить компонент повестки дня, если пользователь в него вписалась. В противном случае отобразить знак в интерфейсе.

Чтобы правильно проверить вход пользователя в состояние, добавьте обработник событий `providerUpdated` в событие с помощью `Providers.onProviderUpdated` функции. В обработнике проверьте состояние поставщика, хранимое в `Providers.globalProvider.state` свойстве.

# <a name="html"></a>[HTML](#tab/HTML)

Если вы используете библиотеку, вы можете получить доступ к глобальному свойству и `mgt-loader` `Provider` из `ProviderState` `mgt` него.

```html
<!DOCTYPE html>
<html>
<head>
  <script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
</head>
<body>
  <mgt-msal2-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal2-provider>
  <div id="main">
    <mgt-login></mgt-login>
  </div>
  <script>
    const loadAgenda = () => {
      if (mgt.Providers.globalProvider.state === mgt.ProviderState.SignedIn) {
        document.getElementById('main').innerHTML = '<mgt-agenda></mgt-agenda>';
      }
    }
    mgt.Providers.onProviderUpdated(loadAgenda);
  </script>
</body>
</html>
```

# <a name="javascript"></a>[JavaScript](#tab/JavaScript)

Если вы используете набор инструментов с помощью пакетов npm, вы можете импортировать и `Provider` `ProviderState` из `@microsoft/mgt` .

```javascript
import { Providers, ProviderState, Msal2Provider } from '@microsoft/mgt';

Providers.globalProvider = new Msal2Provider({
  clientId: "<YOUR_CLIENT_ID>"
});

const loadAgenda = () => {
  if (Providers.globalProvider.state === ProviderState.SignedIn) {
    document.getElementById('main').innerHTML = '<mgt-agenda></mgt-agenda>';
  }
};

Providers.onProviderUpdated(loadAgenda);
```

---

## <a name="next-steps"></a>Дальнейшие действия

- Ознакомьтесь с [пошаговой](/learn/modules/msgraph-toolkit-intro/) инструкцией по началу Graph набор средств Microsoft.
- Воспользуйтесь компонентами в [интерактивной среде](https://mgt.dev).
- Задавайте вопросы на сайте [Stack Overflow](https://aka.ms/mgt-question).
- Сообщайте об ошибках и оставляйте запросы на создание функций в [GitHub](https://aka.ms/mgt).
