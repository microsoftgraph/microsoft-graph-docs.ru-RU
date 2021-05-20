---
title: 'Microsoft Graph Toolkit: компоненты пользовательского интерфейса и поставщики проверки подлинности для Microsoft Graph'
description: Microsoft Graph Toolkit — это коллекция поставщиков проверки подлинности и многократно используемых, не зависящих от платформы веб-компонентов для доступа и работы в Microsoft Graph.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: e39eba8c79d2aae3d1ce048a21d2d0a911aed089
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579769"
---
# <a name="microsoft-graph-toolkit-ui-components-and-authentication-providers-for-microsoft-graph"></a>Microsoft Graph Toolkit: компоненты пользовательского интерфейса и поставщики проверки подлинности для Microsoft Graph 

Microsoft Graph Toolkit — это коллекция многократно используемых, не зависящих от платформы компонентов и поставщиков проверки подлинности для доступа и работы в Microsoft Graph. Готовые компоненты являются полностью функциональными и включают встроенных поставщиков, которые проверяют подлинность и получают данные из Microsoft Graph.

С помощью Microsoft Graph Toolkit можно легко использовать Microsoft Graph в своем приложении. В следующем примере вошедший пользователь и события его календаря отображаются всего лишь в двух строках кода с помощью компонентов [Вход](./components/login.md) и [Повестка дня](./components/agenda.md).

<iframe src="https://mgt.dev/iframe.html?id=samples-general--login-to-show-agenda&source=docs&source=docs" height="400"></iframe>

[Открыть этот пример в mgt.dev](https://mgt.dev/?path=/story/samples-general--login-to-show-agenda&source=docs)

## <a name="whats-in-the-microsoft-graph-toolkit"></a>Что включает Microsoft Graph Toolkit?

### <a name="components"></a>Компоненты

Microsoft Graph Toolkit включает коллекцию веб-компонентов для наиболее распространенных встроенных возможностей на базе API Microsoft Graph. 

Они также доступны как [компоненты React](./get-started/mgt-react.md).

|Компонент|Описание|
|---------|-----------|
|[Вход](./components/login.md)|Кнопка и элемент управления "Всплывающий элемент" для проверки подлинности пользователя с помощью платформы удостоверений Майкрософт и отображения сведений из профиля пользователя при входе.|
|[Человек](./components/person.md)|Отображает пользователя или контакт с помощью его фотографии, имени и/или адреса электронной почты.|
|[Люди](./components/people.md)|Отображает группу людей или контактов с помощью их фотографий или инициалов.|
|[Повестка дня](./components/agenda.md)|Отображает события в календаре пользователя или группы.|
|[Задачи](./components/tasks.md)|Отображает и включает добавление, удаление, выполнение или редактирование задач из Планировщика (Майкрософт) или Microsoft To Do.|
|[Выбор людей](./components/people-picker.md)|Предоставляет возможность поиска людей и отображает список результатов.|
|[Карточка контакта](./components/person-card.md)|Всплывающий элемент, который используется в компоненте "Человек", чтобы отобразить больше сведений профиля о пользователе.|
|[Get](./components/get.md)|Создание GET-запроса к API Microsoft Graph прямо в HTML.|
|[Средство выбора каналов](./components/teams-channel-picker.md)|Предоставляет возможность поиска каналов Microsoft Teams и выбора канала из отображенного списка результатов.|
|[To Do](./components/todo.md)|Отображает и включает добавление, удаление, выполнение или редактирование задач из Microsoft To Do.|

### <a name="providers"></a>Поставщики

[Поставщики](/providers/providers.md) включают проверку подлинности, предоставляют реализацию для приобретения маркеров доступа на разных платформах и используют клиент Microsoft Graph для вызова API Microsoft Graph. Компоненты работают наилучшим образом, если используются с поставщиком, однако поставщики могут использоваться самостоятельно.

|Поставщики|Описание|
|---------|-----------|
|[MSAL](./providers/msal.md)|Использует MSAL.js для входа в систему и получения маркеров, которые применяются с Microsoft Graph.|
|[Msal 2.0](./providers/msal2.md)| Использует msal-браузер для регистрации пользователей и приобретения маркеров для использования в Microsoft Graph.|
|[Электрон](./providers/electron.md)|Проверка подлинности и Graph доступа к компонентам в приложениях Electron|
|[SharePoint](./providers/sharepoint.md)|Проверяет подлинность и предоставляет Microsoft Graph доступ к компонентам в веб-частях SharePoint.|
|[Teams](./providers/teams.md)|Проверяет подлинность и предоставляет Microsoft Graph доступ к компонентам во вкладках Microsoft Teams.|
|[Прокси-сервер](./providers/proxy.md)|Позволяет использовать проверку подлинности на внутреннем сервере с помощью маршрутизации всех вызовов Microsoft Graph через внутренний сервер.|
|[Настраиваемый](./providers/custom.md)|Создание настраиваемого поставщика для включения проверки подлинности и доступа к Microsoft Graph с помощью существующего кода проверки подлинности приложения.|

## <a name="why-use-the-microsoft-graph-toolkit"></a>Зачем использовать Microsoft Graph Toolkit?

Microsoft Graph Toolkit позволяет быстро и легко интегрировать общие возможности на платформе Microsoft Graph в собственное приложение.

:::row:::
   :::column span="":::
    **Сокращает срок разработки**

    Работа по подключению API Microsoft Graph и отображению данных в пользовательском интерфейсе, который выглядит и работает как возможность Microsoft365, выполняется за вас, без обязательной настройки.
  :::column-end:::
  :::column span="":::
    **Работает везде**

    Все компоненты соответствуют веб-стандартам и работают без проблем с любым современным браузером и веб-платформой (React, Angular, Vue и т. д.). 
  :::column-end:::
  :::column span="":::
    **Красивый, но гибкий**

    Компоненты выглядят и работают как возможности Microsoft365, но также могут быть настроены с помощью [настраиваемых свойств CSS](./customize-components/style.md) и [шаблонов](./customize-components/templates.md).
  :::column-end:::
:::row-end:::

## <a name="who-should-use-it"></a>Кто должен его использовать?

Microsoft Graph набор средств отлично подходит для разработчиков всех уровней опыта, которые ищут возможность разработки приложения, которое подключается к данным microsoft Graph, например:
- Веб-приложение
- Microsoft Teams вкладка
- Прогрессивное веб-приложение (PWA)
- Электронное приложение
- SharePoint веб-части

## <a name="where-can-i-use-it"></a>Где его можно использовать?

Microsoft Graph Toolkit поддерживается в следующих браузерах.

|![Microsoft Edge](images/edgeIcon.png)|![Firefox](images/firefoxIcon.png)|![Chrome](images/chromeIcon.png)|![Safari](images/safariIcon.png)|![Opera](images/operaIcon.png)|![Samsung Internet](images/samsungInternetIcon.png)|
|----|----|----|----|----|----|----|
|**Microsoft Edge**|**Firefox**|**Chrome**|**Safari**|**Opera**|**Samsung**|

## <a name="next-steps"></a>Дальнейшие действия

- Попробуйте компоненты в [интерактивной среде](https://mgt.dev).
- [Начало работы](./get-started/overview.md) с Microsoft Graph Toolkit.
- Ознакомьтесь с Microsoft Graph Toolkit на [GitHub](https://aka.ms/mgt).
