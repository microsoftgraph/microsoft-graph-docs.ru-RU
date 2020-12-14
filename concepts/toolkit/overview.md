---
title: 'Microsoft Graph набор средств: компоненты пользовательского интерфейса и поставщики проверки подлинности для Microsoft Graph'
description: Microsoft Graph набор средств — это коллекция поставщиков проверки подлинности и веб-компонентов, которые могут повторно работать, не зависит от структуры, для доступа к Microsoft Graph и работы с ним.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: d2ed14c5862cbd081b7592a180cd15e2bfdb2548
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2020
ms.locfileid: "49659277"
---
# <a name="microsoft-graph-toolkit-ui-components-and-authentication-providers-for-microsoft-graph"></a>Microsoft Graph набор средств: компоненты пользовательского интерфейса и поставщики проверки подлинности для Microsoft Graph 

Microsoft Graph набор средств — это коллекция повторно работающих, не зависит от структуры компонентов и поставщиков проверки подлинности для доступа к Microsoft Graph и работы с ним. Компоненты полностью готовы к функциональности со встроенными поставщиками, которые аутентификация и извлечение данных из Microsoft Graph.

Microsoft Graph набор средств упрощает использование Microsoft Graph в приложении. В следующем примере во время входа пользователя и его событий календаря отображаются только [](./components/agenda.md) две строки кода с помощью компонентов [входа](./components/login.md) и повестки дня.

<iframe src="https://mgt.dev/iframe.html?id=samples-general--login-to-show-agenda&source=docs&source=docs" height="400"></iframe>

[Откройте этот пример в mgt.dev](https://mgt.dev/?path=/story/samples-general--login-to-show-agenda&source=docs)

## <a name="whats-in-the-microsoft-graph-toolkit"></a>Что в microsoft Graph набор средств?

### <a name="components"></a>Компоненты

Microsoft Graph набор средств содержит коллекцию веб-компонентов для наиболее распространенных встроенных API Microsoft Graph. 

Эти компоненты также доступны в качестве [компонентов React.](./get-started/mgt-react.md)

|Компонент|Описание|
|---------|-----------|
|[Вход](./components/login.md)|Кнопка и flyout для проверки подлинности пользователя с помощью платформы удостоверений Майкрософт и отображения сведений профиля пользователя при входе.|
|[Пользователь](./components/person.md)|Отображает человека или контакт по его фотографии, имени и/или адресу электронной почты.|
|[Люди](./components/people.md)|Отображает группу людей или контактов по их фотографиям или инициалам.|
|[Повестка](./components/agenda.md)|Отображает события в календаре пользователя или группы.|
|[Задачи](./components/tasks.md)|Отображает и позволяет добавлять, удалять, завершать или редактировать задачи из Планировщика (Майкрософт) или Microsoft To Do (Майкрософт).|
|[Выбор людей](./components/people-picker.md)|Предоставляет возможность поиска людей и отображения списка результатов.|
|[Карточка человека](./components/person-card.md)|Flyout used on the person component to display more profile information about a user.|
|[получение](./components/get.md);|Сделайте запрос GET к любому API Microsoft Graph непосредственно в HTML-коде.|
|[Выбор канала](./components/teams-channel-picker.md)|Предоставляет возможность поиска каналов Microsoft Teams для выбора канала из отрисовки списка результатов.|
|[To Do](./components/todo.md)|Отображает и позволяет добавлять, удалять, завершать или редактировать задачи из Microsoft To Do.|

### <a name="providers"></a>Поставщики

[Поставщики](/providers/providers.md) обеспечивают проверку подлинности и обеспечивают реализацию для получения маркеров доступа на различных платформах и предоставления клиента Microsoft Graph для вызова API Microsoft Graph. Компоненты лучше всего работают при работе с поставщиком, но их можно использовать самостоятельно.

|Поставщики|Описание|
|---------|-----------|
|[Msal](./providers/msal.md)|Использует MSAL.js для входов пользователей и получения маркеров для использования с Microsoft Graph.|
|[SharePoint](./providers/sharepoint.md)|Проверка подлинности и предоставляет Microsoft Graph доступ к компонентам в веб-частях SharePoint.|
|[Teams](./providers/teams.md)|Проверка подлинности и предоставляет Microsoft Graph доступ к компонентам на вкладке Microsoft Teams.|
|[Прокси-сервер](./providers/proxy.md)|Позволяет использовать проверку подлинности на тыловом компьютере путем маршрутизации всех вызовов в Microsoft Graph через ваш тыл.|
|[Custom](./providers/custom.md)|Создайте настраиваемого поставщика, чтобы включить проверку подлинности и доступ к Microsoft Graph с помощью существующего кода проверки подлинности приложения.|

## <a name="why-use-the-microsoft-graph-toolkit"></a>Зачем использовать microsoft Graph набор средств?

Microsoft Graph набор средств позволяет быстро и просто интегрировать распространенные опытом, встроенные в Microsoft Graph, в собственное приложение.

:::row:::
   :::column span="":::
    **Сокращение времени разработки**

    Работа по подключению к API Microsoft Graph и отрисовка данных в пользовательском интерфейсе, который выглядит как Microsoft365, сделана для вас без необходимости настройки.
  :::column-end:::
  :::column span="":::
    **Работает везде**

    Все компоненты основаны на веб-стандартах и легко работают с любым современным браузером и веб-структурой (React, Angular, Vue и т. д.). 
  :::column-end:::
  :::column span="":::
    **Красивый, но гибкий**

    Эти компоненты предназначены для работы с Microsoft 365, но также настраиваются с помощью настраиваемых свойств [CSS](./customize-components/style.md) и [шаблонов.](./customize-components/templates.md)
  :::column-end:::
:::row-end:::

## <a name="who-should-use-it"></a>Кто должен использовать его?

Microsoft Graph набор средств отлично подходит для разработчиков всех уровней работы, которые ищут разработку веб-приложения, вкладки Microsoft Teams или веб-части SharePoint, которая подключается к данным из Microsoft Graph и имеет к ним доступ.

## <a name="where-can-i-use-it"></a>Где его можно использовать?

Microsoft Graph набор средств в следующих браузерах.

|![Microsoft Edge](images/edgeIcon.png)|![Firefox](images/firefoxIcon.png)|![Chrome](images/chromeIcon.png)|![Safari](images/safariIcon.png)|![Opera](images/operaIcon.png)|![Интернет-подключение к Интернету](images/samsungInternetIcon.png)|
|----|----|----|----|----|----|----|
|**Microsoft Edge**|**Firefox**|**Chrome**|**Safari**|**Opera**|**Сума**|

## <a name="next-steps"></a>Дальнейшие действия

- Попробуйте компоненты в игровой [области.](https://mgt.dev)
- [Начало работы](./get-started/overview.md) с microsoft Graph набор средств.
- Ознакомьтесь с набор средств Microsoft Graph на [сайте GitHub.](https://aka.ms/mgt)
