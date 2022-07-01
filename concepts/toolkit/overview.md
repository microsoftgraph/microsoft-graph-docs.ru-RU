---
title: Обзор Microsoft Graph Toolkit
description: Используйте Microsoft Graph Toolkit для поиска поставщиков проверки подлинности и многократно используемых веб-компонентов, не зависящие от платформы, для доступа к Microsoft Graph и работы с ним.
ms.localizationpriority: medium
author: sebastienlevert
ms.openlocfilehash: a448d79a789f142a2e05bca0e4096db9df127158
ms.sourcegitcommit: af9489bd42a25dff04836dcfcc57369259fda587
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2022
ms.locfileid: "66577807"
---
# <a name="microsoft-graph-toolkit-overview"></a>Обзор Microsoft Graph Toolkit 

Microsoft Graph Toolkit — это коллекция многократно используемых, не зависящих от платформы компонентов и поставщиков проверки подлинности для доступа и работы в Microsoft Graph. Готовые компоненты полностью функциональны и включают встроенных поставщиков, которые проверяют подлинность и получают данные из Microsoft Graph.

Microsoft Graph Toolkit позволяет легко использовать Microsoft Graph в своем приложении. В следующем примере пользователь, выполнив вход, и его события календаря отображаются только с двумя строками кода с помощью компонентов ["](./components/login.md) Вход" и ["Повестка](./components/agenda.md) дня".

<iframe src="https://mgt.dev/iframe.html?id=samples-general--login-to-show-agenda&source=docs&source=docs" height="400"></iframe>

[Откройте этот пример в mgt.dev](https://mgt.dev/?path=/story/samples-general--login-to-show-agenda&source=docs).

## <a name="whats-in-microsoft-graph-toolkit"></a>Что такое Microsoft Graph Toolkit?

### <a name="components"></a>Компоненты

Microsoft Graph Toolkit включает в себя коллекцию веб-компонентов для наиболее часто созданных интерфейсов на основе API Microsoft Graph.

Они также доступны как [компоненты React](./get-started/mgt-react.md).

|Компонент|Описание|
|---------|-----------|
|[Вход](./components/login.md)|Кнопка и всплывающий элемент управления для проверки подлинности пользователя с помощью платформы удостоверений Майкрософт и отображения сведений о профиле пользователя при входе в систему.|
|[Человек](./components/person.md)|Отображает пользователя или контакт с помощью его фотографии, имени и/или адреса электронной почты.|
|[Люди](./components/people.md)|Отображает группу людей или контактов с помощью их фотографий или инициалов.|
|[Повестка дня](./components/agenda.md)|Отображает события в календаре пользователя или группы.|
|[Выбор людей](./components/people-picker.md)|Предоставляет возможность поиска людей и отображает список результатов.|
|[Карточка контакта](./components/person-card.md)|Всплывающий элемент, который используется в компоненте "Человек", чтобы отобразить больше сведений профиля о пользователе.|
|[Файл](./components/file.md)|Представляет файл или папку со значком, именем файла, автором и т. д.|
|[Список файлов](./components/file-list.md)|Отображает список из нескольких файлов или папок.|
|[Получение](./components/get.md)|Позволяет выполнять запрос GET к любому приложению Майкрософт API Graph непосредственно в HTML-коде.|
|[Средство выбора каналов](./components/teams-channel-picker.md)|Предоставляет возможность поиска каналов Microsoft Teams и выбора канала из отображенного списка результатов.|
|[To Do](./components/todo.md)|Отображает и включает добавление, удаление, выполнение или редактирование задач из Microsoft To Do.|
|[Задачи](./components/tasks.md)|Отображает и включает добавление, удаление, выполнение или редактирование задач из Планировщика (Майкрософт) или Microsoft To Do.|

### <a name="providers"></a>Поставщики

[Поставщики](./providers/providers.md) обеспечивают проверку подлинности, предоставляют реализацию для получения маркеров доступа на различных платформах и предоставляют клиент Microsoft Graph для вызова API Microsoft Graph. Компоненты работают наилучшим образом, если используются с поставщиком, однако поставщики могут использоваться самостоятельно.

|Поставщики|Описание|
|---------|-----------|
|[MSAL](./providers/msal.md)|Использует msal.js для входа пользователей и получения маркеров для использования с Microsoft Graph.|
|[MSAL2](./providers/msal2.md)| Использует msal-browser для входа пользователей и получения маркеров для использования с Microsoft Graph.|
|[Электрон](./providers/electron.md)|Выполняет проверку подлинности и предоставляет Microsoft Graph доступ к компонентам в приложениях Electron.|
|[SharePoint](./providers/sharepoint.md)|Проверяет подлинность и предоставляет Microsoft Graph доступ к компонентам в веб-частях SharePoint.|
|[Teams](./providers/teams.md)|Использует msal.js для входа пользователей и получения маркеров на клиенте на вкладке Microsoft Teams.|
|[Teams MSAL2](./providers/teams-msal2.md)|Использует msal-browser для входа пользователей и получения маркеров на вкладке Microsoft Teams. Поддерживает единый вход (SSO) с настраиваемой серверной частью. |
|[Прокси-сервер](./providers/proxy.md)|Позволяет использовать проверку подлинности на внутреннем сервере с помощью маршрутизации всех вызовов Microsoft Graph через внутренний сервер.|
|[Настраиваемый](./providers/custom.md)|Создает настраиваемый поставщик для включения проверки подлинности и доступа к Microsoft Graph с помощью существующего кода проверки подлинности приложения.|

## <a name="why-use-microsoft-graph-toolkit"></a>Зачем использовать Microsoft Graph Toolkit?

Microsoft Graph Toolkit позволяет быстро и легко интегрировать общие возможности на базе Microsoft Graph в собственное приложение. Набор средств:

- **Сокращает время разработки**. Работа по подключению к API Microsoft Graph и отрисовке данных в пользовательском интерфейсе, который выглядит и выглядит как Интерфейс Microsoft 365, выполняется за вас без необходимости настройки.

- **Работает везде**. Все компоненты основаны на веб-стандартах и легко работают с любым современным браузером и веб-платформой (например, React, Angular или Vue). 

- **Привлекательный, но гибкий.** Компоненты предназначены для того, чтобы выглядеть и выглядеть как интерфейсы Microsoft 365, но также настраиваются с помощью настраиваемых свойств [CSS](./customize-components/style.md) и [шаблонов](./customize-components/templates.md).

## <a name="who-should-use-it"></a>Кто должен его использовать?

Microsoft Graph Toolkit отлично подходит для разработчиков всех уровней взаимодействия, которые хотят разработать приложение, которое подключается к данным Из Microsoft Graph и имеет доступ к ним, например:
- Веб-приложение
- Вкладка Microsoft Teams
- Прогрессивное веб-приложение (PWA)
- Приложение Electron
- Веб-часть SharePoint

## <a name="where-can-i-use-it"></a>Где его можно использовать?

Microsoft Graph Toolkit поддерживается в следующих браузерах:

|![Microsoft Edge](images/edgeIcon.png)|![Firefox](images/firefoxIcon.png)|![Chrome](images/chromeIcon.png)|![Safari](images/safariIcon.png)|![Opera](images/operaIcon.png)|![Samsung Internet](images/samsungInternetIcon.png)|
|----|----|----|----|----|----|----|
|**Microsoft Edge**|**Firefox**|**Chrome**|**Safari**|**Opera**|**Samsung**|

## <a name="next-steps"></a>Дальнейшие действия

- Попробуйте компоненты в [интерактивной среде](https://mgt.dev).
- [Начало работы с](./get-started/overview.md) Microsoft Graph Toolkit.
- Ознакомьтесь с Microsoft Graph Toolkit на [сайте GitHub](https://aka.ms/mgt).
