---
title: Создание веб-приложения с помощью Microsoft Graph Toolkit
description: Знакомство с разработкой веб-приложений с помощью Microsoft Graph Toolkit
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: 9890a042ce08533ce17c014a0815f1f63dbfdd46739f4f4af284bf87706124d4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54236859"
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

## <a name="initialize-the-msal-20-provider"></a>Инициализация поставщика MSAL 2.0
Поставщики Microsoft Graph Toolkit обеспечивают проверку подлинности и доступ к Microsoft Graph для компонентов. Дополнительные сведения см. в статье [Использование поставщиков](../providers/providers.md). Поставщик [MSAL 2.0](../providers/msal2.md) использует msal-browser для регистрации пользователей и приобретения маркеров. Этот поставщик можно инициализировать в HTML или JavaScript.

> **Примечание.** Если вы в настоящее время используете поставщика MSAL и хотите обновить до поставщика MSAL 2.0, выполните указанные [здесь действия.](../providers/msal2.md#migrating-from-msal-provider-to-msal-2-provider)
Если вы хотите использовать собственную проверку подлинности, используйте поставщика прокси-серверов на месте поставщика MSAL 2.0. [](../providers/proxy.md)

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

Идентификатор клиента — это единственное свойство, которое требуется для инициализации поставщика, но вы можете настроить дополнительные параметры. Полный список см. в [списке Msal 2.0 Provider](../providers/msal2.md).

### <a name="creating-an-appclient-id"></a>Создание идентификатора клиента/приложения
Чтобы получить идентификатор клиента, вам нужно [зарегистрировать свое приложение](./add-aad-app-registration.md) в Azure AD.

## <a name="add-components"></a>Добавление компонентов
После инициализации поставщика MSAL 2.0 можно начать использовать любой из набор средств компонентов.

# <a name="html"></a>[HTML](#tab/HTML)
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

# <a name="javascript"></a>[JavaScript](#tab/JavaScript)
Это пример с помощью модулей ES6, поставщика MSAL 2.0, инициализированного в JavaScript, и компонента Login:

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
