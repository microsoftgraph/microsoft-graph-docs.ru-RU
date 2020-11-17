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
# <a name="custom-provider"></a><span data-ttu-id="fe301-103">Настраиваемый поставщик</span><span class="sxs-lookup"><span data-stu-id="fe301-103">Custom provider</span></span>

<span data-ttu-id="fe301-104">Если в вашем приложении есть код проверки подлинности, вы можете создать настраиваемый поставщик, чтобы включить проверку подлинности и доступ к Microsoft Graph для компонентов набора инструментов Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="fe301-104">If you have existing authentication code in your application, you can create a custom provider to enable authentication and access to Microsoft Graph for Microsoft Graph Toolkit components.</span></span> <span data-ttu-id="fe301-105">Существует два способа создания настраиваемых поставщиков:</span><span class="sxs-lookup"><span data-stu-id="fe301-105">There are two ways to create custom providers:</span></span>

- <span data-ttu-id="fe301-106">Создание нового `SimpleProvider` путем передачи функции для получения маркера доступа</span><span class="sxs-lookup"><span data-stu-id="fe301-106">Create a new `SimpleProvider` by passing in a function for getting an access token</span></span>
- <span data-ttu-id="fe301-107">Расширение `IProvider` абстрактного класса</span><span class="sxs-lookup"><span data-stu-id="fe301-107">Extend the `IProvider` abstract class</span></span>

<span data-ttu-id="fe301-108">В этой статье каждый из этих способов описывается более подробно.</span><span class="sxs-lookup"><span data-stu-id="fe301-108">This article describes each approach in more detail.</span></span>

## <a name="simpleprovider"></a><span data-ttu-id="fe301-109">симплепровидер</span><span class="sxs-lookup"><span data-stu-id="fe301-109">SimpleProvider</span></span>

<span data-ttu-id="fe301-110">Создайте экземпляр `SimpleProvider` класса, передав функцию, которая будет возвращать маркер доступа для переданных областей.</span><span class="sxs-lookup"><span data-stu-id="fe301-110">Instantiate the `SimpleProvider` class by passing in a function that will return an access token for passed-in scopes.</span></span> 

```ts
let provider = new SimpleProvider((scopes: string[]) => {
  // return a promise with accessToken
});
```

<span data-ttu-id="fe301-111">Кроме того, вы также можете указать дополнительные `login` функции и `logout` функции, которые могут обрабатывать вызовы входа и выхода из компонента [Login](../components/login.md) .</span><span class="sxs-lookup"><span data-stu-id="fe301-111">In addition, you can also provide an optional `login` and `logout` functions that can handle the sign in and sign out calls from the [Login](../components/login.md) component.</span></span>

> [!IMPORTANT] 
> <span data-ttu-id="fe301-112">Чтобы указать компоненты, которые они могут начать вызывать API Microsoft Graph после успешного входа пользователя, необходимо позвонить `Providers.setState(ProviderState.SignedIn)` .</span><span class="sxs-lookup"><span data-stu-id="fe301-112">To indicate to the components that they can start calling the Microsoft Graph APIs after a user successfully signs in, you need to call `Providers.setState(ProviderState.SignedIn)`.</span></span> <span data-ttu-id="fe301-113">Пример такой функции показан в `login` приведенной ниже функции.</span><span class="sxs-lookup"><span data-stu-id="fe301-113">An example of this is shown in the `login` function below.</span></span>

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

### <a name="manage-state"></a><span data-ttu-id="fe301-114">Управление состоянием</span><span class="sxs-lookup"><span data-stu-id="fe301-114">Manage state</span></span>

<span data-ttu-id="fe301-115">Чтобы компоненты могли знать о состоянии поставщика, необходимо вызвать `provider.setState(state: ProviderState)` метод при изменении состояния.</span><span class="sxs-lookup"><span data-stu-id="fe301-115">For the components to be aware of the state of the provider, you will need to call the `provider.setState(state: ProviderState)` method whenever the state changes.</span></span> <span data-ttu-id="fe301-116">Например, если пользователь выполнил вход, вызовите `provider.setState(ProviderState.SignedIn)` .</span><span class="sxs-lookup"><span data-stu-id="fe301-116">For example, when the user has signed in, call `provider.setState(ProviderState.SignedIn)`.</span></span> <span data-ttu-id="fe301-117">`ProviderState`Перечисление определяет три состояния, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="fe301-117">The `ProviderState` enum defines three states, as shown.</span></span>

```ts
export enum ProviderState {
  Loading,
  SignedOut,
  SignedIn
}
```

## <a name="iprovider"></a><span data-ttu-id="fe301-118">ипровидер</span><span class="sxs-lookup"><span data-stu-id="fe301-118">IProvider</span></span>

<span data-ttu-id="fe301-119">`IProvider`Абстрактный класс можно расширить для создания собственного поставщика.</span><span class="sxs-lookup"><span data-stu-id="fe301-119">You can extend the `IProvider` abstract class to create your own provider.</span></span>

### <a name="state"></a><span data-ttu-id="fe301-120">Состояние</span><span class="sxs-lookup"><span data-stu-id="fe301-120">State</span></span>

<span data-ttu-id="fe301-121">Поставщик должен отслеживать состояние проверки подлинности и обновлять компоненты при изменении состояния.</span><span class="sxs-lookup"><span data-stu-id="fe301-121">A provider must keep track of the authentication state and update the components when the state changes.</span></span> <span data-ttu-id="fe301-122">`IProvider`Класс уже реализует `onStateChanged(eventHandler)` обработчик и `state: ProviderState` свойство.</span><span class="sxs-lookup"><span data-stu-id="fe301-122">The `IProvider` class already implements the `onStateChanged(eventHandler)` handler and the `state: ProviderState` property.</span></span> <span data-ttu-id="fe301-123">Для `setState(state:ProviderState)` обновления состояния при изменении состояния необходимо просто использовать метод в реализации.</span><span class="sxs-lookup"><span data-stu-id="fe301-123">You just need to use the `setState(state:ProviderState)` method in your implementation to update the state when it changes.</span></span> <span data-ttu-id="fe301-124">При обновлении состояния событие будет срабатывать `stateChanged` и автоматически обновлены все компоненты.</span><span class="sxs-lookup"><span data-stu-id="fe301-124">Updating the state will fire the `stateChanged` event and update all the components automatically.</span></span>

### <a name="loginlogout"></a><span data-ttu-id="fe301-125">Вход/выход</span><span class="sxs-lookup"><span data-stu-id="fe301-125">Login/Logout</span></span>

<span data-ttu-id="fe301-126">Если поставщик предоставляет функции входа или выхода, реализуйте `login(): Promise<void>` методы и `logout(): Promise<void>` .</span><span class="sxs-lookup"><span data-stu-id="fe301-126">If your provider provides login or logout functionality, implement the `login(): Promise<void>` and `logout(): Promise<void>` methods.</span></span> <span data-ttu-id="fe301-127">Эти методы являются необязательными.</span><span class="sxs-lookup"><span data-stu-id="fe301-127">These methods are optional.</span></span>

### <a name="access-token"></a><span data-ttu-id="fe301-128">Маркер доступа</span><span class="sxs-lookup"><span data-stu-id="fe301-128">Access token</span></span>

<span data-ttu-id="fe301-129">Необходимо реализовать `getAccessToken({'scopes': scopes[]}) : Promise<string>` метод.</span><span class="sxs-lookup"><span data-stu-id="fe301-129">You must implement the `getAccessToken({'scopes': scopes[]}) : Promise<string>` method.</span></span> <span data-ttu-id="fe301-130">Этот метод используется для получения действительного маркера перед каждым вызовом Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="fe301-130">This method is used to get a valid token before every call to Microsoft Graph.</span></span>

### <a name="graph"></a><span data-ttu-id="fe301-131">Graph</span><span class="sxs-lookup"><span data-stu-id="fe301-131">Graph</span></span>

<span data-ttu-id="fe301-132">Компоненты используют пакет SDK JavaScript для Microsoft Graph для всех вызовов Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="fe301-132">The components use the Microsoft Graph Javascript SDK for all calls to Microsoft Graph.</span></span> <span data-ttu-id="fe301-133">Поставщик должен предоставить пакет SDK, доступный через `graph` свойство.</span><span class="sxs-lookup"><span data-stu-id="fe301-133">Your provider must make the SDK available through the `graph` property.</span></span> <span data-ttu-id="fe301-134">В конструкторе создайте новый `Graph` экземпляр, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="fe301-134">In your constructor, create a new `Graph` instance, as shown.</span></span>

```js
this.graph = new Graph(this);
```

<span data-ttu-id="fe301-135">Этот `Graph` класс представляет собой тонкую обертку на основе пакета SDK Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="fe301-135">The `Graph` class is a light wrapper on top of the Microsoft Graph SDK.</span></span>

### <a name="example"></a><span data-ttu-id="fe301-136">Пример</span><span class="sxs-lookup"><span data-stu-id="fe301-136">Example</span></span>

<span data-ttu-id="fe301-137">Все поставщики расширяют `IProvider` абстрактный класс.</span><span class="sxs-lookup"><span data-stu-id="fe301-137">All the providers extend the `IProvider` abstract class.</span></span> <span data-ttu-id="fe301-138">В качестве примера рассмотрим исходный код для любого из [существующих поставщиков](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/main/packages/mgt/src/providers).</span><span class="sxs-lookup"><span data-stu-id="fe301-138">For examples, take a look at the source code for any of the [existing providers](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/main/packages/mgt/src/providers).</span></span>

## <a name="set-the-global-provider"></a><span data-ttu-id="fe301-139">Настройка глобального поставщика</span><span class="sxs-lookup"><span data-stu-id="fe301-139">Set the global provider</span></span>

<span data-ttu-id="fe301-140">Компоненты используют `Providers.globalProvider` свойство для доступа к поставщику.</span><span class="sxs-lookup"><span data-stu-id="fe301-140">Components use the `Providers.globalProvider` property to access a provider.</span></span> <span data-ttu-id="fe301-141">После создания собственного поставщика задайте этому свойству поставщика.</span><span class="sxs-lookup"><span data-stu-id="fe301-141">After you create your own provider, set this property to your provider.</span></span>

```ts
import { Providers } from '@microsoft/mgt';

Providers.globalProvider = myProvider;
```

<span data-ttu-id="fe301-142">Все компоненты будут уведомлены о новом поставщике и приступить к его использованию.</span><span class="sxs-lookup"><span data-stu-id="fe301-142">All the components will be notified of the new provider and start using it.</span></span>
