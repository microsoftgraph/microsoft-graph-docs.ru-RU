---
title: Настраиваемый поставщик
description: Создайте настраиваемый поставщик, чтобы включить проверку подлинности и доступ к Graph для компонентов набора средств Microsoft Graph, если в вашем приложении есть код проверки подлинности.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 4e287a38a584f77b7dfedf6e36d56da7a4e29715
ms.sourcegitcommit: 8e18d7fe3c869b2fd48872365116175d3bdce1b7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/12/2020
ms.locfileid: "46643738"
---
# <a name="custom-provider"></a><span data-ttu-id="3488a-103">Настраиваемый поставщик</span><span class="sxs-lookup"><span data-stu-id="3488a-103">Custom provider</span></span>

<span data-ttu-id="3488a-104">Если в вашем приложении есть код проверки подлинности, вы можете создать настраиваемый поставщик, чтобы включить проверку подлинности и доступ к Microsoft Graph для компонентов набора инструментов Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="3488a-104">If you have existing authentication code in your application, you can create a custom provider to enable authentication and access to Microsoft Graph for Microsoft Graph Toolkit components.</span></span> <span data-ttu-id="3488a-105">Существует два способа создания настраиваемых поставщиков:</span><span class="sxs-lookup"><span data-stu-id="3488a-105">There are two ways to create custom providers:</span></span>

- <span data-ttu-id="3488a-106">Создание нового `SimpleProvider` путем передачи функции для получения маркера доступа</span><span class="sxs-lookup"><span data-stu-id="3488a-106">Create a new `SimpleProvider` by passing in a function for getting an access token</span></span>
- <span data-ttu-id="3488a-107">Расширение `IProvider` абстрактного класса</span><span class="sxs-lookup"><span data-stu-id="3488a-107">Extend the `IProvider` abstract class</span></span>

<span data-ttu-id="3488a-108">В этой статье каждый из этих способов описывается более подробно.</span><span class="sxs-lookup"><span data-stu-id="3488a-108">This article describes each approach in more detail.</span></span>

## <a name="simpleprovider"></a><span data-ttu-id="3488a-109">симплепровидер</span><span class="sxs-lookup"><span data-stu-id="3488a-109">SimpleProvider</span></span>

<span data-ttu-id="3488a-110">Создайте экземпляр `SimpleProvider` класса, передав функцию, которая будет возвращать маркер доступа для переданных областей.</span><span class="sxs-lookup"><span data-stu-id="3488a-110">Instantiate the `SimpleProvider` class by passing in a function that will return an access token for passed-in scopes.</span></span>

```ts
let provider = new SimpleProvider((scopes: string[]) => {
  // return a promise with accessToken
});
```

<span data-ttu-id="3488a-111">Кроме того, вы также можете указать дополнительные `login` функции и `logout` функции, которые могут обрабатывать вызовы входа и выхода из компонента [Login](../components/login.md) .</span><span class="sxs-lookup"><span data-stu-id="3488a-111">In addition, you can also provide an optional `login` and `logout` functions that can handle the sign in and sign out calls from the [Login](../components/login.md) component.</span></span>

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

### <a name="manage-state"></a><span data-ttu-id="3488a-112">Управление состоянием</span><span class="sxs-lookup"><span data-stu-id="3488a-112">Manage state</span></span>

<span data-ttu-id="3488a-113">Чтобы компоненты могли знать о состоянии поставщика, необходимо вызвать `provider.setState(state: ProviderState)` метод при изменении состояния.</span><span class="sxs-lookup"><span data-stu-id="3488a-113">For the components to be aware of the state of the provider, you will need to call the `provider.setState(state: ProviderState)` method whenever the state changes.</span></span> <span data-ttu-id="3488a-114">Например, если пользователь выполнил вход, вызовите `provider.setState(ProviderState.SignedIn)` .</span><span class="sxs-lookup"><span data-stu-id="3488a-114">For example, when the user has signed in, call `provider.setState(ProviderState.SignedIn)`.</span></span> <span data-ttu-id="3488a-115">`ProviderState`Перечисление определяет три состояния, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="3488a-115">The `ProviderState` enum defines three states, as shown.</span></span>

```ts
export enum ProviderState {
  Loading,
  SignedOut,
  SignedIn
}
```

## <a name="iprovider"></a><span data-ttu-id="3488a-116">ипровидер</span><span class="sxs-lookup"><span data-stu-id="3488a-116">IProvider</span></span>

<span data-ttu-id="3488a-117">`IProvider`Абстрактный класс можно расширить для создания собственного поставщика.</span><span class="sxs-lookup"><span data-stu-id="3488a-117">You can extend the `IProvider` abstract class to create your own provider.</span></span>

### <a name="state"></a><span data-ttu-id="3488a-118">State</span><span class="sxs-lookup"><span data-stu-id="3488a-118">State</span></span>

<span data-ttu-id="3488a-119">Поставщик должен отслеживать состояние проверки подлинности и обновлять компоненты при изменении состояния.</span><span class="sxs-lookup"><span data-stu-id="3488a-119">A provider must keep track of the authentication state and update the components when the state changes.</span></span> <span data-ttu-id="3488a-120">`IProvider`Класс уже реализует `onStateChanged(eventHandler)` обработчик и `state: ProviderState` свойство.</span><span class="sxs-lookup"><span data-stu-id="3488a-120">The `IProvider` class already implements the `onStateChanged(eventHandler)` handler and the `state: ProviderState` property.</span></span> <span data-ttu-id="3488a-121">Для `setState(state:ProviderState)` обновления состояния при изменении состояния необходимо просто использовать метод в реализации.</span><span class="sxs-lookup"><span data-stu-id="3488a-121">You just need to use the `setState(state:ProviderState)` method in your implementation to update the state when it changes.</span></span> <span data-ttu-id="3488a-122">При обновлении состояния событие будет срабатывать `stateChanged` и автоматически обновлены все компоненты.</span><span class="sxs-lookup"><span data-stu-id="3488a-122">Updating the state will fire the `stateChanged` event and update all the components automatically.</span></span>

### <a name="loginlogout"></a><span data-ttu-id="3488a-123">Вход/выход</span><span class="sxs-lookup"><span data-stu-id="3488a-123">Login/Logout</span></span>

<span data-ttu-id="3488a-124">Если поставщик предоставляет функции входа или выхода, реализуйте `login(): Promise<void>` методы и `logout(): Promise<void>` .</span><span class="sxs-lookup"><span data-stu-id="3488a-124">If your provider provides login or logout functionality, implement the `login(): Promise<void>` and `logout(): Promise<void>` methods.</span></span> <span data-ttu-id="3488a-125">Эти методы являются необязательными.</span><span class="sxs-lookup"><span data-stu-id="3488a-125">These methods are optional.</span></span>

### <a name="access-token"></a><span data-ttu-id="3488a-126">Маркер доступа</span><span class="sxs-lookup"><span data-stu-id="3488a-126">Access token</span></span>

<span data-ttu-id="3488a-127">Необходимо реализовать `getAccessToken({'scopes': scopes[]}) : Promise<string>` метод.</span><span class="sxs-lookup"><span data-stu-id="3488a-127">You must implement the `getAccessToken({'scopes': scopes[]}) : Promise<string>` method.</span></span> <span data-ttu-id="3488a-128">Этот метод используется для получения действительного маркера перед каждым вызовом Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="3488a-128">This method is used to get a valid token before every call to Microsoft Graph.</span></span>

### <a name="graph"></a><span data-ttu-id="3488a-129">Graph</span><span class="sxs-lookup"><span data-stu-id="3488a-129">Graph</span></span>

<span data-ttu-id="3488a-130">Компоненты используют пакет SDK JavaScript для Microsoft Graph для всех вызовов Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="3488a-130">The components use the Microsoft Graph Javascript SDK for all calls to Microsoft Graph.</span></span> <span data-ttu-id="3488a-131">Поставщик должен предоставить пакет SDK, доступный через `graph` свойство.</span><span class="sxs-lookup"><span data-stu-id="3488a-131">Your provider must make the SDK available through the `graph` property.</span></span> <span data-ttu-id="3488a-132">В конструкторе создайте новый `Graph` экземпляр, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="3488a-132">In your constructor, create a new `Graph` instance, as shown.</span></span>

```js
this.graph = new Graph(this);
```

<span data-ttu-id="3488a-133">Этот `Graph` класс представляет собой тонкую обертку на основе пакета SDK Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="3488a-133">The `Graph` class is a light wrapper on top of the Microsoft Graph SDK.</span></span>

### <a name="example"></a><span data-ttu-id="3488a-134">Пример</span><span class="sxs-lookup"><span data-stu-id="3488a-134">Example</span></span>

<span data-ttu-id="3488a-135">Все поставщики расширяют `IProvider` абстрактный класс.</span><span class="sxs-lookup"><span data-stu-id="3488a-135">All the providers extend the `IProvider` abstract class.</span></span> <span data-ttu-id="3488a-136">В качестве примера рассмотрим исходный код для любого из [существующих поставщиков](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/main/packages/mgt/src/providers).</span><span class="sxs-lookup"><span data-stu-id="3488a-136">For examples, take a look at the source code for any of the [existing providers](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/main/packages/mgt/src/providers).</span></span>

## <a name="set-the-global-provider"></a><span data-ttu-id="3488a-137">Настройка глобального поставщика</span><span class="sxs-lookup"><span data-stu-id="3488a-137">Set the global provider</span></span>

<span data-ttu-id="3488a-138">Компоненты используют `Providers.globalProvider` свойство для доступа к поставщику.</span><span class="sxs-lookup"><span data-stu-id="3488a-138">Components use the `Providers.globalProvider` property to access a provider.</span></span> <span data-ttu-id="3488a-139">После создания собственного поставщика задайте этому свойству поставщика.</span><span class="sxs-lookup"><span data-stu-id="3488a-139">After you create your own provider, set this property to your provider.</span></span>

```ts
import { Providers } from '@microsoft/mgt';

Providers.globalProvider = myProvider;
```

<span data-ttu-id="3488a-140">Все компоненты будут уведомлены о новом поставщике и приступить к его использованию.</span><span class="sxs-lookup"><span data-stu-id="3488a-140">All the components will be notified of the new provider and start using it.</span></span>
