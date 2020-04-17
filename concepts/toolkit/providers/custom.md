---
title: Настраиваемый поставщик
description: Создайте настраиваемый поставщик, чтобы включить проверку подлинности и доступ к Graph для компонентов набора средств Microsoft Graph, если в вашем приложении есть код проверки подлинности.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: acd96e6dc7e13b1e1fbfc5353e3db2132a23e246
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2019
ms.locfileid: "35243081"
---
# <a name="custom-provider"></a>Настраиваемый поставщик

Если в вашем приложении есть код проверки подлинности, вы можете создать настраиваемый поставщик, чтобы включить проверку подлинности и доступ к Microsoft Graph для компонентов набора инструментов Microsoft Graph. Существует два способа создания настраиваемых поставщиков:

- Создание нового `SimpleProvider` путем передачи функции для получения маркера доступа
- Расширение `IProvider` абстрактного класса

В этой статье каждый из этих способов описывается более подробно.

## <a name="simpleprovider"></a>симплепровидер

Создайте экземпляр `SimpleProvider` класса, передав функцию, которая будет возвращать маркер доступа для переданных областей.

```ts
let provider = new SimpleProvider((scopes: string[]) => {
  // return a promise with accessToken
});
```

Кроме того, вы также можете указать дополнительные `login` функции и `logout` функции, которые могут обрабатывать вызовы входа и выхода из компонента [Login](../components/login.md) .

```ts
function getAccessToken(scopes: string[]) {
  // return a promise with accessToken string
}

function login() {
  // login code
}

function logout() {
  // logout code
}

let provider = new SimpleProvider(getAccessToken, login, logout);
```

### <a name="manage-state"></a>Управление состоянием

Чтобы компоненты могли знать о состоянии поставщика, необходимо вызвать `provider.setState(state: ProviderState)` метод при изменении состояния. Например, если пользователь выполнил вход, вызовите `provider.setState(ProviderState.SignedIn)`. `ProviderState` Перечисление определяет три состояния, как показано ниже.

```ts
export enum ProviderState {
  Loading,
  SignedOut,
  SignedIn
}
```

## <a name="iprovider"></a>ипровидер

`IProvider` Абстрактный класс можно расширить для создания собственного поставщика.

### <a name="state"></a>Состояние

Поставщик должен отслеживать состояние проверки подлинности и обновлять компоненты при изменении состояния. `IProvider` Класс уже реализует `onStateChanged(eventHandler)` обработчик и `state: ProviderState` свойство. Для обновления состояния при изменении состояния `setState(state:ProviderState)` необходимо просто использовать метод в реализации. При обновлении состояния `stateChanged` событие будет срабатывать и автоматически обновлены все компоненты.

### <a name="loginlogout"></a>Вход/выход

Если поставщик предоставляет функции входа или выхода, реализуйте методы `login(): Promise<void>` и `logout(): Promise<void>` . Эти методы являются необязательными.

### <a name="access-token"></a>Маркер доступа

Необходимо реализовать `getAccessToken({'scopes': scopes[]}) : Promise<string>` метод. Этот метод используется для получения действительного маркера перед каждым вызовом Microsoft Graph.

### <a name="graph"></a>Graph

Компоненты используют пакет SDK JavaScript для Microsoft Graph для всех вызовов Microsoft Graph. Поставщик должен предоставить пакет SDK, доступный через `graph` свойство. В конструкторе создайте новый `Graph` экземпляр, как показано ниже.

```js
this.graph = new Graph(this);
```

Этот `Graph` класс представляет собой тонкую обертку на основе пакета SDK Microsoft Graph.

### <a name="example"></a>Пример

Все поставщики расширяют `IProvider` абстрактный класс. В качестве примера рассмотрим исходный код для любого из [существующих поставщиков](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/src/providers).

## <a name="set-the-global-provider"></a>Настройка глобального поставщика

Компоненты используют `Providers.globalProvider` свойство для доступа к поставщику. После создания собственного поставщика задайте этому свойству поставщика.

```ts
import { Providers } from '@microsoft/mgt';

Providers.globalProvider = myProvider;
```

Все компоненты будут уведомлены о новом поставщике и приступить к его использованию.
