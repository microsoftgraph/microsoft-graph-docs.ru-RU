---
title: Использование microsoft Graph набор средств React
description: Начало работы с microsoft Graph набор средств в приложении React.
localization_priority: Normal
author: waldekmastykarz
ms.openlocfilehash: 57e9901c8b7ee1f8a5474f21ff4b09def053e7db
ms.sourcegitcommit: 7902607a1e5a030d46e907d08e16644a47a47006
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/12/2020
ms.locfileid: "49664137"
---
# <a name="use-the-microsoft-graph-toolkit-with-react"></a><span data-ttu-id="0d63b-103">Использование microsoft Graph набор средств React</span><span class="sxs-lookup"><span data-stu-id="0d63b-103">Use the Microsoft Graph Toolkit with React</span></span>

<span data-ttu-id="0d63b-104">Microsoft Graph набор средств это набор веб-компонентов, упрощающих подключение к Microsoft Graph и позволяющих сосредоточиться на приложении.</span><span class="sxs-lookup"><span data-stu-id="0d63b-104">Microsoft Graph Toolkit is a set of web components that simplify connecting to Microsoft Graph and allow you to focus on your application instead.</span></span> <span data-ttu-id="0d63b-105">Microsoft Graph набор средств как универсальный набор веб-компонентов, распространяемых через `@microsoft/mgt` пакет npm.</span><span class="sxs-lookup"><span data-stu-id="0d63b-105">Microsoft Graph Toolkit is available as a generic set of web components distributed through the `@microsoft/mgt` npm package.</span></span>

<span data-ttu-id="0d63b-106">Если вы создаете приложения с помощью React, вы можете использовать [ `@microsoft/mgt-react` пакет,](./mgt-react.md)который упаковывает веб-компоненты Microsoft Graph набор средств в компоненты React и упрощает передачу сложных данных.</span><span class="sxs-lookup"><span data-stu-id="0d63b-106">If you're building apps with React, you can use the [`@microsoft/mgt-react` package](./mgt-react.md), which wraps Microsoft Graph Toolkit web components in React components and makes it easier to pass complex data.</span></span>

<span data-ttu-id="0d63b-107">В этой статье описывается пошаговой процесс использования microsoft Graph набор средств для создания приложения React и его подключения к Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="0d63b-107">This article describes the step-by-step process of using the Microsoft Graph Toolkit to create a React app and connect it to Microsoft 365.</span></span> <span data-ttu-id="0d63b-108">После выполнения этих действий у вас будет приложение React, которое отображает предстоящие встречи войдя в microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="0d63b-108">After completing the steps, you'll have a React app that shows the upcoming appointments of the currently signed in user from Microsoft 365.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0d63b-109">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="0d63b-109">Prerequisites</span></span>

<span data-ttu-id="0d63b-110">Чтобы следовать шагам из этой статьи, вам потребуется среда разработки Microsoft 365 и несколько средств.</span><span class="sxs-lookup"><span data-stu-id="0d63b-110">To follow the steps in this article, you'll need a Microsoft 365 development environment and a few tools.</span></span> <span data-ttu-id="0d63b-111">Подробные сведения [см. в сведениях о том, как начать работу.](./overview.md)</span><span class="sxs-lookup"><span data-stu-id="0d63b-111">For details, see [getting started](./overview.md).</span></span>

## <a name="create-a-react-app"></a><span data-ttu-id="0d63b-112">Создание приложения React</span><span class="sxs-lookup"><span data-stu-id="0d63b-112">Create a React app</span></span>

<span data-ttu-id="0d63b-113">Создайте новое приложение React, выдав следующую команду.</span><span class="sxs-lookup"><span data-stu-id="0d63b-113">Create a new React app by running the following command.</span></span> <span data-ttu-id="0d63b-114">Это позволит создать новое приложение React с помощью TypeScript, которое поможет вам написать более надежный код и избежать ошибок во время работы.</span><span class="sxs-lookup"><span data-stu-id="0d63b-114">This will create a new React app using TypeScript, which will help you write more robust code and avoid runtime errors.</span></span>

```cmd
npx create-react-app my-m365-app --template typescript
```

<span data-ttu-id="0d63b-115">Измените рабочий каталог на только что созданное приложение.</span><span class="sxs-lookup"><span data-stu-id="0d63b-115">Change the working directory to the newly created app.</span></span>

```cmd
cd my-m365-app
```

<span data-ttu-id="0d63b-116">Затем установите пакет npm, содержащий компоненты `mgt-react` Microsoft Graph набор средств React.</span><span class="sxs-lookup"><span data-stu-id="0d63b-116">Next, install the `mgt-react` npm package, which contains the Microsoft Graph Toolkit React components.</span></span>

```cmd
npm i @microsoft/mgt-react
```

<span data-ttu-id="0d63b-117">Установите также пакет npm, который содержит поставщика `mgt-msal-provider` `mgt-element` auth MSAL.</span><span class="sxs-lookup"><span data-stu-id="0d63b-117">Install the `mgt-msal-provider` and `mgt-element` npm package as well, which contains the MSAL auth provider.</span></span>

```cmd
npm i @microsoft/mgt-element @microsoft/mgt-msal-provider
```

<span data-ttu-id="0d63b-118">Подтвердите, что вы можете запустить приложение.</span><span class="sxs-lookup"><span data-stu-id="0d63b-118">Confirm that you can run the app.</span></span>

```cmd
npm start
```

<span data-ttu-id="0d63b-119">Вы должны иметь возможность открыть приложение в браузере с помощью `http://localhost:3000` .</span><span class="sxs-lookup"><span data-stu-id="0d63b-119">You should be able to open your app in the browser via `http://localhost:3000`.</span></span>

[!INCLUDE [AAD with implicit flow app registration](../includes/aad-app-registration-spa.md)]

## <a name="connect-react-app-to-microsoft-365"></a><span data-ttu-id="0d63b-120">Подключение приложения React к Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="0d63b-120">Connect React app to Microsoft 365</span></span>

<span data-ttu-id="0d63b-121">После регистрации приложения в Azure Active Directory (Azure AD) вы можете подключить приложение React к Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="0d63b-121">Now that you have registered your application with Azure Active Directory (Azure AD), you can connect the React app to Microsoft 365.</span></span> <span data-ttu-id="0d63b-122">Во-первых, разрешим пользователям войти в приложение с помощью своей учетной записи Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="0d63b-122">First, allow users to sign in to the app using their Microsoft account.</span></span>

### <a name="copy-the-azure-ad-application-registration-id"></a><span data-ttu-id="0d63b-123">Копирование ИД регистрации приложения Azure AD</span><span class="sxs-lookup"><span data-stu-id="0d63b-123">Copy the Azure AD application registration ID</span></span>

1. <span data-ttu-id="0d63b-124">На портале Azure перейдите к регистрации приложения.</span><span class="sxs-lookup"><span data-stu-id="0d63b-124">In the Azure Portal, go to your application registration.</span></span>
1. <span data-ttu-id="0d63b-125">Убедитесь, что вы находитесь на странице **"Обзор".**</span><span class="sxs-lookup"><span data-stu-id="0d63b-125">Verify that you are on the **Overview** page.</span></span>
1. <span data-ttu-id="0d63b-126">В разделе **"Essentials"** скопируйте значение свойства **Application (client) ID**</span><span class="sxs-lookup"><span data-stu-id="0d63b-126">From the **Essentials** section, copy the value of the **Application (client) ID** property</span></span>

### <a name="configure-the-microsoft-graph-toolkit-authentication-provider"></a><span data-ttu-id="0d63b-127">Настройка поставщика проверки подлинности набор средств Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="0d63b-127">Configure the Microsoft Graph Toolkit authentication provider</span></span>

<span data-ttu-id="0d63b-128">Затем настройте поставщика проверки подлинности, который должен набор средств Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="0d63b-128">Next, configure the authentication provider that the Microsoft Graph Toolkit should use.</span></span> <span data-ttu-id="0d63b-129">В этом случае вы будете использовать MSAL, что является хорошим значением по умолчанию для создания автономных приложений.</span><span class="sxs-lookup"><span data-stu-id="0d63b-129">In this case, you'll use MSAL, which is a good default for building standalone applications.</span></span> <span data-ttu-id="0d63b-130">Если вы используете любую из точек возможностей в Microsoft 365, например Teams или SharePoint, вы будете использовать [других поставщиков.](../providers/providers.md)</span><span class="sxs-lookup"><span data-stu-id="0d63b-130">If you use any of the extensibility points in Microsoft 365, like Teams or SharePoint, you will use [other providers](../providers/providers.md).</span></span>

1. <span data-ttu-id="0d63b-131">В редакторе кода откройте **src/index.**</span><span class="sxs-lookup"><span data-stu-id="0d63b-131">In the code editor, open the **src/index.**</span></span> <span data-ttu-id="0d63b-132">и в список импортов добавьте:</span><span class="sxs-lookup"><span data-stu-id="0d63b-132">file, and to the list of imports, add:</span></span>

    ```tsx
    import { Providers } from '@microsoft/mgt-element';
    import { MsalProvider } from '@microsoft/mgt-msal-provider';
    ```

1. <span data-ttu-id="0d63b-133">После последнего `import` оператора инициализировать microsoft Graph набор средств с помощью поставщика MSAL.</span><span class="sxs-lookup"><span data-stu-id="0d63b-133">After the last `import` statement, initialize the Microsoft Graph Toolkit with MSAL provider.</span></span>

    ```tsx
    Providers.globalProvider = new MsalProvider({
      clientId: 'REPLACE_WITH_CLIENTID'
    });
    ```

    <span data-ttu-id="0d63b-134">Замените значение свойства на значение свойства, скопированные ранее `clientId` `Application (client) ID` на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="0d63b-134">Replace the value of the `clientId` property with the value of the `Application (client) ID` property you copied previously in the Azure Portal.</span></span>

<span data-ttu-id="0d63b-135">При этих изменениях **файл src/index.tsx** будет выглядеть следующим образом.</span><span class="sxs-lookup"><span data-stu-id="0d63b-135">With these changes, the **src/index.tsx** file will look like the following.</span></span>

  ```tsx
  import React from 'react';
  import ReactDOM from 'react-dom';
  import App from './App';
  import './index.css';
  import * as serviceWorker from './serviceWorker';

  import { Providers } from '@microsoft/mgt-element';
  import { MsalProvider } from '@microsoft/mgt-msal-provider';
  
  Providers.globalProvider = new MsalProvider({
    clientId: 'REPLACE_WITH_CLIENTID'
  });
  
  ReactDOM.render(
    <React.StrictMode>
      <App />
    </React.StrictMode>,
    document.getElementById('root')
  );
  
  // If you want your app to work offline and load faster, you can change
  // unregister() to register() below. Note this comes with some pitfalls.
  // Learn more about service workers: https://bit.ly/CRA-PWA
  serviceWorker.unregister();
  ```

### <a name="add-the-sign-in-button"></a><span data-ttu-id="0d63b-136">Добавление кнопки "Вход"</span><span class="sxs-lookup"><span data-stu-id="0d63b-136">Add the Sign in button</span></span>

<span data-ttu-id="0d63b-137">Добавьте компонент **Microsoft** Graph для входа набор средств React,  который отобразит кнопку входа, которую можно использовать для входа с помощью учетной записи Майкрософт в ваше приложение.</span><span class="sxs-lookup"><span data-stu-id="0d63b-137">Add the **Login** Microsoft Graph Toolkit React component, which will display the **Sign in** button people can use to sign in with their Microsoft account to your app.</span></span>

1. <span data-ttu-id="0d63b-138">В редакторе кода откройте **файл src/App.tsx** и добавьте в список импорта:</span><span class="sxs-lookup"><span data-stu-id="0d63b-138">In the code editor, open the **src/App.tsx** file, and to the list of imports add:</span></span>

    ```tsx
    import { Login } from '@microsoft/mgt-react';
    ```

1. <span data-ttu-id="0d63b-139">В функции замените содержимое предложения базовой структурой, включая компонент `App` `return` Microsoft Graph набор средств входа:</span><span class="sxs-lookup"><span data-stu-id="0d63b-139">In the `App` function, replace the contents of the `return` clause with the basic structure including the Microsoft Graph Toolkit Login component:</span></span>

    ```tsx
    <div className="App">
      <header>
        <Login />
      </header>
    </div>
    ```

<span data-ttu-id="0d63b-140">После этих изменений **файл src/App.tsx** будет выглядеть следующим образом.</span><span class="sxs-lookup"><span data-stu-id="0d63b-140">With these changes, the **src/App.tsx** file will look like the following.</span></span>
```tsx

import { Login } from '@microsoft/mgt-react';
import React from 'react';
import './App.css';

function App() {
  return (
    <div className="App">
      <header>
        <Login />
      </header>
    </div>
  );
}

export default App;
```

### <a name="test-signing-in-to-your-application"></a><span data-ttu-id="0d63b-141">Проверка вход в приложение</span><span class="sxs-lookup"><span data-stu-id="0d63b-141">Test signing in to your application</span></span>

<span data-ttu-id="0d63b-142">Теперь у вас должна быть возможность войти в приложение с помощью учетной записи Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="0d63b-142">You should now be able to sign in to your application with your Microsoft account.</span></span>

1. <span data-ttu-id="0d63b-143">Перейдите в браузер, в котором запущено приложение React.</span><span class="sxs-lookup"><span data-stu-id="0d63b-143">Go back to the browser where your React app is running.</span></span> <span data-ttu-id="0d63b-144">Теперь вы увидите кнопку **"Вход".**</span><span class="sxs-lookup"><span data-stu-id="0d63b-144">You should now see a **Sign in** button.</span></span>
1. <span data-ttu-id="0d63b-145">При нажатии кнопки "Вход" вам будет предложено войти с помощью учетной записи Майкрософт (вы можете использовать ту же учетную запись, что и учетную запись, с помощью учетной записи, с помощью которая была у вас на портале Azure). </span><span class="sxs-lookup"><span data-stu-id="0d63b-145">When you click the **Sign in** button, you will be prompted to sign in with your Microsoft account (you can use the same account as the one you accessed the Azure Portal with).</span></span>
1. <span data-ttu-id="0d63b-146">Так как это первый раз, когда вы используете это приложение Azure AD, необходимо согласиться на его использование в вашей организации.</span><span class="sxs-lookup"><span data-stu-id="0d63b-146">Because this is the first time you're using this Azure AD application, you need to consent its use in your organization.</span></span>
1. <span data-ttu-id="0d63b-147">После этого вы будете перенаправлены в приложение React.</span><span class="sxs-lookup"><span data-stu-id="0d63b-147">After signing in, you will be redirected to your React app.</span></span> <span data-ttu-id="0d63b-148">Обратите внимание, что кнопка **"Вход"** изменена для показа имени пользователя в приложении React, в котором отображаются сведения о пользователе, полученные из Microsoft 365 с помощью ![ Microsoft Graph ](../images/mgt-react-userinfo.png) набор средств.</span><span class="sxs-lookup"><span data-stu-id="0d63b-148">Notice that the **Sign in** button changed to show your user's name ![React app showing user info retrieved from Microsoft 365 using Microsoft Graph Toolkit](../images/mgt-react-userinfo.png).</span></span>

## <a name="load-data-from-microsoft-365"></a><span data-ttu-id="0d63b-149">Загрузка данных из Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="0d63b-149">Load data from Microsoft 365</span></span>

<span data-ttu-id="0d63b-150">Microsoft Graph набор средств не только упрощает проверку подлинности в Microsoft 365, но и загружает ее данные.</span><span class="sxs-lookup"><span data-stu-id="0d63b-150">Microsoft Graph Toolkit not only simplifies authentication to Microsoft 365, but also loading its data.</span></span> <span data-ttu-id="0d63b-151">В этом примере вы увидите календарь во время подписания.</span><span class="sxs-lookup"><span data-stu-id="0d63b-151">In this example, you'll show the signed in person's calendar.</span></span>

### <a name="specify-permissions-needed-for-your-application"></a><span data-ttu-id="0d63b-152">Указание разрешений, необходимых для приложения</span><span class="sxs-lookup"><span data-stu-id="0d63b-152">Specify permissions needed for your application</span></span>

<span data-ttu-id="0d63b-153">Перед загрузкой данных из Microsoft 365 необходимо указать список областей разрешений, которые должно предоставить приложение для доступа к данным пользователя.</span><span class="sxs-lookup"><span data-stu-id="0d63b-153">Before you can load data from Microsoft 365, you need to specify the list of permission scopes your application must be granted to access user's data.</span></span> <span data-ttu-id="0d63b-154">Эти области различаются в зависимости от типа информации, которую необходимо отдемонстрировать.</span><span class="sxs-lookup"><span data-stu-id="0d63b-154">These scopes differ depending on what kind of information you want to show.</span></span> <span data-ttu-id="0d63b-155">В этом случае вам потребуется доступ к календарю людей, а также базовый доступ к сведениям о людей, которые также отображаются в календаре.</span><span class="sxs-lookup"><span data-stu-id="0d63b-155">In this case, you will need access to people's calendar as well as basic access to information about people that is also displayed in the calendar.</span></span> <span data-ttu-id="0d63b-156">Области, необходимые для каждого API, можно найти в документации [по API Microsoft Graph.](/graph/api/overview)</span><span class="sxs-lookup"><span data-stu-id="0d63b-156">You can find the scopes required by each API in the [Microsoft Graph API documentation](/graph/api/overview).</span></span>

1. <span data-ttu-id="0d63b-157">В редакторе кода откройте **файл src/index.tsx** и обновим код инициализации поставщика.</span><span class="sxs-lookup"><span data-stu-id="0d63b-157">In the code editor, open the **src/index.tsx** file, and update the provider initialization code.</span></span>

    ```tsx
    Providers.globalProvider = new MsalProvider({
      clientId: 'd7cb93c9-9097-4e38-8f06-7c0088ac3318',
      scopes: ['calendars.read', 'user.read', 'openid', 'profile', 'people.read', 'user.readbasic.all']
    });
    ```

### <a name="show-users-data-after-signing-in"></a><span data-ttu-id="0d63b-158">Показывать данные пользователя после входов</span><span class="sxs-lookup"><span data-stu-id="0d63b-158">Show user's data after signing in</span></span>

<span data-ttu-id="0d63b-159">Затем расширим приложение, чтобы показать данные из календаря пользователя.</span><span class="sxs-lookup"><span data-stu-id="0d63b-159">Next, extend the application to show data from the user's calendar.</span></span> <span data-ttu-id="0d63b-160">Вы можете получить доступ к этой информации только после того, как пользователь войт.</span><span class="sxs-lookup"><span data-stu-id="0d63b-160">You can access this information only after the user has signed in.</span></span> <span data-ttu-id="0d63b-161">Для этого необходимо отслеживать состояние пользователя при входе и показывать данные календаря после того, как пользователь войт в свою учетную запись Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="0d63b-161">To do this, you will need to track the  user's sign in state and show the calendar data after the user has signed in with their Microsoft account.</span></span>

#### <a name="track-users-sign-in-state"></a><span data-ttu-id="0d63b-162">Отслеживание состояния пользователя при входе</span><span class="sxs-lookup"><span data-stu-id="0d63b-162">Track user's sign in state</span></span>

<span data-ttu-id="0d63b-163">Чтобы отслеживать состояние пользователя при входе в приложение, вы будете использовать React и обработчики в сочетании с обработчиками `useState` `useEffect` событий поставщика.</span><span class="sxs-lookup"><span data-stu-id="0d63b-163">To track the user's sign in state in your application, you will use the React `useState` and `useEffect` hooks in combination with provider event handlers.</span></span>

1. <span data-ttu-id="0d63b-164">В редакторе кода откройте **файл src/App.tsx** и расширйте существующий `import` выписку React.</span><span class="sxs-lookup"><span data-stu-id="0d63b-164">In the code editor, open the **src/App.tsx** file and extend the existing React `import` statement.</span></span>

    ```tsx
    import React, { useState, useEffect } from 'react';
    ```

1. <span data-ttu-id="0d63b-165">Импортировать `Provider` типы и типы из , добавив в `ProviderState` `mgt-element` импорт.</span><span class="sxs-lookup"><span data-stu-id="0d63b-165">Import the `Provider` and `ProviderState` types from `mgt-element`, by adding to imports.</span></span>

    ```tsx
    import { Providers, ProviderState } from '@microsoft/mgt-element';
    ```

1. <span data-ttu-id="0d63b-166">Добавьте пользовательскую функцию с именем, которая позволяет отслеживать состояние пользователя при входе `useIsSignedIn` в приложение.</span><span class="sxs-lookup"><span data-stu-id="0d63b-166">Add a custom function named `useIsSignedIn` that enables tracking the user's sign in state in your application.</span></span>

    ```tsx
    function useIsSignedIn(): [boolean] {
      const [isSignedIn, setIsSignedIn] = useState(false);
    
      useEffect(() => {
        const updateState = () => {
          const provider = Providers.globalProvider;
          setIsSignedIn(provider && provider.state === ProviderState.SignedIn);
        };
    
        Providers.onProviderUpdated(updateState);
        updateState();
    
        return () => {
          Providers.removeProviderUpdatedListener(updateState);
        }
      }, []);
    
      return [isSignedIn];
    }
    ```

<span data-ttu-id="0d63b-167">Эта функция делает две вещи.</span><span class="sxs-lookup"><span data-stu-id="0d63b-167">This function does two things.</span></span> <span data-ttu-id="0d63b-168">Во-первых, с помощью `useState` обцепки React он включает отслеживание состояния в компоненте.</span><span class="sxs-lookup"><span data-stu-id="0d63b-168">First, using the React `useState` hook, it enables tracking state inside your component.</span></span> <span data-ttu-id="0d63b-169">При смене состояния React будет повторно отрисовки компонента.</span><span class="sxs-lookup"><span data-stu-id="0d63b-169">Whenever the state changes, React will re-render your component.</span></span> <span data-ttu-id="0d63b-170">Во-вторых, с помощью обработца React он расширяет жизненный цикл компонента, отслеживая изменения в поставщике набор средств Microsoft Graph и при необходимости обновляя `useEffect` компонент.</span><span class="sxs-lookup"><span data-stu-id="0d63b-170">Second, using the React `useEffect` hook, it extends the component's lifecycle by tracking changes in the Microsoft Graph Toolkit provider and updating the component if necessary.</span></span>

#### <a name="load-users-calendar-if-user-is-signed-in"></a><span data-ttu-id="0d63b-171">Загрузка календаря пользователя, если пользователь в него вписались</span><span class="sxs-lookup"><span data-stu-id="0d63b-171">Load user's calendar if user is signed in</span></span>

<span data-ttu-id="0d63b-172">Теперь, когда вы отслеживаете состояние пользователя в приложении, вы можете отследить его календарь после того, как он войт.</span><span class="sxs-lookup"><span data-stu-id="0d63b-172">Now that you track the user's sign in state in your application, you can show their calendar after they signed in.</span></span>

1. <span data-ttu-id="0d63b-173">В редакторе кода откройте **файл src/App.tsx** и добавьте в функцию **App:**</span><span class="sxs-lookup"><span data-stu-id="0d63b-173">In the code editor, open the **src/App.tsx** file, and inside the **App** function, add:</span></span>

    ```tsx
    const [isSignedIn] = useIsSignedIn();
    ```

    <span data-ttu-id="0d63b-174">Таким образом определяется boolean constant, с помощью которой можно определить, в данный момент ли пользователь вписан `isSignedIn` в приложение.</span><span class="sxs-lookup"><span data-stu-id="0d63b-174">This defines a Boolean `isSignedIn` constant, which you can use to determine whether the user is currently signed in to your application.</span></span>

1. <span data-ttu-id="0d63b-175">Расширим содержимое предложения с помощью дополнительного компонента и компонента `return` `div` Microsoft Graph набор средств Agenda.</span><span class="sxs-lookup"><span data-stu-id="0d63b-175">Extend the contents of the `return` clause with an additional `div` and the Microsoft Graph Toolkit Agenda component.</span></span>

    ```tsx
    <div>
      {isSignedIn &&
        <Agenda />}
    </div>
    ```

<span data-ttu-id="0d63b-176">При этих изменениях **файл src/App.tsx** должен выглядеть следующим образом.</span><span class="sxs-lookup"><span data-stu-id="0d63b-176">With these changes, the **src/App.tsx** file should look like the following.</span></span>

```tsx
import { Providers, ProviderState } from '@microsoft/mgt';
import { Agenda, Login } from '@microsoft/mgt-react';
import React, { useState, useEffect } from 'react';
import './App.css';

function useIsSignedIn(): [boolean] {
  const [isSignedIn, setIsSignedIn] = useState(false);

  useEffect(() => {
    const updateState = () => {
      const provider = Providers.globalProvider;
      setIsSignedIn(provider && provider.state === ProviderState.SignedIn);
    };

    Providers.onProviderUpdated(updateState);
    updateState();

    return () => {
      Providers.removeProviderUpdatedListener(updateState);
    }
  }, []);

  return [isSignedIn];
}

function App() {
  const [isSignedIn] = useIsSignedIn();

  return (
    <div className="App">
      <header>
        <Login />
      </header>
      <div>
        {isSignedIn &&
          <Agenda />}
      </div>
    </div>
  );
}

export default App;
```

### <a name="test-showing-users-calendar-after-they-signed-in"></a><span data-ttu-id="0d63b-177">Тестирование с отображением календаря пользователя после его войки</span><span class="sxs-lookup"><span data-stu-id="0d63b-177">Test showing user's calendar after they signed in</span></span>

<span data-ttu-id="0d63b-178">После внесения этих изменений в приложение с помощью учетной записи Майкрософт вы должны увидеть свой календарь.</span><span class="sxs-lookup"><span data-stu-id="0d63b-178">With these changes, after signing in to your application with your Microsoft account, you should see your calendar.</span></span>

1. <span data-ttu-id="0d63b-179">Чтобы увидеть изменения, закроем браузер и снова откройте его и перейдите к `http://localhost:3000` .</span><span class="sxs-lookup"><span data-stu-id="0d63b-179">To see the changes, close the browser and open it again, and go to `http://localhost:3000`.</span></span> <span data-ttu-id="0d63b-180">Это необходимо, так как вы изменили значение свойства, что влияет на маркер `scopes` доступа, запрашиваемого из Azure AD.</span><span class="sxs-lookup"><span data-stu-id="0d63b-180">You do this because you changed the value of the `scopes` property, which affects the access token that you request from Azure AD.</span></span>
1. <span data-ttu-id="0d63b-181">Choose the **Sign In** button and sign in using your Microsoft account.</span><span class="sxs-lookup"><span data-stu-id="0d63b-181">Choose the **Sign In** button and sign in using your Microsoft account.</span></span> <span data-ttu-id="0d63b-182">Обратите внимание на дополнения к списку разрешений, запрашиваемого в запросе согласия.</span><span class="sxs-lookup"><span data-stu-id="0d63b-182">Notice the additions to the list of permissions requested in the consent prompt.</span></span> <span data-ttu-id="0d63b-183">Это необходимо из-за того, что вы включили дополнительные разрешения в `scope` свойство.</span><span class="sxs-lookup"><span data-stu-id="0d63b-183">This is because you included additional permissions in the `scope` property.</span></span>
1. <span data-ttu-id="0d63b-184">После согласия на использование приложения вы должны увидеть сведения о текущем пользователе и его календаре.</span><span class="sxs-lookup"><span data-stu-id="0d63b-184">After consenting to the use of the application, you should see information about the current user and their calendar.</span></span>

![Готовое приложение](../images/mgt-finished-app.png)

## <a name="next-steps"></a><span data-ttu-id="0d63b-186">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="0d63b-186">Next steps</span></span>

- <span data-ttu-id="0d63b-187">Посмотрите, [что в Microsoft Graph набор средств.](../overview.md)</span><span class="sxs-lookup"><span data-stu-id="0d63b-187">See [what's in the Microsoft Graph Toolkit](../overview.md).</span></span>
- <span data-ttu-id="0d63b-188">Попробуйте компоненты в игровой [области.](https://mgt.dev)</span><span class="sxs-lookup"><span data-stu-id="0d63b-188">Try out the components in the [playground](https://mgt.dev).</span></span>
- <span data-ttu-id="0d63b-189">Задайте вопрос на [сайте Stack Overflow.](https://aka.ms/mgt-question)</span><span class="sxs-lookup"><span data-stu-id="0d63b-189">Ask a question on [Stack Overflow](https://aka.ms/mgt-question).</span></span>
- <span data-ttu-id="0d63b-190">Сообщать об ошибках или оставлять запрос на функции на [GitHub.](https://aka.ms/mgt)</span><span class="sxs-lookup"><span data-stu-id="0d63b-190">Report bugs or leave a feature request on [GitHub](https://aka.ms/mgt).</span></span>
