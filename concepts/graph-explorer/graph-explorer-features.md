---
title: Работа с graph Explorer
description: Узнайте, как использовать некоторые важные функции в обозревателе Graph.
localization_priority: Normal
author: bettirosengugi
ms.openlocfilehash: b4c669ae6983efe2082b623c3de5b019a049311d
ms.sourcegitcommit: 7dc8ca82a8b2c25c5084e6b3121688766c9c14a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/02/2021
ms.locfileid: "50072394"
---
# <a name="working-with-graph-explorer"></a>Работа с graph Explorer

[Graph Explorer](https://developer.microsoft.com/graph/graph-explorer/) — это средство разработчика, которое позволяет удобно создавать запросы REST API Microsoft Graph и просматривать соответствующие ответы. В этой статье описывается использование некоторых важных функций в обозревателе Graph.

## <a name="consent-to-permissions"></a>Согласие на разрешения

Пользователь или администратор должен предоставить graph Explorer правильные разрешения с помощью процесса согласия на доступ к данным в Microsoft Graph. Согласие на разрешения в проводнике  Graph с помощью  вкладки "Изменение разрешений" или параметра "Выбор разрешений" в шестеренке параметров рядом с профилем при выходе в систему. На **вкладке "Изменение разрешений"** перечислены все разрешения, необходимые для выполнения запроса в адресной панели. 

Чтобы дать согласие на разрешения:

1.  Выберите пример запроса и запустите его.
2.  Выберите **вкладку "Изменение разрешений".**
3.  См. список разрешений, необходимых для выполнения запроса.
4.  Выберите кнопку согласия рядом с разрешением, на который вы хотите согласиться. 

![Screenshot of Graph Explorer with the steps to consent to permissions highlighted](./images/modify-permissions.png)

Функция **"Изменение разрешений"** в настоящее время находится на стадии предварительного просмотра, и в некоторых запросах могут от отсутствуют разрешения. Если для запроса отсутствуют разрешения, параметр **"Выбор** разрешений" в шестеренки параметров рядом с профилем содержит список всех доступных разрешений:

1.  Перейдите к шестеренкой параметров и выберите параметр **"Выбор** разрешений". Этот параметр содержит список всех доступных разрешений.
2.  Из списка всех разрешений согласиться с нужными разрешениями.

![Снимок экрана: обозреватель Graph с выделенной опцией "Выбор разрешений"](./images/select-permissions.png)

## <a name="get-an-access-or-authentication-token"></a>Получить маркер доступа или проверки подлинности

В проводнике Graph есть вкладка **маркера доступа,** на которую указывается маркер доступа при входе. На **вкладке маркера Access** вы можете скопировать маркер, если его необходимо использовать в своем любимом клиентских приложениях REST.

![Снимок экрана: вкладка маркера доступа в обозревателе Graph с выделенной кнопкой "Копировать"](./images/access-token.png)

## <a name="copy-code-snippets"></a>Копирование фрагментов кода

Для каждого запроса REST API, который вы выбираете или вводите в обозревателе Graph,  вы можете узнать, как вызывать этот API на каждом из четырех языков, демонстрируемых на вкладке "Фрагменты кода" — C#, Java, JavaScript и Objective-C. 

![Снимок экрана: обозреватель Graph с выделенной вкладками фрагментов кода](./images/code-snippets.png)

## <a name="ui-component-integration"></a>Интеграция компонентов пользовательского интерфейса

В проводнике Graph есть несколько функций, упрощающих реализацию пользовательского интерфейса. Повторное использование этих компонентов и в приложениях.

### <a name="microsoft-graph-toolkit-integration"></a>Интеграция набор средств Microsoft Graph

Microsoft [Graph набор средств](/graph/toolkit/overview) — это коллекция веб-компонентов, которые не зависит от структуры, и помощников для доступа к Microsoft Graph и работы с ним. Эти компоненты полностью функциональны и имеют встроенные поставщики, которые аутентификация и извлечение данных из Microsoft Graph.

В проводнике Graph есть примеры запросов REST API, которые соответствуют набор средств Microsoft Graph. Синяя точка на вкладке **набор средств** компонента указывает, что набор средств предоставляет компонент для указанного в настоящее время запроса REST API в обозревателе Graph. Вы можете легко скопировать код компонента в приложение.

В следующей таблице перечислены примеры запросов, которые в настоящее время включают набор средств компонента.

| **Пример запроса в проводнике Graph** | **набор средств примере URL-адреса iFrame** |
| --- | --- |
| GET мой профиль | [https://mgt.dev/iframe.html?id=components-mgt-person-card- person-card-hover](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fmgt.dev%2Fiframe.html%3Fid%3Dcomponents-mgt-person-card--person-card-hover&amp;data=04%7C01%7CElise.Yang%40microsoft.com%7Ca81f0f07873240d8571b08d7dac329d4%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637218404083362882%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&amp;sdata=9FvGlMZNc78EE66JiY7hrusYVuGUm2NeflYlVgwTVwo%3D&amp;reserved=0) |
| Get people I work with | [https://mgt.dev/iframe.html?id=components-mgt-people— people](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fmgt.dev%2Fiframe.html%3Fid%3Dcomponents-mgt-people--people&amp;data=04%7C01%7CElise.Yang%40microsoft.com%7Ca81f0f07873240d8571b08d7dac329d4%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637218404083372878%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&amp;sdata=yMF3X0M%2FmvWTUfhMdNYkG5I7fDMXpPHS6Fwea%2B3ycPs%3D&amp;reserved=0) |
| GET все мои задачи планировщика | [https://mgt.dev/iframe.html?id=components-mgt-tasks- tasks](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fmgt.dev%2Fiframe.html%3Fid%3Dcomponents-mgt-tasks--tasks&amp;data=04%7C01%7CElise.Yang%40microsoft.com%7Ca81f0f07873240d8571b08d7dac329d4%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637218404083382869%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&amp;sdata=Vk5IhPb%2FNbni7c6bteEveIdQNn%2BPm6AchwewCJ%2Fkmzk%3D&amp;reserved=0) |
| Get my events for the next week | [https://mgt.dev/iframe.html?id=components-mgt-agenda— get-events-for-next-week](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fmgt.dev%2Fiframe.html%3Fid%3Dcomponents-mgt-agenda--get-events-for-next-week&amp;data=04%7C01%7CElise.Yang%40microsoft.com%7Ca81f0f07873240d8571b08d7dac329d4%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637218404083382869%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&amp;sdata=VVFcx3gXMmg%2B%2BdQCZXjAmkCk5zKcrntK6fI35jbdN94%3D&amp;reserved=0) |
| Получение своей фотографии | [https://mgt.dev/iframe.html?id=components-mgt-person-person-photo-only](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fmgt.dev%2Fiframe.html%3Fid%3Dcomponents-mgt-person--person-photo-only&amp;data=04%7C01%7CElise.Yang%40microsoft.com%7Ca81f0f07873240d8571b08d7dac329d4%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637218404083392872%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&amp;sdata=aI%2BUqciLPOxEqlIpbjT8wtWBgcaJWM6sqooRlLVspZ0%3D&amp;reserved=0) |

![Screenshot showing the набор средств components tab with the code to generate the component highlighted](./images/get-graph-toolkit-card.png)

### <a name="adaptive-cards-integration"></a>Интеграция адаптивных карточек

[Адаптивные карточки](https://adaptivecards.io/) — это не зависит от платформы фрагменты пользовательского интерфейса, авторские в JSON, которые приложения и службы могут открыто обмениваться. При запуске запроса и наличии адаптивной карточки на вкладке адаптивных карт появляется синяя **точка.**

![Screenshot of the adaptive cards tab in Graph Explorer with the response details highlighted](./images/adaptive-cards.png)

## <a name="customize-the-theme-in-graph-explorer"></a>Настройка темы в обозревателе Graph

Выберите тему для проводника Graph, выбрав параметр "Изменить **тему"** под шестеренкой параметров. Параметры темы: Light, Dark и High contrast.

![Снимок экрана: параметр "Изменить тему" в обозревателе Graph с выделенной темой](./images/change-theme.png)

## <a name="storing-and-sharing-queries"></a>Хранение запросов и совместное использование

Запросы, которые запускаются в проводнике Graph, сохраняются в течение 30 дней на вкладке **"История".** На вкладке "История" можно:

1.  Экспортировать все элементы истории в формате .har.
2.  Удаление всех элементов истории.
3.  Просмотр этого элемента истории.
4.  Запустите этот запрос.
5.  Экспортировать этот элемент истории в формате .har.
6.  Удалите этот элемент истории.

![Снимок экрана: вкладка "История" с выделенной опцией](./images/storing-and-sharing-queries.png)

Чтобы поделиться запросами, нажмите кнопку "Поделиться запросом" в области ответа и нажмите кнопку **"Копировать".** Это копирует ссылку для обмена и позволяет другим пользователям видеть ваш запрос и результаты.

![Снимок экрана: обозреватель Graph с выделенной опцией "Поделиться" и "Копировать"](./images/share-query.png)

## <a name="graph-explorer-ui-features"></a>Функции пользовательского интерфейса проводника Graph

Свернуть и развернуть компонент боковой панели в обозревателе Graph, чтобы расширить область запроса и ответа. Чтобы свернуть компонент боковой панели, выберите значок гамбургера в верхней левой части боковой панели.

![Снимок экрана: обозреватель Graph с выделенной опцией расширения и свернутого экрана](./images/expand-collapse-sidebar-component.png)

Раз развернуть и свернуть предварительный просмотр отклика, выбрав стрелку в окне предварительного просмотра отклика.

![Screenshot of the response pane with the expand and collapse options highlighted](./images/expand-collapse-response-preview.png)

Удобный доступ к сайту программы для разработчиков Microsoft 365 из пользовательского интерфейса песочницы Graph, чтобы получить бесплатную песочницу с примерами данных для экспериментов. Под шестеренкой параметра выберите **"Получить песочницу" с примерами данных.**

![Screenshot of Graph Explorer with the Get a sandbox with sample data option highlighted](./images/link-to-m365-dev-program.png)


## <a name="next-steps"></a>Дальнейшие действия

- Посетите [обозреватель Graph и](https://developer.microsoft.com/graph/graph-explorer/) изучите примеры запросов.
- Изучите [документацию по набор средств Microsoft Graph.](/graph/toolkit/overview)
- Участие или предоставление отзывов в [репозитарии GitHub в обозревателе Graph.](https://github.com/microsoftgraph/microsoft-graph-explorer-v4/issues/new/choose)
