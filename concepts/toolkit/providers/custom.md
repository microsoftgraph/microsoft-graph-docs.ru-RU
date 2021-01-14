---
title: Настраиваемый поставщик
description: Создайте настраиваемый поставщик, чтобы включить проверку подлинности и доступ к Microsoft Graph для компонентов Microsoft Graph Toolkit при наличии существующего кода проверки подлинности в вашем приложении.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 57b7ca843f71d22992df18dc2466d0182d3fc556
ms.sourcegitcommit: 186d738f04e5a558da423f2429165fb4fbe780aa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086601"
---
# <a name="custom-provider"></a><span data-ttu-id="bcb94-103">Настраиваемый поставщик</span><span class="sxs-lookup"><span data-stu-id="bcb94-103">Custom provider</span></span>

<span data-ttu-id="bcb94-104">Если в вашем приложении есть существующий код проверки подлинности, вы можете создать настраиваемый поставщик, чтобы включить проверку подлинности и доступ к Microsoft Graph для компонентов Microsoft Graph Toolkit.</span><span class="sxs-lookup"><span data-stu-id="bcb94-104">If you have existing authentication code in your application, you can create a custom provider to enable authentication and access to Microsoft Graph for Microsoft Graph Toolkit components.</span></span> <span data-ttu-id="bcb94-105">Создать настраиваемых поставщиков можно двумя способами:</span><span class="sxs-lookup"><span data-stu-id="bcb94-105">There are two ways to create custom providers:</span></span>

- <span data-ttu-id="bcb94-106">Создать новый класс `SimpleProvider`, передав функцию для получения маркера доступа</span><span class="sxs-lookup"><span data-stu-id="bcb94-106">Create a new `SimpleProvider` by passing in a function for getting an access token</span></span>
- <span data-ttu-id="bcb94-107">Расширить абстрактный класс `IProvider`</span><span class="sxs-lookup"><span data-stu-id="bcb94-107">Extend the `IProvider` abstract class</span></span>

<span data-ttu-id="bcb94-108">В этой статье подробно описан каждый из подходов.</span><span class="sxs-lookup"><span data-stu-id="bcb94-108">This article describes each approach in more detail.</span></span>

## <a name="simpleprovider"></a><span data-ttu-id="bcb94-109">SimpleProvider</span><span class="sxs-lookup"><span data-stu-id="bcb94-109">SimpleProvider</span></span>

<span data-ttu-id="bcb94-110">Создайте экземпляр класса `SimpleProvider`, передав функцию, которая вернет маркер доступа для переданных областей.</span><span class="sxs-lookup"><span data-stu-id="bcb94-110">Instantiate the `SimpleProvider` class by passing in a function that will return an access token for passed-in scopes.</span></span> 

```ts
let provider = new SimpleProvider((scopes: string[]) => {
  // return a promise with accessToken
});
```

<span data-ttu-id="bcb94-111">Кроме того, вы также можете предоставить необязательные функции `login` и `logout`, которые могут обрабатывать вызовы входа и выхода из компонента [Вход](../components/login.md).</span><span class="sxs-lookup"><span data-stu-id="bcb94-111">In addition, you can also provide an optional `login` and `logout` functions that can handle the sign in and sign out calls from the [Login](../components/login.md) component.</span></span>

> [!IMPORTANT] 
> <span data-ttu-id="bcb94-112">Чтобы указать компонентам, что они могут начать вызов API Microsoft Graph после успешного входа пользователя, необходимо вызвать `Providers.setState(ProviderState.SignedIn)`.</span><span class="sxs-lookup"><span data-stu-id="bcb94-112">To indicate to the components that they can start calling the Microsoft Graph APIs after a user successfully signs in, you need to call `Providers.setState(ProviderState.SignedIn)`.</span></span> <span data-ttu-id="bcb94-113">Пример показан в функции `login` ниже.</span><span class="sxs-lookup"><span data-stu-id="bcb94-113">An example of this is shown in the `login` function below.</span></span>

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

### <a name="manage-state"></a><span data-ttu-id="bcb94-114">Управление состоянием</span><span class="sxs-lookup"><span data-stu-id="bcb94-114">Manage state</span></span>

<span data-ttu-id="bcb94-115">Чтобы компоненты знали состояние поставщика, следует вызывать метод `provider.setState(state: ProviderState)` при любом изменении состояния.</span><span class="sxs-lookup"><span data-stu-id="bcb94-115">For the components to be aware of the state of the provider, you will need to call the `provider.setState(state: ProviderState)` method whenever the state changes.</span></span> <span data-ttu-id="bcb94-116">Например, когда пользователь вошел, вызовите`provider.setState(ProviderState.SignedIn)`.</span><span class="sxs-lookup"><span data-stu-id="bcb94-116">For example, when the user has signed in, call `provider.setState(ProviderState.SignedIn)`.</span></span> <span data-ttu-id="bcb94-117">Как показано, перечисление `ProviderState` определяет три состояния.</span><span class="sxs-lookup"><span data-stu-id="bcb94-117">The `ProviderState` enum defines three states, as shown.</span></span>

```ts
export enum ProviderState {
  Loading,
  SignedOut,
  SignedIn
}
```

## <a name="iprovider"></a><span data-ttu-id="bcb94-118">IProvider</span><span class="sxs-lookup"><span data-stu-id="bcb94-118">IProvider</span></span>

<span data-ttu-id="bcb94-119">Вы можете расширить абстрактный класс `IProvider`, чтобы создать собственный поставщик.</span><span class="sxs-lookup"><span data-stu-id="bcb94-119">You can extend the `IProvider` abstract class to create your own provider.</span></span>

### <a name="state"></a><span data-ttu-id="bcb94-120">Состояние</span><span class="sxs-lookup"><span data-stu-id="bcb94-120">State</span></span>

<span data-ttu-id="bcb94-121">Поставщик должен следить за состоянием проверки подлинности и обновлять компоненты при изменении состояния.</span><span class="sxs-lookup"><span data-stu-id="bcb94-121">A provider must keep track of the authentication state and update the components when the state changes.</span></span> <span data-ttu-id="bcb94-122">Класс `IProvider` уже реализует обработчик `onStateChanged(eventHandler)` и свойство `state: ProviderState`.</span><span class="sxs-lookup"><span data-stu-id="bcb94-122">The `IProvider` class already implements the `onStateChanged(eventHandler)` handler and the `state: ProviderState` property.</span></span> <span data-ttu-id="bcb94-123">Вам просто нужно использовать метод `setState(state:ProviderState)` в реализации, чтобы обновить состояние, когда оно изменится.</span><span class="sxs-lookup"><span data-stu-id="bcb94-123">You just need to use the `setState(state:ProviderState)` method in your implementation to update the state when it changes.</span></span> <span data-ttu-id="bcb94-124">При обновлении состояния будет вызвано событие `stateChanged` и автоматически обновлены все компоненты.</span><span class="sxs-lookup"><span data-stu-id="bcb94-124">Updating the state will fire the `stateChanged` event and update all the components automatically.</span></span>

### <a name="loginlogout"></a><span data-ttu-id="bcb94-125">Вход/Выход</span><span class="sxs-lookup"><span data-stu-id="bcb94-125">Login/Logout</span></span>

<span data-ttu-id="bcb94-126">Если поставщик предоставляет функцию входа или выхода, реализуйте методы `login(): Promise<void>` и `logout(): Promise<void>`.</span><span class="sxs-lookup"><span data-stu-id="bcb94-126">If your provider provides login or logout functionality, implement the `login(): Promise<void>` and `logout(): Promise<void>` methods.</span></span> <span data-ttu-id="bcb94-127">Эти методы являются необязательными.</span><span class="sxs-lookup"><span data-stu-id="bcb94-127">These methods are optional.</span></span>

### <a name="access-token"></a><span data-ttu-id="bcb94-128">Маркер доступа</span><span class="sxs-lookup"><span data-stu-id="bcb94-128">Access token</span></span>

<span data-ttu-id="bcb94-129">Необходимо реализовать метод `getAccessToken({'scopes': scopes[]}) : Promise<string>`.</span><span class="sxs-lookup"><span data-stu-id="bcb94-129">You must implement the `getAccessToken({'scopes': scopes[]}) : Promise<string>` method.</span></span> <span data-ttu-id="bcb94-130">Этот метод используется для получения допустимого маркера перед каждым вызовом Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="bcb94-130">This method is used to get a valid token before every call to Microsoft Graph.</span></span>

### <a name="graph"></a><span data-ttu-id="bcb94-131">Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="bcb94-131">Graph</span></span>

<span data-ttu-id="bcb94-132">Компоненты используют пакет SDK Microsoft Graph для JavaScript для всех вызовов Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="bcb94-132">The components use the Microsoft Graph Javascript SDK for all calls to Microsoft Graph.</span></span> <span data-ttu-id="bcb94-133">Поставщик должен сделать пакет SDK доступным с помощью свойства `graph`.</span><span class="sxs-lookup"><span data-stu-id="bcb94-133">Your provider must make the SDK available through the `graph` property.</span></span> <span data-ttu-id="bcb94-134">Создайте в конструкторе новый экземпляр `Graph`, как показано.</span><span class="sxs-lookup"><span data-stu-id="bcb94-134">In your constructor, create a new `Graph` instance, as shown.</span></span>

```js
this.graph = new Graph(this);
```

<span data-ttu-id="bcb94-135">Класс `Graph` — это легкая оболочка поверх пакета SDK Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="bcb94-135">The `Graph` class is a light wrapper on top of the Microsoft Graph SDK.</span></span>

### <a name="example"></a><span data-ttu-id="bcb94-136">Пример</span><span class="sxs-lookup"><span data-stu-id="bcb94-136">Example</span></span>

<span data-ttu-id="bcb94-137">Все поставщики расширяют абстрактный класс `IProvider`.</span><span class="sxs-lookup"><span data-stu-id="bcb94-137">All the providers extend the `IProvider` abstract class.</span></span> <span data-ttu-id="bcb94-138">Например, посмотрите на исходный код для любого из [существующих поставщиков](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/main/packages/mgt/src/providers).</span><span class="sxs-lookup"><span data-stu-id="bcb94-138">For examples, take a look at the source code for any of the [existing providers](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/main/packages/mgt/src/providers).</span></span>

## <a name="set-the-global-provider"></a><span data-ttu-id="bcb94-139">Настройка глобального поставщика</span><span class="sxs-lookup"><span data-stu-id="bcb94-139">Set the global provider</span></span>

<span data-ttu-id="bcb94-140">Компоненты используют свойство `Providers.globalProvider` для доступа к поставщику.</span><span class="sxs-lookup"><span data-stu-id="bcb94-140">Components use the `Providers.globalProvider` property to access a provider.</span></span> <span data-ttu-id="bcb94-141">После создания собственного поставщика, задайте это свойство для него.</span><span class="sxs-lookup"><span data-stu-id="bcb94-141">After you create your own provider, set this property to your provider.</span></span>

```ts
import { Providers } from '@microsoft/mgt';

Providers.globalProvider = myProvider;
```

<span data-ttu-id="bcb94-142">Все компоненты будут уведомлены о новом поставщике и начнут его использовать.</span><span class="sxs-lookup"><span data-stu-id="bcb94-142">All the components will be notified of the new provider and start using it.</span></span>
