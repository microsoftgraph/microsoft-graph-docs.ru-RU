---
title: Настраиваемый поставщик
description: Создайте настраиваемый поставщик, чтобы включить проверку подлинности и доступ к Microsoft Graph для компонентов Microsoft Graph Toolkit при наличии существующего кода проверки подлинности в вашем приложении.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 4327bea637043fa8280bf6c39f55cdb8a0333b1c529f4994e9c8273ff0e3d99b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54204928"
---
# <a name="custom-provider"></a>Настраиваемый поставщик

Если в вашем приложении есть существующий код проверки подлинности, вы можете создать настраиваемый поставщик, чтобы включить проверку подлинности и доступ к Microsoft Graph для компонентов Microsoft Graph Toolkit. Создать настраиваемых поставщиков можно двумя способами:

- Создать новый класс `SimpleProvider`, передав функцию для получения маркера доступа
- Расширить абстрактный класс `IProvider`

В этой статье подробно описан каждый из подходов.

## <a name="simpleprovider"></a>SimpleProvider

Создайте экземпляр класса `SimpleProvider`, передав функцию, которая вернет маркер доступа для переданных областей. 

```ts
let provider = new SimpleProvider((scopes: string[]) => {
  // return a promise with accessToken
});
```

Кроме того, вы также можете предоставить необязательные функции `login` и `logout`, которые могут обрабатывать вызовы входа и выхода из компонента [Вход](../components/login.md).

> [!IMPORTANT] 
> Чтобы указать компонентам, что они могут начать вызов API Microsoft Graph после успешного входа пользователя, необходимо вызвать `Providers.setState(ProviderState.SignedIn)`. Пример показан в функции `login` ниже.

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

Чтобы компоненты знали состояние поставщика, следует вызывать метод `provider.setState(state: ProviderState)` при любом изменении состояния. Например, когда пользователь вошел, вызовите`provider.setState(ProviderState.SignedIn)`. Как показано, перечисление `ProviderState` определяет три состояния.

```ts
export enum ProviderState {
  Loading,
  SignedOut,
  SignedIn
}
```

## <a name="iprovider"></a>IProvider

Вы можете расширить абстрактный класс `IProvider`, чтобы создать собственный поставщик.

### <a name="state"></a>Состояние

Поставщик должен следить за состоянием проверки подлинности и обновлять компоненты при изменении состояния. Класс `IProvider` уже реализует обработчик `onStateChanged(eventHandler)` и свойство `state: ProviderState`. Вам просто нужно использовать метод `setState(state:ProviderState)` в реализации, чтобы обновить состояние, когда оно изменится. При обновлении состояния будет вызвано событие `stateChanged` и автоматически обновлены все компоненты.

### <a name="loginlogout"></a>Вход/Выход

Если поставщик предоставляет функцию входа или выхода, реализуйте методы `login(): Promise<void>` и `logout(): Promise<void>`. Эти методы являются необязательными.

### <a name="access-token"></a>Маркер доступа

Необходимо реализовать метод `getAccessToken({'scopes': scopes[]}) : Promise<string>`. Этот метод используется для получения допустимого маркера перед каждым вызовом Microsoft Graph.

### <a name="graph"></a>Microsoft Graph

Компоненты используют пакет SDK Microsoft Graph для JavaScript для всех вызовов Microsoft Graph. Поставщик должен сделать пакет SDK доступным с помощью свойства `graph`. Создайте в конструкторе новый экземпляр `Graph`, как показано.

```js
this.graph = new Graph(this);
```

Класс `Graph` — это легкая оболочка поверх пакета SDK Microsoft Graph.

### <a name="example"></a>Пример

Все поставщики расширяют абстрактный класс `IProvider`. Например, посмотрите на исходный код для любого из [существующих поставщиков](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/main/packages/mgt/src/providers).

## <a name="set-the-global-provider"></a>Настройка глобального поставщика

Компоненты используют свойство `Providers.globalProvider` для доступа к поставщику. После создания собственного поставщика, задайте это свойство для него.

```ts
import { Providers } from '@microsoft/mgt';

Providers.globalProvider = myProvider;
```

Все компоненты будут уведомлены о новом поставщике и начнут его использовать.
