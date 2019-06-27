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
# <a name="custom-provider"></a><span data-ttu-id="cedca-103">Настраиваемый поставщик</span><span class="sxs-lookup"><span data-stu-id="cedca-103">Custom provider</span></span>

<span data-ttu-id="cedca-104">Если в вашем приложении есть код проверки подлинности, вы можете создать настраиваемый поставщик, чтобы включить проверку подлинности и доступ к Microsoft Graph для компонентов набора инструментов Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="cedca-104">If you have existing authentication code in your application, you can create a custom provider to enable authentication and access to Microsoft Graph for Microsoft Graph Toolkit components.</span></span> <span data-ttu-id="cedca-105">Существует два способа создания настраиваемых поставщиков:</span><span class="sxs-lookup"><span data-stu-id="cedca-105">There are two ways to create custom providers:</span></span>

- <span data-ttu-id="cedca-106">Создание нового `SimpleProvider` путем передачи функции для получения маркера доступа</span><span class="sxs-lookup"><span data-stu-id="cedca-106">Create a new `SimpleProvider` by passing in a function for getting an access token</span></span>
- <span data-ttu-id="cedca-107">Расширение `IProvider` абстрактного класса</span><span class="sxs-lookup"><span data-stu-id="cedca-107">Extend the `IProvider` abstract class</span></span>

<span data-ttu-id="cedca-108">В этой статье каждый из этих способов описывается более подробно.</span><span class="sxs-lookup"><span data-stu-id="cedca-108">This article describes each approach in more detail.</span></span>

## <a name="simpleprovider"></a><span data-ttu-id="cedca-109">Симплепровидер</span><span class="sxs-lookup"><span data-stu-id="cedca-109">SimpleProvider</span></span>

<span data-ttu-id="cedca-110">Создайте экземпляр `SimpleProvider` класса, передав функцию, которая будет возвращать маркер доступа для переданных областей.</span><span class="sxs-lookup"><span data-stu-id="cedca-110">Instantiate the `SimpleProvider` class by passing in a function that will return an access token for passed-in scopes.</span></span>

```ts
let provider = new SimpleProvider((scopes: string[]) => {
  // return a promise with accessToken
});
```

<span data-ttu-id="cedca-111">Кроме того, вы также можете указать дополнительные `login` функции и `logout` функции, которые могут обрабатывать вызовы входа и выхода из компонента [Login](../components/login.md) .</span><span class="sxs-lookup"><span data-stu-id="cedca-111">In addition, you can also provide an optional `login` and `logout` functions that can handle the sign in and sign out calls from the [Login](../components/login.md) component.</span></span>

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

### <a name="manage-state"></a><span data-ttu-id="cedca-112">Управление состоянием</span><span class="sxs-lookup"><span data-stu-id="cedca-112">Manage state</span></span>

<span data-ttu-id="cedca-113">Чтобы компоненты могли знать о состоянии поставщика, необходимо вызвать `provider.setState(state: ProviderState)` метод при изменении состояния.</span><span class="sxs-lookup"><span data-stu-id="cedca-113">For the components to be aware of the state of the provider, you will need to call the `provider.setState(state: ProviderState)` method whenever the state changes.</span></span> <span data-ttu-id="cedca-114">Например, если пользователь выполнил вход, вызовите `provider.setState(ProviderState.SignedIn)`.</span><span class="sxs-lookup"><span data-stu-id="cedca-114">For example, when the user has signed in, call `provider.setState(ProviderState.SignedIn)`.</span></span> <span data-ttu-id="cedca-115">`ProviderState` Перечисление определяет три состояния, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="cedca-115">The `ProviderState` enum defines three states, as shown.</span></span>

```ts
export enum ProviderState {
  Loading,
  SignedOut,
  SignedIn
}
```

## <a name="iprovider"></a><span data-ttu-id="cedca-116">Ипровидер</span><span class="sxs-lookup"><span data-stu-id="cedca-116">IProvider</span></span>

<span data-ttu-id="cedca-117">`IProvider` Абстрактный класс можно расширить для создания собственного поставщика.</span><span class="sxs-lookup"><span data-stu-id="cedca-117">You can extend the `IProvider` abstract class to create your own provider.</span></span>

### <a name="state"></a><span data-ttu-id="cedca-118">Состояние</span><span class="sxs-lookup"><span data-stu-id="cedca-118">State</span></span>

<span data-ttu-id="cedca-119">Поставщик должен отслеживать состояние проверки подлинности и обновлять компоненты при изменении состояния.</span><span class="sxs-lookup"><span data-stu-id="cedca-119">A provider must keep track of the authentication state and update the components when the state changes.</span></span> <span data-ttu-id="cedca-120">`IProvider` Класс уже реализует `onStateChanged(eventHandler)` обработчик и `state: ProviderState` свойство.</span><span class="sxs-lookup"><span data-stu-id="cedca-120">The `IProvider` class already implements the `onStateChanged(eventHandler)` handler and the `state: ProviderState` property.</span></span> <span data-ttu-id="cedca-121">Для обновления состояния при изменении состояния `setState(state:ProviderState)` необходимо просто использовать метод в реализации.</span><span class="sxs-lookup"><span data-stu-id="cedca-121">You just need to use the `setState(state:ProviderState)` method in your implementation to update the state when it changes.</span></span> <span data-ttu-id="cedca-122">При обновлении состояния `stateChanged` событие будет срабатывать и автоматически обновлены все компоненты.</span><span class="sxs-lookup"><span data-stu-id="cedca-122">Updating the state will fire the `stateChanged` event and update all the components automatically.</span></span>

### <a name="loginlogout"></a><span data-ttu-id="cedca-123">Вход/выход</span><span class="sxs-lookup"><span data-stu-id="cedca-123">Login/Logout</span></span>

<span data-ttu-id="cedca-124">Если поставщик предоставляет функции входа или выхода, реализуйте методы `login(): Promise<void>` и `logout(): Promise<void>` .</span><span class="sxs-lookup"><span data-stu-id="cedca-124">If your provider provides login or logout functionality, implement the `login(): Promise<void>` and `logout(): Promise<void>` methods.</span></span> <span data-ttu-id="cedca-125">Эти методы являются необязательными.</span><span class="sxs-lookup"><span data-stu-id="cedca-125">These methods are optional.</span></span>

### <a name="access-token"></a><span data-ttu-id="cedca-126">Маркер доступа</span><span class="sxs-lookup"><span data-stu-id="cedca-126">Access token</span></span>

<span data-ttu-id="cedca-127">Необходимо реализовать `getAccessToken({'scopes': scopes[]}) : Promise<string>` метод.</span><span class="sxs-lookup"><span data-stu-id="cedca-127">You must implement the `getAccessToken({'scopes': scopes[]}) : Promise<string>` method.</span></span> <span data-ttu-id="cedca-128">Этот метод используется для получения действительного маркера перед каждым вызовом Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="cedca-128">This method is used to get a valid token before every call to Microsoft Graph.</span></span>

### <a name="graph"></a><span data-ttu-id="cedca-129">Автоматически</span><span class="sxs-lookup"><span data-stu-id="cedca-129">Graph</span></span>

<span data-ttu-id="cedca-130">Компоненты используют пакет SDK JavaScript для Microsoft Graph для всех вызовов Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="cedca-130">The components use the Microsoft Graph Javascript SDK for all calls to Microsoft Graph.</span></span> <span data-ttu-id="cedca-131">Поставщик должен предоставить пакет SDK, доступный через `graph` свойство.</span><span class="sxs-lookup"><span data-stu-id="cedca-131">Your provider must make the SDK available through the `graph` property.</span></span> <span data-ttu-id="cedca-132">В конструкторе создайте новый `Graph` экземпляр, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="cedca-132">In your constructor, create a new `Graph` instance, as shown.</span></span>

```js
this.graph = new Graph(this);
```

<span data-ttu-id="cedca-133">Этот `Graph` класс представляет собой тонкую обертку на основе пакета SDK Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="cedca-133">The `Graph` class is a light wrapper on top of the Microsoft Graph SDK.</span></span>

### <a name="example"></a><span data-ttu-id="cedca-134">Пример</span><span class="sxs-lookup"><span data-stu-id="cedca-134">Example</span></span>

<span data-ttu-id="cedca-135">Все поставщики расширяют `IProvider` абстрактный класс.</span><span class="sxs-lookup"><span data-stu-id="cedca-135">All the providers extend the `IProvider` abstract class.</span></span> <span data-ttu-id="cedca-136">В качестве примера рассмотрим исходный код для любого из [существующих поставщиков](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/src/providers).</span><span class="sxs-lookup"><span data-stu-id="cedca-136">For examples, take a look at the source code for any of the [existing providers](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/src/providers).</span></span>

## <a name="set-the-global-provider"></a><span data-ttu-id="cedca-137">Настройка глобального поставщика</span><span class="sxs-lookup"><span data-stu-id="cedca-137">Set the global provider</span></span>

<span data-ttu-id="cedca-138">Компоненты используют `Providers.globalProvider` свойство для доступа к поставщику.</span><span class="sxs-lookup"><span data-stu-id="cedca-138">Components use the `Providers.globalProvider` property to access a provider.</span></span> <span data-ttu-id="cedca-139">После создания собственного поставщика задайте этому свойству поставщика.</span><span class="sxs-lookup"><span data-stu-id="cedca-139">After you create your own provider, set this property to your provider.</span></span>

```ts
import { Providers } from '@microsoft/mgt';

Providers.globalProvider = myProvider;
```

<span data-ttu-id="cedca-140">Все компоненты будут уведомлены о новом поставщике и приступить к его использованию.</span><span class="sxs-lookup"><span data-stu-id="cedca-140">All the components will be notified of the new provider and start using it.</span></span>
