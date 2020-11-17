---
title: Настраиваемый поставщик
description: Создайте настраиваемый поставщик, чтобы включить проверку подлинности и доступ к Graph для компонентов набора средств Microsoft Graph, если в вашем приложении есть код проверки подлинности.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 57b7ca843f71d22992df18dc2466d0182d3fc556
ms.sourcegitcommit: 186d738f04e5a558da423f2429165fb4fbe780aa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086601"
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

> [!IMPORTANT] 
> Чтобы указать компоненты, которые они могут начать вызывать API Microsoft Graph после успешного входа пользователя, необходимо позвонить `Providers.setState(ProviderState.SignedIn)` . Пример такой функции показан в `login` приведенной ниже функции.

```ts
function getAccessToken(scopes: string[]) {
  // return a promise with accessToken string
}

function login() {
  //login code
  Providers.globalProvider.setState(ProviderState.SignedIn)
}

function logout() {
  // logout code
}

let provider = new SimpleProvider(getAccessToken, login, logout);
```

### <a name="manage-state"></a>Управление состоянием

Чтобы компоненты могли знать о состоянии поставщика, необходимо вызвать `provider.setState(state: ProviderState)` метод при изменении состояния. Например, если пользователь выполнил вход, вызовите `provider.setState(ProviderState.SignedIn)` . `ProviderState`Перечисление определяет три состояния, как показано ниже.

```ts
export enum ProviderState {
  Loading,
  SignedOut,
  SignedIn
}
```

## <a name="iprovider"></a>ипровидер

`IProvider`Абстрактный класс можно расширить для создания собственного поставщика.

### <a name="state"></a>Состояние

Поставщик должен отслеживать состояние проверки подлинности и обновлять компоненты при изменении состояния. `IProvider`Класс уже реализует `onStateChanged(eventHandler)` обработчик и `state: ProviderState` свойство. Для `setState(state:ProviderState)` обновления состояния при изменении состояния необходимо просто использовать метод в реализации. При обновлении состояния событие будет срабатывать `stateChanged` и автоматически обновлены все компоненты.

### <a name="loginlogout"></a>Вход/выход

Если поставщик предоставляет функции входа или выхода, реализуйте `login(): Promise<void>` методы и `logout(): Promise<void>` . Эти методы являются необязательными.

### <a name="access-token"></a>Маркер доступа

Необходимо реализовать `getAccessToken({'scopes': scopes[]}) : Promise<string>` метод. Этот метод используется для получения действительного маркера перед каждым вызовом Microsoft Graph.

### <a name="graph"></a>Graph

Компоненты используют пакет SDK JavaScript для Microsoft Graph для всех вызовов Microsoft Graph. Поставщик должен предоставить пакет SDK, доступный через `graph` свойство. В конструкторе создайте новый `Graph` экземпляр, как показано ниже.

```js
this.graph = new Graph(this);
```

Этот `Graph` класс представляет собой тонкую обертку на основе пакета SDK Microsoft Graph.

### <a name="example"></a>Пример

Все поставщики расширяют `IProvider` абстрактный класс. В качестве примера рассмотрим исходный код для любого из [существующих поставщиков](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/main/packages/mgt/src/providers).

## <a name="set-the-global-provider"></a>Настройка глобального поставщика

Компоненты используют `Providers.globalProvider` свойство для доступа к поставщику. После создания собственного поставщика задайте этому свойству поставщика.

```ts
import { Providers } from '@microsoft/mgt';

Providers.globalProvider = myProvider;
```

Все компоненты будут уведомлены о новом поставщике и приступить к его использованию.
