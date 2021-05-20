---
title: Использование Microsoft Graph Toolkit с React
description: Начало использования Microsoft Graph Toolkit в приложении React
localization_priority: Normal
author: waldekmastykarz
ms.openlocfilehash: a1eaf17b4d4b12e04c11941ab25c5e2bdfd6d57a
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579776"
---
# <a name="use-the-microsoft-graph-toolkit-with-react"></a><span data-ttu-id="1b896-103">Использование Microsoft Graph Toolkit с React</span><span class="sxs-lookup"><span data-stu-id="1b896-103">Use the Microsoft Graph Toolkit with React</span></span>

<span data-ttu-id="1b896-104">Microsoft Graph Toolkit — это набор веб-компонентов, которые упрощают подключение к Microsoft Graph и позволяют вам сосредоточиться на своем приложении.</span><span class="sxs-lookup"><span data-stu-id="1b896-104">Microsoft Graph Toolkit is a set of web components that simplify connecting to Microsoft Graph and allow you to focus on your application instead.</span></span> <span data-ttu-id="1b896-105">Microsoft Graph Toolkit доступен как общий набор веб-компонентов, распространяемых через пакет NPM `@microsoft/mgt`.</span><span class="sxs-lookup"><span data-stu-id="1b896-105">Microsoft Graph Toolkit is available as a generic set of web components distributed through the `@microsoft/mgt` npm package.</span></span>

<span data-ttu-id="1b896-106">Если вы создаете приложения с помощью React, вы можете использовать [пакет `@microsoft/mgt-react`](./mgt-react.md), который упаковывает веб-компоненты Microsoft Graph Toolkit в компоненты React и упрощает передачу сложных данных.</span><span class="sxs-lookup"><span data-stu-id="1b896-106">If you're building apps with React, you can use the [`@microsoft/mgt-react` package](./mgt-react.md), which wraps Microsoft Graph Toolkit web components in React components and makes it easier to pass complex data.</span></span>

<span data-ttu-id="1b896-107">В этой статье описывается пошаговый процесс использования Microsoft Graph Toolkit для создания приложения React и подключения его к Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="1b896-107">This article describes the step-by-step process of using the Microsoft Graph Toolkit to create a React app and connect it to Microsoft 365.</span></span> <span data-ttu-id="1b896-108">После выполнения всех шагов у вас получится приложение React, которое показывает предстоящие встречи пользователя, вошедшего в систему в Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="1b896-108">After completing the steps, you'll have a React app that shows the upcoming appointments of the currently signed in user from Microsoft 365.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1b896-109">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="1b896-109">Prerequisites</span></span>

<span data-ttu-id="1b896-110">Чтобы выполнить действия, описанные в этой статье, вам понадобится среда разработки Microsoft 365 и несколько инструментов.</span><span class="sxs-lookup"><span data-stu-id="1b896-110">To follow the steps in this article, you'll need a Microsoft 365 development environment and a few tools.</span></span> <span data-ttu-id="1b896-111">Дополнительные сведения см. в разделе [Приступая к работе](./overview.md).</span><span class="sxs-lookup"><span data-stu-id="1b896-111">For details, see [getting started](./overview.md).</span></span>

## <a name="create-a-react-app"></a><span data-ttu-id="1b896-112">Создание приложения React</span><span class="sxs-lookup"><span data-stu-id="1b896-112">Create a React app</span></span>

<span data-ttu-id="1b896-113">Создайте приложение React, выполнив следующую команду.</span><span class="sxs-lookup"><span data-stu-id="1b896-113">Create a new React app by running the following command.</span></span> <span data-ttu-id="1b896-114">Это создаст новое приложение React с использованием TypeScript, что поможет написать более функциональный код и избежать ошибок выполнения.</span><span class="sxs-lookup"><span data-stu-id="1b896-114">This will create a new React app using TypeScript, which will help you write more robust code and avoid runtime errors.</span></span>

```cmd
npx create-react-app my-m365-app --template typescript --use-npm
```

<span data-ttu-id="1b896-115">Измените рабочий каталог на только что созданное приложение.</span><span class="sxs-lookup"><span data-stu-id="1b896-115">Change the working directory to the newly created app.</span></span>

```cmd
cd my-m365-app
```

<span data-ttu-id="1b896-116">Затем установите пакет NPM `mgt-react`, который содержит компоненты Microsoft Graph Toolkit для React.</span><span class="sxs-lookup"><span data-stu-id="1b896-116">Next, install the `mgt-react` npm package, which contains the Microsoft Graph Toolkit React components.</span></span>

```cmd
npm i @microsoft/mgt-react
```

<span data-ttu-id="1b896-117">Установите и пакет npm, который содержит `mgt-msal2-provider` `mgt-element` поставщика auth MSAL 2.0.</span><span class="sxs-lookup"><span data-stu-id="1b896-117">Install the `mgt-msal2-provider` and `mgt-element` npm package as well, which contains the MSAL 2.0 auth provider.</span></span>

```cmd
npm i @microsoft/mgt-element @microsoft/mgt-msal2-provider
```

<span data-ttu-id="1b896-118">Подтвердите, что вы можете запустить приложение.</span><span class="sxs-lookup"><span data-stu-id="1b896-118">Confirm that you can run the app.</span></span>

```cmd
npm start
```

<span data-ttu-id="1b896-119">У вас должна быть возможность открыть приложение в браузере через `http://localhost:3000`.</span><span class="sxs-lookup"><span data-stu-id="1b896-119">You should be able to open your app in the browser via `http://localhost:3000`.</span></span>

[!INCLUDE [AAD with implicit flow app registration](../includes/aad-app-registration-spa.md)]

## <a name="connect-react-app-to-microsoft-365"></a><span data-ttu-id="1b896-120">Подключение приложения React к Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="1b896-120">Connect React app to Microsoft 365</span></span>

<span data-ttu-id="1b896-121">Теперь, когда вы зарегистрировали свое приложение в Azure Active Directory (Azure AD), вы можете подключить приложение React к Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="1b896-121">Now that you have registered your application with Azure Active Directory (Azure AD), you can connect the React app to Microsoft 365.</span></span> <span data-ttu-id="1b896-122">Для начала разрешите пользователям входить в приложение при помощи учетной записи Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="1b896-122">First, allow users to sign in to the app using their Microsoft account.</span></span>

### <a name="copy-the-azure-ad-application-registration-id"></a><span data-ttu-id="1b896-123">Скопируйте идентификатор регистрации приложения в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="1b896-123">Copy the Azure AD application registration ID</span></span>

1. <span data-ttu-id="1b896-124">На портале Azure перейдите к регистрации приложения.</span><span class="sxs-lookup"><span data-stu-id="1b896-124">In the Azure Portal, go to your application registration.</span></span>
1. <span data-ttu-id="1b896-125">Убедитесь, что вы находитесь на странице **Обзор**.</span><span class="sxs-lookup"><span data-stu-id="1b896-125">Verify that you are on the **Overview** page.</span></span>
1. <span data-ttu-id="1b896-126">Скопируйте значение свойства **Идентификатор приложения (клиента)** из раздела **Основное**. </span><span class="sxs-lookup"><span data-stu-id="1b896-126">From the **Essentials** section, copy the value of the **Application (client) ID** property</span></span>

### <a name="configure-the-microsoft-graph-toolkit-authentication-provider"></a><span data-ttu-id="1b896-127">Настройка поставщика проверки подлинности Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="1b896-127">Configure the Microsoft Graph Toolkit authentication provider</span></span>

<span data-ttu-id="1b896-128">Теперь настройте поставщика проверки подлинности, который должен использовать Microsoft Graph Toolkit.</span><span class="sxs-lookup"><span data-stu-id="1b896-128">Next, configure the authentication provider that the Microsoft Graph Toolkit should use.</span></span> <span data-ttu-id="1b896-129">В этом случае будет использоваться MSAL, который по умолчанию подходит для создания автономных приложений.</span><span class="sxs-lookup"><span data-stu-id="1b896-129">In this case, you'll use MSAL, which is a good default for building standalone applications.</span></span> <span data-ttu-id="1b896-130">Если вы используете какие-либо точки расширения в Microsoft 365, например Teams или SharePoint, то необходимо будет выбрать [других поставщиков](../providers/providers.md).</span><span class="sxs-lookup"><span data-stu-id="1b896-130">If you use any of the extensibility points in Microsoft 365, like Teams or SharePoint, you will use [other providers](../providers/providers.md).</span></span>

>[!NOTE] 
><span data-ttu-id="1b896-131">Если вы в настоящее время используете поставщика MSAL и хотите обновить поставщика MSAL 2, выполните действия в статье [поставщика MSAL 2.](../providers/msal2.md#migrating-from-msal-provider-to-msal-2-provider)</span><span class="sxs-lookup"><span data-stu-id="1b896-131">If you are currently using MSAL Provider and would like to update to the MSAL 2 Provider, follow the steps in the [MSAL 2 provider](../providers/msal2.md#migrating-from-msal-provider-to-msal-2-provider) article.</span></span>

1. <span data-ttu-id="1b896-132">Откройте в редакторе кода файл **src/index.**</span><span class="sxs-lookup"><span data-stu-id="1b896-132">In the code editor, open the **src/index.**</span></span> <span data-ttu-id="1b896-133">и добавьте в список операций импорта следующее:</span><span class="sxs-lookup"><span data-stu-id="1b896-133">file, and to the list of imports, add:</span></span>

    ```tsx
    import { Providers } from '@microsoft/mgt-element';
    import { Msal2Provider } from '@microsoft/mgt-msal2-provider';
    ```

1. <span data-ttu-id="1b896-134">После последнего оператора `import` инициализируйте Microsoft Graph Toolkit с помощью поставщика MSAL.</span><span class="sxs-lookup"><span data-stu-id="1b896-134">After the last `import` statement, initialize the Microsoft Graph Toolkit with MSAL provider.</span></span>

    ```tsx
    Providers.globalProvider = new Msal2Provider({
      clientId: 'REPLACE_WITH_CLIENTID'
    });
    ```

    <span data-ttu-id="1b896-135">Замените значение свойства `clientId` значением свойства `Application (client) ID`, которое вы ранее скопировали на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="1b896-135">Replace the value of the `clientId` property with the value of the `Application (client) ID` property you copied previously in the Azure Portal.</span></span>

<span data-ttu-id="1b896-136">С этими изменениями файл **src/index.tsx** будет выглядеть следующим образом.</span><span class="sxs-lookup"><span data-stu-id="1b896-136">With these changes, the **src/index.tsx** file will look like the following.</span></span>

  ```tsx
  import React from 'react';
  import ReactDOM from 'react-dom';
  import App from './App';
  import './index.css';
  import * as serviceWorker from './serviceWorker';

  import { Providers } from '@microsoft/mgt-element';
  import { Msal2Provider } from '@microsoft/mgt-msal2-provider';
  
  Providers.globalProvider = new Msal2Provider({
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

### <a name="add-the-sign-in-button"></a><span data-ttu-id="1b896-137">Добавление кнопки входа</span><span class="sxs-lookup"><span data-stu-id="1b896-137">Add the Sign in button</span></span>

<span data-ttu-id="1b896-138">Добавьте компонент Microsoft Graph Toolkit для React под названием **Вход**, отображающий кнопку **Войти**, которую пользователи смогут использовать для входа в ваше приложение со своей учетной записью Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="1b896-138">Add the **Login** Microsoft Graph Toolkit React component, which will display the **Sign in** button people can use to sign in with their Microsoft account to your app.</span></span>

1. <span data-ttu-id="1b896-139">Откройте в редакторе кода файл **src/App.tsx** и добавьте в список операций импорта следующее:</span><span class="sxs-lookup"><span data-stu-id="1b896-139">In the code editor, open the **src/App.tsx** file, and to the list of imports add:</span></span>

    ```tsx
    import { Login } from '@microsoft/mgt-react';
    ```

1. <span data-ttu-id="1b896-140">В функции `App` замените содержимое пункта `return` базовой структурой, включая компонент входа Microsoft Graph Toolkit:</span><span class="sxs-lookup"><span data-stu-id="1b896-140">In the `App` function, replace the contents of the `return` clause with the basic structure including the Microsoft Graph Toolkit Login component:</span></span>

    ```tsx
    <div className="App">
      <header>
        <Login />
      </header>
    </div>
    ```

<span data-ttu-id="1b896-141">С этими изменениями файл **src/App.tsx** будет выглядеть следующим образом.</span><span class="sxs-lookup"><span data-stu-id="1b896-141">With these changes, the **src/App.tsx** file will look like the following.</span></span>
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

### <a name="test-signing-in-to-your-application"></a><span data-ttu-id="1b896-142">Тестирование входа в приложение</span><span class="sxs-lookup"><span data-stu-id="1b896-142">Test signing in to your application</span></span>

<span data-ttu-id="1b896-143">Теперь вы можете входить в приложение с помощью своей учетной записи Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="1b896-143">You should now be able to sign in to your application with your Microsoft account.</span></span>

1. <span data-ttu-id="1b896-144">Вернитесь в браузер, в котором выполняется ваше приложение React.</span><span class="sxs-lookup"><span data-stu-id="1b896-144">Go back to the browser where your React app is running.</span></span> <span data-ttu-id="1b896-145">Теперь вы должны видеть кнопку **Войти**.</span><span class="sxs-lookup"><span data-stu-id="1b896-145">You should now see a **Sign in** button.</span></span>
1. <span data-ttu-id="1b896-146">При нажатии кнопки **Войти** вам будет предложено войти в систему с помощью учетной записи Майкрософт. Вы можете использовать ту же учетную запись, с помощью которой заходили на портал Azure.</span><span class="sxs-lookup"><span data-stu-id="1b896-146">When you click the **Sign in** button, you will be prompted to sign in with your Microsoft account (you can use the same account as the one you accessed the Azure Portal with).</span></span>
1. <span data-ttu-id="1b896-147">Так как это приложение Azure AD используется впервые, вам необходимо дать согласие на его использование в вашей организации.</span><span class="sxs-lookup"><span data-stu-id="1b896-147">Because this is the first time you're using this Azure AD application, you need to consent its use in your organization.</span></span>
1. <span data-ttu-id="1b896-148">После входа в систему вы будете перенаправлены в приложение React.</span><span class="sxs-lookup"><span data-stu-id="1b896-148">After signing in, you will be redirected to your React app.</span></span> <span data-ttu-id="1b896-149">Обратите внимание, что кнопка **Войти** изменилась и теперь показывает ваше имя пользователя ![Приложение React отображает информацию о пользователе, полученную из Microsoft 365 с помощью Microsoft Graph Toolkit](../images/mgt-react-userinfo.png).</span><span class="sxs-lookup"><span data-stu-id="1b896-149">Notice that the **Sign in** button changed to show your user's name ![React app showing user info retrieved from Microsoft 365 using Microsoft Graph Toolkit](../images/mgt-react-userinfo.png).</span></span>

## <a name="load-data-from-microsoft-365"></a><span data-ttu-id="1b896-150">Загрузка данных из Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="1b896-150">Load data from Microsoft 365</span></span>

<span data-ttu-id="1b896-151">Microsoft Graph Toolkit не только упрощает проверку подлинности при входе в Microsoft 365, но и загружает его данные.</span><span class="sxs-lookup"><span data-stu-id="1b896-151">Microsoft Graph Toolkit not only simplifies authentication to Microsoft 365, but also loading its data.</span></span> <span data-ttu-id="1b896-152">В этом примере будет показан календарь пользователя, вошедшего в систему.</span><span class="sxs-lookup"><span data-stu-id="1b896-152">In this example, you'll show the signed in person's calendar.</span></span>

### <a name="specify-permissions-needed-for-your-application"></a><span data-ttu-id="1b896-153">Определение разрешений, необходимых для вашего приложения</span><span class="sxs-lookup"><span data-stu-id="1b896-153">Specify permissions needed for your application</span></span>

<span data-ttu-id="1b896-154">Прежде чем вы сможете загружать данные из Microsoft 365, необходимо определить список областей разрешений, которые необходимы вашему приложению для получения доступа к данным пользователя.</span><span class="sxs-lookup"><span data-stu-id="1b896-154">Before you can load data from Microsoft 365, you need to specify the list of permission scopes your application must be granted to access user's data.</span></span> <span data-ttu-id="1b896-155">Эти области различаются в зависимости от того, какую информацию вы хотите показать.</span><span class="sxs-lookup"><span data-stu-id="1b896-155">These scopes differ depending on what kind of information you want to show.</span></span> <span data-ttu-id="1b896-156">В этом случае понадобится доступ к календарю пользователей, а также базовый доступ к информации о пользователях, которая также отображается в календаре.</span><span class="sxs-lookup"><span data-stu-id="1b896-156">In this case, you will need access to people's calendar as well as basic access to information about people that is also displayed in the calendar.</span></span> <span data-ttu-id="1b896-157">Области разрешений, необходимые для каждого API, можно найти в [документации API Microsoft Graph](/graph/api/overview).</span><span class="sxs-lookup"><span data-stu-id="1b896-157">You can find the scopes required by each API in the [Microsoft Graph API documentation](/graph/api/overview).</span></span>

1. <span data-ttu-id="1b896-158">Откройте в редакторе кода файл **src/index.tsx** и обновите код инициализации поставщика.</span><span class="sxs-lookup"><span data-stu-id="1b896-158">In the code editor, open the **src/index.tsx** file, and update the provider initialization code.</span></span>

    ```tsx
    Providers.globalProvider = new Msal2Provider({
      clientId: 'REPLACE_WITH_CLIENTID',
      scopes: ['calendars.read', 'user.read', 'openid', 'profile', 'people.read', 'user.readbasic.all']
    });
    ```

### <a name="show-users-data-after-signing-in"></a><span data-ttu-id="1b896-159">Отображение данных пользователя после входа в систему</span><span class="sxs-lookup"><span data-stu-id="1b896-159">Show user's data after signing in</span></span>

<span data-ttu-id="1b896-160">Теперь дополните приложение, чтобы оно отображало данные из календаря пользователя.</span><span class="sxs-lookup"><span data-stu-id="1b896-160">Next, extend the application to show data from the user's calendar.</span></span> <span data-ttu-id="1b896-161">Доступ к этой информации можно получить только после того, как пользователь вошел в систему.</span><span class="sxs-lookup"><span data-stu-id="1b896-161">You can access this information only after the user has signed in.</span></span> <span data-ttu-id="1b896-162">Для этого необходимо отслеживать, находится ли пользователь в системе, и отображать данные календаря только после того, как пользователь вошел в систему с помощью своей учетной записи Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="1b896-162">To do this, you will need to track the  user's sign in state and show the calendar data after the user has signed in with their Microsoft account.</span></span>

#### <a name="track-users-sign-in-state"></a><span data-ttu-id="1b896-163">Отслеживание состояния входа пользователя в систему</span><span class="sxs-lookup"><span data-stu-id="1b896-163">Track user's sign in state</span></span>

<span data-ttu-id="1b896-164">Для отслеживания состояния входа пользователя в приложение будет использоваться обработчики React `useState` и `useEffect` в сочетании с обработчиками событий провайдера.</span><span class="sxs-lookup"><span data-stu-id="1b896-164">To track the user's sign in state in your application, you will use the React `useState` and `useEffect` hooks in combination with provider event handlers.</span></span>

1. <span data-ttu-id="1b896-165">Откройте в редакторе кода файл **src/App.tsx** и дополните существующий оператор React `import`.</span><span class="sxs-lookup"><span data-stu-id="1b896-165">In the code editor, open the **src/App.tsx** file and extend the existing React `import` statement.</span></span>

    ```tsx
    import React, { useState, useEffect } from 'react';
    ```

1. <span data-ttu-id="1b896-166">Импортируйте типы `Provider` и `ProviderState` из `mgt-element`, добавив их в операции импорта.</span><span class="sxs-lookup"><span data-stu-id="1b896-166">Import the `Provider` and `ProviderState` types from `mgt-element`, by adding to imports.</span></span>

    ```tsx
    import { Providers, ProviderState } from '@microsoft/mgt-element';
    ```

1. <span data-ttu-id="1b896-167">Добавьте настраиваемую функцию с именем `useIsSignedIn`, которая позволяет отслеживать состояние входа пользователя в приложение.</span><span class="sxs-lookup"><span data-stu-id="1b896-167">Add a custom function named `useIsSignedIn` that enables tracking the user's sign in state in your application.</span></span>

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

<span data-ttu-id="1b896-168">Эта функция выполняет два действия.</span><span class="sxs-lookup"><span data-stu-id="1b896-168">This function does two things.</span></span> <span data-ttu-id="1b896-169">Во-первых, с помощью обработчика React `useState` она позволяет отслеживать состояние внутри компонента.</span><span class="sxs-lookup"><span data-stu-id="1b896-169">First, using the React `useState` hook, it enables tracking state inside your component.</span></span> <span data-ttu-id="1b896-170">При каждом изменении состояния React повторно отображает ваш компонент.</span><span class="sxs-lookup"><span data-stu-id="1b896-170">Whenever the state changes, React will re-render your component.</span></span> <span data-ttu-id="1b896-171">Во-вторых, с помощью обработчика React `useEffect` она продлевает жизненный цикл компонента, отслеживая изменения в поставщике Microsoft Graph Toolkit и обновляя компонент при необходимости.</span><span class="sxs-lookup"><span data-stu-id="1b896-171">Second, using the React `useEffect` hook, it extends the component's lifecycle by tracking changes in the Microsoft Graph Toolkit provider and updating the component if necessary.</span></span>

#### <a name="load-users-calendar-if-user-is-signed-in"></a><span data-ttu-id="1b896-172">Загрузка календаря пользователя, вошедшего в систему</span><span class="sxs-lookup"><span data-stu-id="1b896-172">Load user's calendar if user is signed in</span></span>

<span data-ttu-id="1b896-173">Теперь, когда отслеживается состояние входа пользователя в приложение, вы можете отображать календарь пользователя после входа в систему.</span><span class="sxs-lookup"><span data-stu-id="1b896-173">Now that you track the user's sign in state in your application, you can show their calendar after they signed in.</span></span>

1. <span data-ttu-id="1b896-174">Откройте в редакторе кода файл **src/App.tsx** и внутри функции **Приложение** добавьте следующее:</span><span class="sxs-lookup"><span data-stu-id="1b896-174">In the code editor, open the **src/App.tsx** file, and inside the **App** function, add:</span></span>

    ```tsx
    const [isSignedIn] = useIsSignedIn();
    ```

    <span data-ttu-id="1b896-175">Это определяет логическую константу `isSignedIn`, которую можно использовать для определения, выполнил ли пользователь вход в приложение.</span><span class="sxs-lookup"><span data-stu-id="1b896-175">This defines a Boolean `isSignedIn` constant, which you can use to determine whether the user is currently signed in to your application.</span></span>

1. <span data-ttu-id="1b896-176">В содержимое пункта `return` добавьте `div`, а также компонент расписания Microsoft Graph Toolkit.</span><span class="sxs-lookup"><span data-stu-id="1b896-176">Extend the contents of the `return` clause with an additional `div` and the Microsoft Graph Toolkit Agenda component.</span></span>

    ```tsx
    <div>
      {isSignedIn &&
        <Agenda />}
    </div>
    ```

<span data-ttu-id="1b896-177">С этими изменениями файл **src/App.tsx** будет выглядеть следующим образом.</span><span class="sxs-lookup"><span data-stu-id="1b896-177">With these changes, the **src/App.tsx** file should look like the following.</span></span>

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

### <a name="test-showing-users-calendar-after-they-signed-in"></a><span data-ttu-id="1b896-178">Тестирование отображения календаря пользователя после входа в систему</span><span class="sxs-lookup"><span data-stu-id="1b896-178">Test showing user's calendar after they signed in</span></span>

<span data-ttu-id="1b896-179">С внесением этих изменений вы должны увидеть свой календарь после входа в приложение с учетной записью Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="1b896-179">With these changes, after signing in to your application with your Microsoft account, you should see your calendar.</span></span>

1. <span data-ttu-id="1b896-180">Чтобы увидеть изменения, закройте браузер, откройте его снова и перейдите на `http://localhost:3000`.</span><span class="sxs-lookup"><span data-stu-id="1b896-180">To see the changes, close the browser and open it again, and go to `http://localhost:3000`.</span></span> <span data-ttu-id="1b896-181">Это нужно сделать, потому что вы изменили значение свойства `scopes`, которое влияет на маркер доступа, запрашиваемый из Azure AD.</span><span class="sxs-lookup"><span data-stu-id="1b896-181">You do this because you changed the value of the `scopes` property, which affects the access token that you request from Azure AD.</span></span>
1. <span data-ttu-id="1b896-182">Нажмите кнопку **Войти** и войдите с помощью учетной записи Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="1b896-182">Choose the **Sign In** button and sign in using your Microsoft account.</span></span> <span data-ttu-id="1b896-183">Обратите внимание на новые пункты списка разрешений в запросе на продолжение.</span><span class="sxs-lookup"><span data-stu-id="1b896-183">Notice the additions to the list of permissions requested in the consent prompt.</span></span> <span data-ttu-id="1b896-184">Они появились, так как вы включили в свойство `scope` дополнительные разрешения.</span><span class="sxs-lookup"><span data-stu-id="1b896-184">This is because you included additional permissions in the `scope` property.</span></span>
1. <span data-ttu-id="1b896-185">После подтверждения согласия на использование приложения вы должны увидеть информацию о текущем пользователе и его календаре.</span><span class="sxs-lookup"><span data-stu-id="1b896-185">After consenting to the use of the application, you should see information about the current user and their calendar.</span></span>

![Готовое приложение](../images/mgt-finished-app.png)

## <a name="next-steps"></a><span data-ttu-id="1b896-187">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="1b896-187">Next steps</span></span>

- <span data-ttu-id="1b896-188">Узнать, [что включает Microsoft Graph Toolkit](../overview.md).</span><span class="sxs-lookup"><span data-stu-id="1b896-188">See [what's in the Microsoft Graph Toolkit](../overview.md).</span></span>
- <span data-ttu-id="1b896-189">Воспользуйтесь компонентами в [интерактивной среде](https://mgt.dev).</span><span class="sxs-lookup"><span data-stu-id="1b896-189">Try out the components in the [playground](https://mgt.dev).</span></span>
- <span data-ttu-id="1b896-190">Задавайте вопросы на сайте [Stack Overflow](https://aka.ms/mgt-question).</span><span class="sxs-lookup"><span data-stu-id="1b896-190">Ask a question on [Stack Overflow](https://aka.ms/mgt-question).</span></span>
- <span data-ttu-id="1b896-191">Сообщайте об ошибках и оставляйте запросы на создание функций в [GitHub](https://aka.ms/mgt).</span><span class="sxs-lookup"><span data-stu-id="1b896-191">Report bugs or leave a feature request on [GitHub](https://aka.ms/mgt).</span></span>
