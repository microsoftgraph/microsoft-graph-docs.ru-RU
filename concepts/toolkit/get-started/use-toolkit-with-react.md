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
# <a name="use-the-microsoft-graph-toolkit-with-react"></a>Использование microsoft Graph набор средств React

Microsoft Graph набор средств это набор веб-компонентов, упрощающих подключение к Microsoft Graph и позволяющих сосредоточиться на приложении. Microsoft Graph набор средств как универсальный набор веб-компонентов, распространяемых через `@microsoft/mgt` пакет npm.

Если вы создаете приложения с помощью React, вы можете использовать [ `@microsoft/mgt-react` пакет,](./mgt-react.md)который упаковывает веб-компоненты Microsoft Graph набор средств в компоненты React и упрощает передачу сложных данных.

В этой статье описывается пошаговой процесс использования microsoft Graph набор средств для создания приложения React и его подключения к Microsoft 365. После выполнения этих действий у вас будет приложение React, которое отображает предстоящие встречи войдя в microsoft 365.

## <a name="prerequisites"></a>Предварительные условия

Чтобы следовать шагам из этой статьи, вам потребуется среда разработки Microsoft 365 и несколько средств. Подробные сведения [см. в сведениях о том, как начать работу.](./overview.md)

## <a name="create-a-react-app"></a>Создание приложения React

Создайте новое приложение React, выдав следующую команду. Это позволит создать новое приложение React с помощью TypeScript, которое поможет вам написать более надежный код и избежать ошибок во время работы.

```cmd
npx create-react-app my-m365-app --template typescript
```

Измените рабочий каталог на только что созданное приложение.

```cmd
cd my-m365-app
```

Затем установите пакет npm, содержащий компоненты `mgt-react` Microsoft Graph набор средств React.

```cmd
npm i @microsoft/mgt-react
```

Установите также пакет npm, который содержит поставщика `mgt-msal-provider` `mgt-element` auth MSAL.

```cmd
npm i @microsoft/mgt-element @microsoft/mgt-msal-provider
```

Подтвердите, что вы можете запустить приложение.

```cmd
npm start
```

Вы должны иметь возможность открыть приложение в браузере с помощью `http://localhost:3000` .

[!INCLUDE [AAD with implicit flow app registration](../includes/aad-app-registration-spa.md)]

## <a name="connect-react-app-to-microsoft-365"></a>Подключение приложения React к Microsoft 365

После регистрации приложения в Azure Active Directory (Azure AD) вы можете подключить приложение React к Microsoft 365. Во-первых, разрешим пользователям войти в приложение с помощью своей учетной записи Майкрософт.

### <a name="copy-the-azure-ad-application-registration-id"></a>Копирование ИД регистрации приложения Azure AD

1. На портале Azure перейдите к регистрации приложения.
1. Убедитесь, что вы находитесь на странице **"Обзор".**
1. В разделе **"Essentials"** скопируйте значение свойства **Application (client) ID**

### <a name="configure-the-microsoft-graph-toolkit-authentication-provider"></a>Настройка поставщика проверки подлинности набор средств Microsoft Graph

Затем настройте поставщика проверки подлинности, который должен набор средств Microsoft Graph. В этом случае вы будете использовать MSAL, что является хорошим значением по умолчанию для создания автономных приложений. Если вы используете любую из точек возможностей в Microsoft 365, например Teams или SharePoint, вы будете использовать [других поставщиков.](../providers/providers.md)

1. В редакторе кода откройте **src/index.** и в список импортов добавьте:

    ```tsx
    import { Providers } from '@microsoft/mgt-element';
    import { MsalProvider } from '@microsoft/mgt-msal-provider';
    ```

1. После последнего `import` оператора инициализировать microsoft Graph набор средств с помощью поставщика MSAL.

    ```tsx
    Providers.globalProvider = new MsalProvider({
      clientId: 'REPLACE_WITH_CLIENTID'
    });
    ```

    Замените значение свойства на значение свойства, скопированные ранее `clientId` `Application (client) ID` на портале Azure.

При этих изменениях **файл src/index.tsx** будет выглядеть следующим образом.

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

### <a name="add-the-sign-in-button"></a>Добавление кнопки "Вход"

Добавьте компонент **Microsoft** Graph для входа набор средств React,  который отобразит кнопку входа, которую можно использовать для входа с помощью учетной записи Майкрософт в ваше приложение.

1. В редакторе кода откройте **файл src/App.tsx** и добавьте в список импорта:

    ```tsx
    import { Login } from '@microsoft/mgt-react';
    ```

1. В функции замените содержимое предложения базовой структурой, включая компонент `App` `return` Microsoft Graph набор средств входа:

    ```tsx
    <div className="App">
      <header>
        <Login />
      </header>
    </div>
    ```

После этих изменений **файл src/App.tsx** будет выглядеть следующим образом.
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

### <a name="test-signing-in-to-your-application"></a>Проверка вход в приложение

Теперь у вас должна быть возможность войти в приложение с помощью учетной записи Майкрософт.

1. Перейдите в браузер, в котором запущено приложение React. Теперь вы увидите кнопку **"Вход".**
1. При нажатии кнопки "Вход" вам будет предложено войти с помощью учетной записи Майкрософт (вы можете использовать ту же учетную запись, что и учетную запись, с помощью учетной записи, с помощью которая была у вас на портале Azure). 
1. Так как это первый раз, когда вы используете это приложение Azure AD, необходимо согласиться на его использование в вашей организации.
1. После этого вы будете перенаправлены в приложение React. Обратите внимание, что кнопка **"Вход"** изменена для показа имени пользователя в приложении React, в котором отображаются сведения о пользователе, полученные из Microsoft 365 с помощью ![ Microsoft Graph ](../images/mgt-react-userinfo.png) набор средств.

## <a name="load-data-from-microsoft-365"></a>Загрузка данных из Microsoft 365

Microsoft Graph набор средств не только упрощает проверку подлинности в Microsoft 365, но и загружает ее данные. В этом примере вы увидите календарь во время подписания.

### <a name="specify-permissions-needed-for-your-application"></a>Указание разрешений, необходимых для приложения

Перед загрузкой данных из Microsoft 365 необходимо указать список областей разрешений, которые должно предоставить приложение для доступа к данным пользователя. Эти области различаются в зависимости от типа информации, которую необходимо отдемонстрировать. В этом случае вам потребуется доступ к календарю людей, а также базовый доступ к сведениям о людей, которые также отображаются в календаре. Области, необходимые для каждого API, можно найти в документации [по API Microsoft Graph.](/graph/api/overview)

1. В редакторе кода откройте **файл src/index.tsx** и обновим код инициализации поставщика.

    ```tsx
    Providers.globalProvider = new MsalProvider({
      clientId: 'd7cb93c9-9097-4e38-8f06-7c0088ac3318',
      scopes: ['calendars.read', 'user.read', 'openid', 'profile', 'people.read', 'user.readbasic.all']
    });
    ```

### <a name="show-users-data-after-signing-in"></a>Показывать данные пользователя после входов

Затем расширим приложение, чтобы показать данные из календаря пользователя. Вы можете получить доступ к этой информации только после того, как пользователь войт. Для этого необходимо отслеживать состояние пользователя при входе и показывать данные календаря после того, как пользователь войт в свою учетную запись Майкрософт.

#### <a name="track-users-sign-in-state"></a>Отслеживание состояния пользователя при входе

Чтобы отслеживать состояние пользователя при входе в приложение, вы будете использовать React и обработчики в сочетании с обработчиками `useState` `useEffect` событий поставщика.

1. В редакторе кода откройте **файл src/App.tsx** и расширйте существующий `import` выписку React.

    ```tsx
    import React, { useState, useEffect } from 'react';
    ```

1. Импортировать `Provider` типы и типы из , добавив в `ProviderState` `mgt-element` импорт.

    ```tsx
    import { Providers, ProviderState } from '@microsoft/mgt-element';
    ```

1. Добавьте пользовательскую функцию с именем, которая позволяет отслеживать состояние пользователя при входе `useIsSignedIn` в приложение.

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

Эта функция делает две вещи. Во-первых, с помощью `useState` обцепки React он включает отслеживание состояния в компоненте. При смене состояния React будет повторно отрисовки компонента. Во-вторых, с помощью обработца React он расширяет жизненный цикл компонента, отслеживая изменения в поставщике набор средств Microsoft Graph и при необходимости обновляя `useEffect` компонент.

#### <a name="load-users-calendar-if-user-is-signed-in"></a>Загрузка календаря пользователя, если пользователь в него вписались

Теперь, когда вы отслеживаете состояние пользователя в приложении, вы можете отследить его календарь после того, как он войт.

1. В редакторе кода откройте **файл src/App.tsx** и добавьте в функцию **App:**

    ```tsx
    const [isSignedIn] = useIsSignedIn();
    ```

    Таким образом определяется boolean constant, с помощью которой можно определить, в данный момент ли пользователь вписан `isSignedIn` в приложение.

1. Расширим содержимое предложения с помощью дополнительного компонента и компонента `return` `div` Microsoft Graph набор средств Agenda.

    ```tsx
    <div>
      {isSignedIn &&
        <Agenda />}
    </div>
    ```

При этих изменениях **файл src/App.tsx** должен выглядеть следующим образом.

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

### <a name="test-showing-users-calendar-after-they-signed-in"></a>Тестирование с отображением календаря пользователя после его войки

После внесения этих изменений в приложение с помощью учетной записи Майкрософт вы должны увидеть свой календарь.

1. Чтобы увидеть изменения, закроем браузер и снова откройте его и перейдите к `http://localhost:3000` . Это необходимо, так как вы изменили значение свойства, что влияет на маркер `scopes` доступа, запрашиваемого из Azure AD.
1. Choose the **Sign In** button and sign in using your Microsoft account. Обратите внимание на дополнения к списку разрешений, запрашиваемого в запросе согласия. Это необходимо из-за того, что вы включили дополнительные разрешения в `scope` свойство.
1. После согласия на использование приложения вы должны увидеть сведения о текущем пользователе и его календаре.

![Готовое приложение](../images/mgt-finished-app.png)

## <a name="next-steps"></a>Дальнейшие действия

- Посмотрите, [что в Microsoft Graph набор средств.](../overview.md)
- Попробуйте компоненты в игровой [области.](https://mgt.dev)
- Задайте вопрос на [сайте Stack Overflow.](https://aka.ms/mgt-question)
- Сообщать об ошибках или оставлять запрос на функции на [GitHub.](https://aka.ms/mgt)
