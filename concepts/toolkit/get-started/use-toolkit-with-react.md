---
title: Использование набора средств Microsoft Graph с откликом
description: Приступите к работе с набором инструментов Microsoft Graph в приложении для реагирования.
localization_priority: Normal
author: waldekmastykarz
ms.openlocfilehash: 8f570caf2be4c123bd9a9a93e45a5508029efdee
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48967773"
---
# <a name="use-the-microsoft-graph-toolkit-with-react"></a><span data-ttu-id="6cda3-103">Использование набора средств Microsoft Graph с откликом</span><span class="sxs-lookup"><span data-stu-id="6cda3-103">Use the Microsoft Graph Toolkit with React</span></span>

<span data-ttu-id="6cda3-104">Набор инструментов Microsoft Graph — это набор веб-компонентов, упрощающих подключение к Microsoft Graph и позволяющий сосредоточиться на вашем приложении.</span><span class="sxs-lookup"><span data-stu-id="6cda3-104">Microsoft Graph Toolkit is a set of web components that simplify connecting to Microsoft Graph and allow you to focus on your application instead.</span></span> <span data-ttu-id="6cda3-105">Набор средств Microsoft Graph доступен в качестве универсального набора веб-компонентов, распространяемых через пакет **@microsoft/МГТ** NPM.</span><span class="sxs-lookup"><span data-stu-id="6cda3-105">Microsoft Graph Toolkit is available as a generic set of web components distributed through the **@microsoft/mgt** npm package.</span></span>

<span data-ttu-id="6cda3-106">Если вы создаете приложения с помощью реагирующих, вы можете использовать пакет **@microsoft/МГТ-РЕАКТ** , который упаковывает веб-компоненты набора средств Microsoft Graph в компоненты "реагирующий" и упрощает передачу сложных данных.</span><span class="sxs-lookup"><span data-stu-id="6cda3-106">If you're building apps with React, you can use the **@microsoft/mgt-react** package, which wraps Microsoft Graph Toolkit web components in React components and makes it easier to pass complex data.</span></span>

<span data-ttu-id="6cda3-107">В этой статье описывается пошаговый процесс использования набора средств Microsoft Graph для создания приложения с откликом и его подключения к Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="6cda3-107">This article describes the step-by-step process of using the Microsoft Graph Toolkit to create a React app and connect it to Microsoft 365.</span></span> <span data-ttu-id="6cda3-108">После выполнения этих действий у вас будет приложение с откликом, в котором показаны запланированные встречи пользователя, выполнившего вход в Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="6cda3-108">After completing the steps, you'll have a React app that shows the upcoming appointments of the currently signed in user from Microsoft 365.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6cda3-109">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6cda3-109">Prerequisites</span></span>

<span data-ttu-id="6cda3-110">Для выполнения действий, описанных в этой статье, вам потребуется среда разработки Microsoft 365 и несколько средств.</span><span class="sxs-lookup"><span data-stu-id="6cda3-110">To follow the steps in this article, you'll need a Microsoft 365 development environment and a few tools.</span></span> <span data-ttu-id="6cda3-111">Подробнее: [Начало работы](./overview.md).</span><span class="sxs-lookup"><span data-stu-id="6cda3-111">For details, see [getting started](./overview.md).</span></span>

## <a name="create-a-react-app"></a><span data-ttu-id="6cda3-112">Создание реагирующих приложений</span><span class="sxs-lookup"><span data-stu-id="6cda3-112">Create a React app</span></span>

<span data-ttu-id="6cda3-113">Создайте новое приложение для реагирования, выполнив следующую команду.</span><span class="sxs-lookup"><span data-stu-id="6cda3-113">Create a new React app by running the following command.</span></span> <span data-ttu-id="6cda3-114">При этом будет создано новое Реагируее приложение с использованием TypeScript, которое поможет вам написать более надежный код и избежать ошибок времени выполнения.</span><span class="sxs-lookup"><span data-stu-id="6cda3-114">This will create a new React app using TypeScript, which will help you write more robust code and avoid runtime errors.</span></span>

```cmd
npx create-react-app my-m365-app --template typescript
```

<span data-ttu-id="6cda3-115">Измените рабочий каталог на вновь созданное приложение.</span><span class="sxs-lookup"><span data-stu-id="6cda3-115">Change the working directory to the newly created app.</span></span>

```cmd
cd my-m365-app
```

<span data-ttu-id="6cda3-116">Затем установите пакет управления " **центр** управления NPM", который содержит компоненты, реагирующие на набор инструментов Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="6cda3-116">Next, install the **mgt-react** npm package, which contains the Microsoft Graph Toolkit React components.</span></span>

```cmd
npm i @microsoft/mgt-react
```

<span data-ttu-id="6cda3-117">Подтвердите, что вы можете запустить приложение.</span><span class="sxs-lookup"><span data-stu-id="6cda3-117">Confirm that you can run the app.</span></span>

```cmd
HTTPS=true npm start
```

> [!IMPORTANT]
> <span data-ttu-id="6cda3-118">Чтобы приложение могло пройти проверку подлинности в Microsoft 365, его необходимо запускать на HTTPS.</span><span class="sxs-lookup"><span data-stu-id="6cda3-118">Your app need to run on HTTPS in order to be able to authenticate against Microsoft 365.</span></span> <span data-ttu-id="6cda3-119">Для локального тестирования с помощью сценариев реагирования можно настроить локальный веб-сервер для работы с протоколом HTTPS, задав `HTTPS` для переменной среды значение `true` .</span><span class="sxs-lookup"><span data-stu-id="6cda3-119">For local testing, with the React scripts, you can configure the local web server to run on HTTPS by setting the `HTTPS` environment variable to `true`.</span></span> <span data-ttu-id="6cda3-120">Это можно сделать каждый раз, добавив перед `npm start` командой `HTTPS=true` (работает только в bash) или задав глобальную переменную среды на компьютере.</span><span class="sxs-lookup"><span data-stu-id="6cda3-120">You can do this either each time, by prefixing the `npm start` command with `HTTPS=true` (works only in bash) or by setting the environment variable globally on your computer.</span></span>

<span data-ttu-id="6cda3-121">Вы должны иметь возможность открыть приложение в браузере с помощью `https://localhost:3000` .</span><span class="sxs-lookup"><span data-stu-id="6cda3-121">You should be able to open your app in the browser via `https://localhost:3000`.</span></span>

[!INCLUDE [AAD with implicit flow app registration](../includes/aad-app-registration-spa.md)]

## <a name="connect-react-app-to-microsoft-365"></a><span data-ttu-id="6cda3-122">Подключение приложения, реагирующий на реагирование, в Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="6cda3-122">Connect React app to Microsoft 365</span></span>

<span data-ttu-id="6cda3-123">Теперь, когда вы зарегистрировали свое приложение с помощью Azure Active Directory (Azure AD), вы можете подключить приложение, реагируя к Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="6cda3-123">Now that you have registered your application with Azure Active Directory (Azure AD), you can connect the React app to Microsoft 365.</span></span> <span data-ttu-id="6cda3-124">Для начала разрешите пользователям входить в приложение с помощью учетной записи Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="6cda3-124">First, allow users to sign in to the app using their Microsoft account.</span></span>

### <a name="copy-the-azure-ad-application-registration-id"></a><span data-ttu-id="6cda3-125">Копирование идентификатора регистрации приложения Azure AD</span><span class="sxs-lookup"><span data-stu-id="6cda3-125">Copy the Azure AD application registration ID</span></span>

1. <span data-ttu-id="6cda3-126">На портале Azure перейдите к регистрационному приложению.</span><span class="sxs-lookup"><span data-stu-id="6cda3-126">In the Azure Portal, go to your application registration.</span></span>
1. <span data-ttu-id="6cda3-127">Убедитесь, что вы используете страницу **Обзор** .</span><span class="sxs-lookup"><span data-stu-id="6cda3-127">Verify that you are on the **Overview** page.</span></span>
1. <span data-ttu-id="6cda3-128">В разделе **Essentials (основные** сведения) скопируйте значение свойства **ID Application (Client)** .</span><span class="sxs-lookup"><span data-stu-id="6cda3-128">From the **Essentials** section, copy the value of the **Application (client) ID** property</span></span>

### <a name="configure-the-microsoft-graph-toolkit-authentication-provider"></a><span data-ttu-id="6cda3-129">Настройка поставщика проверки подлинности набора средств Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="6cda3-129">Configure the Microsoft Graph Toolkit authentication provider</span></span>

<span data-ttu-id="6cda3-130">Затем настройте поставщика проверки подлинности, который должен использовать набор средств Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="6cda3-130">Next, configure the authentication provider that the Microsoft Graph Toolkit should use.</span></span> <span data-ttu-id="6cda3-131">В этом случае вы будете использовать MSAL, который является хорошим значением по умолчанию для создания автономных приложений.</span><span class="sxs-lookup"><span data-stu-id="6cda3-131">In this case, you'll use MSAL, which is a good default for building standalone applications.</span></span> <span data-ttu-id="6cda3-132">Если вы используете любую из точек расширения Microsoft 365, таких как teams или SharePoint, вы будете использовать [других поставщиков](../providers.md).</span><span class="sxs-lookup"><span data-stu-id="6cda3-132">If you use any of the extensibility points in Microsoft 365, like Teams or SharePoint, you will use [other providers](../providers.md).</span></span>

1. <span data-ttu-id="6cda3-133">В редакторе кода откройте **src/индекс.**</span><span class="sxs-lookup"><span data-stu-id="6cda3-133">In the code editor, open the **src/index.**</span></span> <span data-ttu-id="6cda3-134">файл и в список импортов добавьте:</span><span class="sxs-lookup"><span data-stu-id="6cda3-134">file, and to the list of imports, add:</span></span>

    ```tsx
    import { MsalProvider, Providers } from '@microsoft/mgt';
    ```

1. <span data-ttu-id="6cda3-135">После последнего `import` оператора инициализируйте набор инструментов Microsoft Graph с помощью поставщика MSAL.</span><span class="sxs-lookup"><span data-stu-id="6cda3-135">After the last `import` statement, initialize the Microsoft Graph Toolkit with MSAL provider.</span></span>

    ```tsx
    Providers.globalProvider = new MsalProvider({
      clientId: 'REPLACE_WITH_CLIENTID'
    });
    ```

    <span data-ttu-id="6cda3-136">Замените значение `clientId` Свойства на значение, `Application (client) ID` скопированное ранее на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="6cda3-136">Replace the value of the `clientId` property with the value of the `Application (client) ID` property you copied previously in the Azure Portal.</span></span>

<span data-ttu-id="6cda3-137">В результате этих изменений файл **src/index. Целевой** файл будет выглядеть так, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="6cda3-137">With these changes, the **src/index.tsx** file will look like the following.</span></span>

  ```tsx
  import { MsalProvider, Providers } from '@microsoft/mgt';
  import React from 'react';
  import ReactDOM from 'react-dom';
  import App from './App';
  import './index.css';
  import * as serviceWorker from './serviceWorker';
  
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

### <a name="add-the-sign-in-button"></a><span data-ttu-id="6cda3-138">Добавление кнопки входа</span><span class="sxs-lookup"><span data-stu-id="6cda3-138">Add the Sign in button</span></span>

<span data-ttu-id="6cda3-139">Добавьте для **входа** компонент "реакция на Office Graph Toolkit", в котором будет отображаться кнопка **входа** пользователи могут использовать для входа в приложение с помощью своей учетной записи Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="6cda3-139">Add the **Login** Microsoft Graph Toolkit React component, which will display the **Sign in** button people can use to sign in with their Microsoft account to your app.</span></span>

1. <span data-ttu-id="6cda3-140">В редакторе кода откройте файл **src/App. Целевой** файл и добавьте в список импортируемых компонентов:</span><span class="sxs-lookup"><span data-stu-id="6cda3-140">In the code editor, open the **src/App.tsx** file, and to the list of imports add:</span></span>

    ```tsx
    import { Login } from '@microsoft/mgt-react';
    ```

1. <span data-ttu-id="6cda3-141">В `App` функции замените содержимое `return` предложения основной структурой, включая компонент входа Microsoft Graph Toolkit:</span><span class="sxs-lookup"><span data-stu-id="6cda3-141">In the `App` function, replace the contents of the `return` clause with the basic structure including the Microsoft Graph Toolkit Login component:</span></span>

    ```tsx
    <div className="App">
      <header>
        <Login />
      </header>
    </div>
    ```

<span data-ttu-id="6cda3-142">В результате этих изменений файл **src/App. Целевой** файл будет выглядеть так, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="6cda3-142">With these changes, the **src/App.tsx** file will look like the following.</span></span>
```tsx
import { MsalProvider, Providers } from '@microsoft/mgt';
import { Login } from '@microsoft/mgt-react';
import React from 'react';
import './App.css';

function App() {
  Providers.globalProvider = new MsalProvider({
    clientId: 'REPLACE_WITH_CLIENTID'
  });

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

### <a name="test-signing-in-to-your-application"></a><span data-ttu-id="6cda3-143">Проверка входа в приложение</span><span class="sxs-lookup"><span data-stu-id="6cda3-143">Test signing in to your application</span></span>

<span data-ttu-id="6cda3-144">Теперь вы можете войти в приложение с помощью учетной записи Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="6cda3-144">You should now be able to sign in to your application with your Microsoft account.</span></span>

1. <span data-ttu-id="6cda3-145">Вернитесь в браузер, где запущено работающее приложение.</span><span class="sxs-lookup"><span data-stu-id="6cda3-145">Go back to the browser where your React app is running.</span></span> <span data-ttu-id="6cda3-146">Теперь должна появиться кнопка **войти** .</span><span class="sxs-lookup"><span data-stu-id="6cda3-146">You should now see a **Sign in** button.</span></span>
1. <span data-ttu-id="6cda3-147">При нажатии кнопки **входа** вам будет предложено войти с помощью учетной записи Майкрософт (вы можете использовать ту же учетную запись, что и у вас есть доступ к порталу Azure).</span><span class="sxs-lookup"><span data-stu-id="6cda3-147">When you click the **Sign in** button, you will be prompted to sign in with your Microsoft account (you can use the same account as the one you accessed the Azure Portal with).</span></span>
1. <span data-ttu-id="6cda3-148">Так как вы впервые используете это приложение Azure AD, вам необходимо согласиться с его использованием в вашей организации.</span><span class="sxs-lookup"><span data-stu-id="6cda3-148">Because this is the first time you're using this Azure AD application, you need to consent its use in your organization.</span></span>
1. <span data-ttu-id="6cda3-149">После входа вы будете перенаправлены в приложение, используемое для реагирования.</span><span class="sxs-lookup"><span data-stu-id="6cda3-149">After signing in, you will be redirected to your React app.</span></span> <span data-ttu-id="6cda3-150">Обратите внимание, что кнопка **входа** изменилась, отображая имя пользователя, на ![ котором отображаются сведения о пользователе, полученные из Microsoft 365 с помощью набора средств Microsoft Graph ](../images/mgt-react-userinfo.png) .</span><span class="sxs-lookup"><span data-stu-id="6cda3-150">Notice that the **Sign in** button changed to show your user's name ![React app showing user info retrieved from Microsoft 365 using Microsoft Graph Toolkit](../images/mgt-react-userinfo.png).</span></span>

## <a name="load-data-from-microsoft-365"></a><span data-ttu-id="6cda3-151">Загрузка данных из Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="6cda3-151">Load data from Microsoft 365</span></span>

<span data-ttu-id="6cda3-152">Набор средств Microsoft Graph не только упрощает проверку подлинности в Microsoft 365, но и загрузку данных.</span><span class="sxs-lookup"><span data-stu-id="6cda3-152">Microsoft Graph Toolkit not only simplifies authentication to Microsoft 365, but also loading its data.</span></span> <span data-ttu-id="6cda3-153">В этом примере показано, как Показать календарь пользователя, выполнившего вход.</span><span class="sxs-lookup"><span data-stu-id="6cda3-153">In this example, you'll show the signed in person's calendar.</span></span>

### <a name="specify-permissions-needed-for-your-application"></a><span data-ttu-id="6cda3-154">Указание разрешений, необходимых для приложения</span><span class="sxs-lookup"><span data-stu-id="6cda3-154">Specify permissions needed for your application</span></span>

<span data-ttu-id="6cda3-155">Перед загрузкой данных из Microsoft 365 необходимо указать список областей разрешений, которые должно быть назначено вашему приложению для доступа к данным пользователя.</span><span class="sxs-lookup"><span data-stu-id="6cda3-155">Before you can load data from Microsoft 365, you need to specify the list of permission scopes your application must be granted to access user's data.</span></span> <span data-ttu-id="6cda3-156">Эти области различаются в зависимости от типа информации, которую вы хотите показать.</span><span class="sxs-lookup"><span data-stu-id="6cda3-156">These scopes differ depending on what kind of information you want to show.</span></span> <span data-ttu-id="6cda3-157">В этом случае необходим доступ к календарю пользователей, а также к основному доступу к сведениям о пользователях, которые также отображаются в календаре.</span><span class="sxs-lookup"><span data-stu-id="6cda3-157">In this case, you will need access to people's calendar as well as basic access to information about people that is also displayed in the calendar.</span></span> <span data-ttu-id="6cda3-158">Вы можете найти области, необходимые для каждого API, в [документации по API Microsoft Graph](/graph/api/overview?toc=.%2Fref%2Ftoc.json&view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="6cda3-158">You can find the scopes required by each API in the [Microsoft Graph API documentation](/graph/api/overview?toc=.%2Fref%2Ftoc.json&view=graph-rest-1.0).</span></span>

1. <span data-ttu-id="6cda3-159">В редакторе кода откройте файл **src/index. Целевой** файл и обновите код инициализации поставщика.</span><span class="sxs-lookup"><span data-stu-id="6cda3-159">In the code editor, open the **src/index.tsx** file, and update the provider initialization code.</span></span>

    ```tsx
    Providers.globalProvider = new MsalProvider({
      clientId: 'd7cb93c9-9097-4e38-8f06-7c0088ac3318',
      scopes: ['calendars.read', 'user.read', 'openid', 'profile', 'people.read', 'user.readbasic.all']
    });
    ```

### <a name="show-users-data-after-signing-in"></a><span data-ttu-id="6cda3-160">Отображение данных пользователя после входа</span><span class="sxs-lookup"><span data-stu-id="6cda3-160">Show user's data after signing in</span></span>

<span data-ttu-id="6cda3-161">Затем Расширьте приложение, чтобы отобразить данные из календаря пользователя.</span><span class="sxs-lookup"><span data-stu-id="6cda3-161">Next, extend the application to show data from the user's calendar.</span></span> <span data-ttu-id="6cda3-162">Доступ к этим сведениям можно получить только после того, как пользователь выполнил вход.</span><span class="sxs-lookup"><span data-stu-id="6cda3-162">You can access this information only after the user has signed in.</span></span> <span data-ttu-id="6cda3-163">Для этого необходимо отслеживать состояние входа пользователя и отображать данные календаря после того, как пользователь войдет с помощью учетной записи Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="6cda3-163">To do this, you will need to track the  user's sign in state and show the calendar data after the user has signed in with their Microsoft account.</span></span>

#### <a name="track-users-sign-in-state"></a><span data-ttu-id="6cda3-164">Отслеживание состояния входа пользователя</span><span class="sxs-lookup"><span data-stu-id="6cda3-164">Track user's sign in state</span></span>

<span data-ttu-id="6cda3-165">Чтобы отслеживать состояние входа пользователя в приложение, вы будете использовать отклики и обработчики `useState` `useEffect` в сочетании с обработчиками событий поставщика.</span><span class="sxs-lookup"><span data-stu-id="6cda3-165">To track the user's sign in state in your application, you will use the React `useState` and `useEffect` hooks in combination with provider event handlers.</span></span>

1. <span data-ttu-id="6cda3-166">В редакторе кода откройте файл **src/App. Целевой** файл и расширьте существующий оператор реагируя `import` .</span><span class="sxs-lookup"><span data-stu-id="6cda3-166">In the code editor, open the **src/App.tsx** file and extend the existing React `import` statement.</span></span>

    ```tsx
    import React, { useState, useEffect } from 'react';
    ```

1. <span data-ttu-id="6cda3-167">Импортируйте `Provider` `ProviderState` типы и типы из набора инструментов Microsoft Graph, добавив их в "Импорт".</span><span class="sxs-lookup"><span data-stu-id="6cda3-167">Import the `Provider` and `ProviderState` types from Microsoft Graph Toolkit, by adding to imports.</span></span>

    ```tsx
    import { Providers, ProviderState } from '@microsoft/mgt';
    ```

1. <span data-ttu-id="6cda3-168">Добавьте пользовательскую функцию с именем `useIsSignedIn` , позволяющую отслеживать состояние входа пользователя в приложении.</span><span class="sxs-lookup"><span data-stu-id="6cda3-168">Add a custom function named `useIsSignedIn` that enables tracking the user's sign in state in your application.</span></span>

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

<span data-ttu-id="6cda3-169">Эта функция выполняет две задачи.</span><span class="sxs-lookup"><span data-stu-id="6cda3-169">This function does two things.</span></span> <span data-ttu-id="6cda3-170">Во-первых, с помощью `useState` обработчика реагирующих включается состояние отслеживания в компоненте.</span><span class="sxs-lookup"><span data-stu-id="6cda3-170">First, using the React `useState` hook, it enables tracking state inside your component.</span></span> <span data-ttu-id="6cda3-171">При изменении состояния реагирует на то, что компонент будет повторно визуализирован.</span><span class="sxs-lookup"><span data-stu-id="6cda3-171">Whenever the state changes, React will re-render your component.</span></span> <span data-ttu-id="6cda3-172">Во-вторых, с помощью `useEffect` обработчика реагирования он расширяет жизненный цикл компонента, отслеживая изменения в поставщике набора средств Microsoft Graph и обновляя компонент при необходимости.</span><span class="sxs-lookup"><span data-stu-id="6cda3-172">Second, using the React `useEffect` hook, it extends the component's lifecycle by tracking changes in the Microsoft Graph Toolkit provider and updating the component if necessary.</span></span>

#### <a name="load-users-calendar-if-user-is-signed-in"></a><span data-ttu-id="6cda3-173">Загружать календарь пользователя, если пользователь вошел в систему</span><span class="sxs-lookup"><span data-stu-id="6cda3-173">Load user's calendar if user is signed in</span></span>

<span data-ttu-id="6cda3-174">Теперь, когда вы отслеживаете состояние входа пользователя в приложении, вы можете отобразить свой календарь после того, как они вошли в систему.</span><span class="sxs-lookup"><span data-stu-id="6cda3-174">Now that you track the user's sign in state in your application, you can show their calendar after they signed in.</span></span>

1. <span data-ttu-id="6cda3-175">В редакторе кода откройте файл **src/App. Целевой** файл, а затем в функции **app** добавьте:</span><span class="sxs-lookup"><span data-stu-id="6cda3-175">In the code editor, open the **src/App.tsx** file, and inside the **App** function, add:</span></span>

    ```tsx
    const [isSignedIn] = useIsSignedIn();
    ```

    <span data-ttu-id="6cda3-176">Этот параметр определяет логическую `isSignedIn` константу, которую можно использовать для определения того, вошел ли пользователь в систему в данный момент.</span><span class="sxs-lookup"><span data-stu-id="6cda3-176">This defines a Boolean `isSignedIn` constant, which you can use to determine whether the user is currently signed in to your application.</span></span>

1. <span data-ttu-id="6cda3-177">Расширьте содержимое `return` предложения с дополнительным `div` компонентом и компонентом повестки набора средств Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="6cda3-177">Extend the contents of the `return` clause with an additional `div` and the Microsoft Graph Toolkit Agenda component.</span></span>

    ```tsx
    <div>
      {isSignedIn &&
        <Agenda />}
    </div>
    ```

<span data-ttu-id="6cda3-178">В результате этих изменений файл **src/App. Целевой** должен выглядеть следующим образом:</span><span class="sxs-lookup"><span data-stu-id="6cda3-178">With these changes, the **src/App.tsx** file should look like the following.</span></span>

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

### <a name="test-showing-users-calendar-after-they-signed-in"></a><span data-ttu-id="6cda3-179">Тестирование отображения календаря пользователя после входа</span><span class="sxs-lookup"><span data-stu-id="6cda3-179">Test showing user's calendar after they signed in</span></span>

<span data-ttu-id="6cda3-180">После выполнения этих изменений после входа в приложение с помощью учетной записи Майкрософт вы должны увидеть свой календарь.</span><span class="sxs-lookup"><span data-stu-id="6cda3-180">With these changes, after signing in to your application with your Microsoft account, you should see your calendar.</span></span>

1. <span data-ttu-id="6cda3-181">Чтобы просмотреть изменения, закройте браузер и откройте его еще раз и перейдите по адресу `https://localhost:3000` .</span><span class="sxs-lookup"><span data-stu-id="6cda3-181">To see the changes, close the browser and open it again, and go to `https://localhost:3000`.</span></span> <span data-ttu-id="6cda3-182">Это делается потому, что вы изменили значение `scopes` свойства, которое влияет на маркер доступа, который вы запрашиваете из Azure AD.</span><span class="sxs-lookup"><span data-stu-id="6cda3-182">You do this because you changed the value of the `scopes` property, which affects the access token that you request from Azure AD.</span></span>
1. <span data-ttu-id="6cda3-183">Нажмите кнопку **входа** и войдите с помощью своей учетной записи Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="6cda3-183">Choose the **Sign In** button and sign in using your Microsoft account.</span></span> <span data-ttu-id="6cda3-184">Обратите внимание на добавления в список разрешений, запрашиваемых в запросе согласия.</span><span class="sxs-lookup"><span data-stu-id="6cda3-184">Notice the additions to the list of permissions requested in the consent prompt.</span></span> <span data-ttu-id="6cda3-185">Это связано с тем, что в свойстве включены дополнительные разрешения `scope` .</span><span class="sxs-lookup"><span data-stu-id="6cda3-185">This is because you included additional permissions in the `scope` property.</span></span>
1. <span data-ttu-id="6cda3-186">После того как вы отправили использование приложения, вам будут видны сведения о текущем пользователе и их календаре.</span><span class="sxs-lookup"><span data-stu-id="6cda3-186">After consenting to the use of the application, you should see information about the current user and their calendar.</span></span>

![Законченное приложение](../images/mgt-finished-app.png)

## <a name="next-steps"></a><span data-ttu-id="6cda3-188">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="6cda3-188">Next steps</span></span>

- <span data-ttu-id="6cda3-189">Узнайте [, что находится в наборе средств Microsoft Graph](../overview.md).</span><span class="sxs-lookup"><span data-stu-id="6cda3-189">See [what's in the Microsoft Graph Toolkit](../overview.md).</span></span>
- <span data-ttu-id="6cda3-190">Опробуйте компоненты в [интерактивная среда](https://mgt.dev).</span><span class="sxs-lookup"><span data-stu-id="6cda3-190">Try out the components in the [playground](https://mgt.dev).</span></span>
- <span data-ttu-id="6cda3-191">Задайте вопрос о [переполнении стека](https://aka.ms/mgt-question).</span><span class="sxs-lookup"><span data-stu-id="6cda3-191">Ask a question on [Stack Overflow](https://aka.ms/mgt-question).</span></span>
- <span data-ttu-id="6cda3-192">Сообщать об ошибках или оставлять запрос на функцию в [GitHub](https://aka.ms/mgt).</span><span class="sxs-lookup"><span data-stu-id="6cda3-192">Report bugs or leave a feature request on [GitHub](https://aka.ms/mgt).</span></span>
