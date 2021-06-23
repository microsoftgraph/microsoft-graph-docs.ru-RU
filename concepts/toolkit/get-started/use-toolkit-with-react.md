---
title: Использование Microsoft Graph Toolkit с React
description: Начало использования Microsoft Graph Toolkit в приложении React
localization_priority: Normal
author: waldekmastykarz
ms.openlocfilehash: 6618599b767f5c7ebe3d0469aed012c81125738e
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060497"
---
# <a name="use-the-microsoft-graph-toolkit-with-react"></a>Использование Microsoft Graph Toolkit с React

Microsoft Graph Toolkit — это набор веб-компонентов, которые упрощают подключение к Microsoft Graph и позволяют вам сосредоточиться на своем приложении. Microsoft Graph Toolkit доступен как общий набор веб-компонентов, распространяемых через пакет NPM `@microsoft/mgt`.

Если вы создаете приложения с помощью React, вы можете использовать [пакет `@microsoft/mgt-react`](./mgt-react.md), который упаковывает веб-компоненты Microsoft Graph Toolkit в компоненты React и упрощает передачу сложных данных.

В этой статье описывается пошаговый процесс использования Microsoft Graph Toolkit для создания приложения React и подключения его к Microsoft 365. После выполнения всех шагов у вас получится приложение React, которое показывает предстоящие встречи пользователя, вошедшего в систему в Microsoft 365.

> [!TIP]
> Вы также можете следовать этому учебнику в качестве интерактивного тура кода. Подробные сведения см. [в GitHub репо в стартовом проекте.](https://github.com/microsoftgraph/mgt-react-codetour)

## <a name="prerequisites"></a>Предварительные условия

Чтобы выполнить действия, описанные в этой статье, вам понадобится среда разработки Microsoft 365 и несколько инструментов. Дополнительные сведения см. в разделе [Приступая к работе](./overview.md).

## <a name="create-a-react-app"></a>Создание приложения React

Создайте приложение React, выполнив следующую команду. Это создаст новое приложение React с использованием TypeScript, что поможет написать более функциональный код и избежать ошибок выполнения.

```Command Line
npx create-react-app my-m365-app --template typescript --use-npm
```

Измените рабочий каталог на только что созданное приложение.

```Command Line
cd my-m365-app
```

Затем установите пакет NPM `mgt-react`, который содержит компоненты Microsoft Graph Toolkit для React.

```Command Line
npm i @microsoft/mgt-react
```

Установите и пакет npm, который содержит `mgt-msal2-provider` `mgt-element` поставщика auth MSAL 2.0.

```Command Line
npm i @microsoft/mgt-element @microsoft/mgt-msal2-provider
```

Подтвердите, что вы можете запустить приложение.

```Command Line
npm start
```

У вас должна быть возможность открыть приложение в браузере через `http://localhost:3000`.

[!INCLUDE [AAD with implicit flow app registration](../includes/aad-app-registration-spa.md)]

## <a name="connect-react-app-to-microsoft-365"></a>Подключение приложения React к Microsoft 365

Теперь, когда вы зарегистрировали свое приложение в Azure Active Directory (Azure AD), вы можете подключить приложение React к Microsoft 365. Для начала разрешите пользователям входить в приложение при помощи учетной записи Майкрософт.

### <a name="copy-the-azure-ad-application-registration-id"></a>Скопируйте идентификатор регистрации приложения в Azure AD.

1. На портале Azure перейдите к регистрации приложения.
1. Убедитесь, что вы находитесь на странице **Обзор**.
1. Скопируйте значение свойства **Идентификатор приложения (клиента)** из раздела **Основное**. 

### <a name="configure-the-microsoft-graph-toolkit-authentication-provider"></a>Настройка поставщика проверки подлинности Microsoft Graph Toolkit

Теперь настройте поставщика проверки подлинности, который должен использовать Microsoft Graph Toolkit. В этом случае будет использоваться MSAL, который по умолчанию подходит для создания автономных приложений. Если вы используете какие-либо точки расширения в Microsoft 365, например Teams или SharePoint, то необходимо будет выбрать [других поставщиков](../providers/providers.md).

>[!NOTE] 
>Если вы в настоящее время используете поставщика MSAL и хотите обновить поставщика MSAL 2, выполните действия в статье [поставщика MSAL 2.](../providers/msal2.md#migrating-from-msal-provider-to-msal-2-provider)

1. Откройте в редакторе кода файл **src/index.** и добавьте в список операций импорта следующее:

    ```TypeScript
    import { Providers } from '@microsoft/mgt-element';
    import { Msal2Provider } from '@microsoft/mgt-msal2-provider';
    ```

1. После последнего оператора `import` инициализируйте Microsoft Graph Toolkit с помощью поставщика MSAL.

    ```TypeScript
    Providers.globalProvider = new Msal2Provider({
      clientId: 'REPLACE_WITH_CLIENTID'
    });
    ```

    Замените значение свойства `clientId` значением свойства `Application (client) ID`, которое вы ранее скопировали на портале Azure.

С этими изменениями файл **src/index.tsx** будет выглядеть следующим образом.

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

### <a name="add-the-sign-in-button"></a>Добавление кнопки входа

Добавьте компонент Microsoft Graph Toolkit для React под названием **Вход**, отображающий кнопку **Войти**, которую пользователи смогут использовать для входа в ваше приложение со своей учетной записью Майкрософт.

1. Откройте в редакторе кода файл **src/App.tsx** и добавьте в список операций импорта следующее:

    ```TypeScript
    import { Login } from '@microsoft/mgt-react';
    ```

1. В функции `App` замените содержимое пункта `return` базовой структурой, включая компонент входа Microsoft Graph Toolkit:

    ```TypeScript
    <div className="App">
      <header>
        <Login />
      </header>
    </div>
    ```

С этими изменениями файл **src/App.tsx** будет выглядеть следующим образом.
```TypeScript

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

### <a name="test-signing-in-to-your-application"></a>Тестирование входа в приложение

Теперь вы можете входить в приложение с помощью своей учетной записи Майкрософт.

1. Вернитесь в браузер, в котором выполняется ваше приложение React. Теперь вы должны видеть кнопку **Войти**.
1. При нажатии кнопки **Войти** вам будет предложено войти в систему с помощью учетной записи Майкрософт. Вы можете использовать ту же учетную запись, с помощью которой заходили на портал Azure.
1. Так как это приложение Azure AD используется впервые, вам необходимо дать согласие на его использование в вашей организации.
1. После входа в систему вы будете перенаправлены в приложение React. Обратите внимание, что кнопка **Войти** изменилась и теперь показывает ваше имя пользователя ![Приложение React отображает информацию о пользователе, полученную из Microsoft 365 с помощью Microsoft Graph Toolkit](../images/mgt-react-userinfo.png).

## <a name="load-data-from-microsoft-365"></a>Загрузка данных из Microsoft 365

Microsoft Graph Toolkit не только упрощает проверку подлинности при входе в Microsoft 365, но и загружает его данные. В этом примере будет показан календарь пользователя, вошедшего в систему.

### <a name="specify-permissions-needed-for-your-application"></a>Определение разрешений, необходимых для вашего приложения

Прежде чем вы сможете загружать данные из Microsoft 365, необходимо определить список областей разрешений, которые необходимы вашему приложению для получения доступа к данным пользователя. Эти области различаются в зависимости от того, какую информацию вы хотите показать. В этом случае понадобится доступ к календарю пользователей, а также базовый доступ к информации о пользователях, которая также отображается в календаре. Области разрешений, необходимые для каждого API, можно найти в [документации API Microsoft Graph](/graph/api/overview).

1. Откройте в редакторе кода файл **src/index.tsx** и обновите код инициализации поставщика.

    ```TypeScript
    Providers.globalProvider = new Msal2Provider({
      clientId: 'REPLACE_WITH_CLIENTID',
      scopes: ['calendars.read', 'user.read', 'openid', 'profile', 'people.read', 'user.readbasic.all']
    });
    ```

### <a name="show-users-data-after-signing-in"></a>Отображение данных пользователя после входа в систему

Теперь дополните приложение, чтобы оно отображало данные из календаря пользователя. Доступ к этой информации можно получить только после того, как пользователь вошел в систему. Для этого необходимо отслеживать, находится ли пользователь в системе, и отображать данные календаря только после того, как пользователь вошел в систему с помощью своей учетной записи Майкрософт.

#### <a name="track-users-sign-in-state"></a>Отслеживание состояния входа пользователя в систему

Для отслеживания состояния входа пользователя в приложение будет использоваться обработчики React `useState` и `useEffect` в сочетании с обработчиками событий провайдера.

1. Откройте в редакторе кода файл **src/App.tsx** и дополните существующий оператор React `import`.

    ```TypeScript
    import React, { useState, useEffect } from 'react';
    ```

1. Импортируйте типы `Provider` и `ProviderState` из `mgt-element`, добавив их в операции импорта.

    ```TypeScript
    import { Providers, ProviderState } from '@microsoft/mgt-element';
    ```

1. Добавьте настраиваемую функцию с именем `useIsSignedIn`, которая позволяет отслеживать состояние входа пользователя в приложение.

    ```TypeScript
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

Эта функция выполняет два действия. Во-первых, с помощью обработчика React `useState` она позволяет отслеживать состояние внутри компонента. При каждом изменении состояния React повторно отображает ваш компонент. Во-вторых, с помощью обработчика React `useEffect` она продлевает жизненный цикл компонента, отслеживая изменения в поставщике Microsoft Graph Toolkit и обновляя компонент при необходимости.

#### <a name="load-users-calendar-if-user-is-signed-in"></a>Загрузка календаря пользователя, вошедшего в систему

Теперь, когда отслеживается состояние входа пользователя в приложение, вы можете отображать календарь пользователя после входа в систему.

1. В редакторе кода откройте **файл src/App.tsx** и раздвяйте заявление компонента `import` с **компонентом Agenda.**

    ```TypeScript
    import { Agenda, Login } from '@microsoft/mgt-react';
    ```

1. Далее в **функции App** добавьте:

    ```TypeScript
    const [isSignedIn] = useIsSignedIn();
    ```

    Это определяет логическую константу `isSignedIn`, которую можно использовать для определения, выполнил ли пользователь вход в приложение.

1. В содержимое пункта `return` добавьте `div`, а также компонент расписания Microsoft Graph Toolkit.

    ```TypeScript
    <div>
      {isSignedIn &&
        <Agenda />}
    </div>
    ```

С этими изменениями файл **src/App.tsx** будет выглядеть следующим образом.

```TypeScript
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

### <a name="test-showing-users-calendar-after-they-signed-in"></a>Тестирование отображения календаря пользователя после входа в систему

С внесением этих изменений вы должны увидеть свой календарь после входа в приложение с учетной записью Майкрософт.

1. Чтобы увидеть изменения, закройте браузер, откройте его снова и перейдите на `http://localhost:3000`. Это нужно сделать, потому что вы изменили значение свойства `scopes`, которое влияет на маркер доступа, запрашиваемый из Azure AD.
1. Нажмите кнопку **Войти** и войдите с помощью учетной записи Майкрософт. Обратите внимание на новые пункты списка разрешений в запросе на продолжение. Они появились, так как вы включили в свойство `scope` дополнительные разрешения.
1. После подтверждения согласия на использование приложения вы должны увидеть информацию о текущем пользователе и его календаре.

![Готовое приложение](../images/mgt-finished-app.png)

## <a name="next-steps"></a>Дальнейшие действия

- Узнать, [что включает Microsoft Graph Toolkit](../overview.md).
- Воспользуйтесь компонентами в [интерактивной среде](https://mgt.dev).
- Задавайте вопросы на сайте [Stack Overflow](https://aka.ms/mgt-question).
- Сообщайте об ошибках и оставляйте запросы на создание функций в [GitHub](https://aka.ms/mgt).
