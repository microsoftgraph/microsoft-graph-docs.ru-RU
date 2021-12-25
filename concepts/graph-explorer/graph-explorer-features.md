---
title: Работа с песочницей Graph
description: Узнайте, как использовать некоторые важные функции песочницы Graph.
ms.localizationpriority: high
author: RabebOthmani
ms.openlocfilehash: bfbde32a895118816bfaa3553582d7733880bbc1
ms.sourcegitcommit: 9759b647acfbed99d5675a6f512aaa33932a723f
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/23/2021
ms.locfileid: "61604289"
---
# <a name="working-with-graph-explorer"></a>Работа с песочницей Graph

[Песочница Graph](https://developer.microsoft.com/graph/graph-explorer/) — это средство для разработчика, при помощи которого удобно создавать запросы REST API Microsoft Graph и просматривать их ответы. В этой статье вы узнаете, как использовать некоторые важные функции песочницы Graph.

## <a name="consent-to-permissions"></a>Согласие на разрешения

Для доступа к данным в Microsoft Graph пользователь или администратор должны предоставить песочнице Graph правильные разрешения с помощью процесса согласия. Дайте согласие на разрешения в песочнице Graph Explorer на вкладке **Изменить разрешения** или в разделе **Выбрать разрешения**, который можно открыть, нажав на значок шестеренки, появляющийся рядом со значком профиля пользователя, когда тот вошел в учетную запись. На вкладке **Изменить разрешения** перечислены все разрешения, необходимые для запуска запроса в адресной строке. 

Чтобы дать согласие на разрешения:

1.  Выберите пример запроса и запустите его.
2.  Выберите вкладку **Изменить разрешения**.
3.  Просмотрите список разрешений, необходимых для выполнения запроса.
4.  Выберите кнопку "Дать согласие" рядом с разрешением, на которое требуется дать согласие. 

![Снимок экрана песочницы Graph, на котором выделена последовательность действий, позволяющая дать согласие на разрешения](./images/modify-permissions.png)

Функция **Изменить разрешения** в настоящее время находится в предварительной версии, и разрешения на некоторые запросы могут отсутствовать. Если вы не видите разрешений, необходимых для какого-либо запроса, зайдите в раздел **Выбрать разрешения**, нажав на значок шестеренки, появляющийся рядом со значком профиля пользователя, когда тот вошел в учетную запись.:

1.  Щелкните значок шестеренки, а затем **Выбрать разрешения**. Вы увидите список всех доступных разрешений.
2.  Найдите в списке всех разрешений нужные и дайте согласие на них.

![Снимок экрана песочницы Graph с развернутым разделом "Выбрать разрешения"](./images/select-permissions.png)

## <a name="get-an-access-or-authentication-token"></a>Получить маркер доступа или проверки подлинности

В песочнице Graph есть вкладка **Маркер доступа**: она показывает маркер доступа, когда пользователь выполнил вход в учетную запись. На вкладке **Маркер доступа** можно скопировать маркер, если вы хотите использовать его в своем любимом клиентском REST-приложении.

![Снимок экрана вкладки "Маркер доступа" в песочнице Graph с выделенной кнопкой "Копировать"](./images/access-token.png)

## <a name="copy-code-snippets"></a>Копировать фрагменты кода

Для каждого запроса REST API, который вы выбираете или вводите в песочнице Graph, способ вызова этого API на каждом из четырех языков (C#, Java, JavaScript и Objective-C) можно найти на вкладке **Фрагменты кода**. 

![Снимок экрана песочницы Graph с выделенной вкладкой "Фрагменты кода"](./images/code-snippets.png)

## <a name="ui-component-integration"></a>Интеграция компонентов пользовательского интерфейса

Песочница Graph содержит несколько функций, упрощающих реализацию пользовательского интерфейса. Вы можете использовать эти компоненты при создании приложений.

### <a name="microsoft-graph-toolkit-integration"></a>Интеграция Microsoft Graph Toolkit

[Microsoft Graph Toolkit](../toolkit/overview.md) — это набор многократно используемых, не зависящих от платформы веб-компонентов и вспомогательных средств для доступа и работы в Microsoft Graph. Компоненты полностью функциональны, со встроенными поставщиками, которые проводят проверку подлинности с помощью Microsoft Graph и извлекают из него данные.

Песочница Graph предоставляет примеры запросов REST API, соответствующих компонентам Microsoft Graph Toolkit. Синяя точка на вкладке **Компонент Toolkit** указывает, что Toolkit предоставляет компонент для указанного в настоящее время в песочнице Graph запроса REST API. Код компонента удобно скопировать в приложение.

В следующей таблице перечислены примеры запросов, которые в настоящее время содержат компонент Toolkit.

| **Пример запроса в песочнице Graph** | **Пример URL-адреса iFrame из Toolkit** |
| --- | --- |
| GET мой профиль | [https://mgt.dev/iframe.html?id=components-mgt-person-card — компонент для вывода информации при наведении курсора мыши на карточку контакта](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fmgt.dev%2Fiframe.html%3Fid%3Dcomponents-mgt-person-card--person-card-hover&amp;data=04%7C01%7CElise.Yang%40microsoft.com%7Ca81f0f07873240d8571b08d7dac329d4%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637218404083362882%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&amp;sdata=9FvGlMZNc78EE66JiY7hrusYVuGUm2NeflYlVgwTVwo%3D&amp;reserved=0) |
| Получить информацию о людях, с которыми я работаю | [https://mgt.dev/iframe.html?id=components-mgt-people—Люди](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fmgt.dev%2Fiframe.html%3Fid%3Dcomponents-mgt-people--people&amp;data=04%7C01%7CElise.Yang%40microsoft.com%7Ca81f0f07873240d8571b08d7dac329d4%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637218404083372878%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&amp;sdata=yMF3X0M%2FmvWTUfhMdNYkG5I7fDMXpPHS6Fwea%2B3ycPs%3D&amp;reserved=0) |
| Получить все мои задачи Планировщика | [https://mgt.dev/iframe.html?id=components-mgt-tasks—задачи](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fmgt.dev%2Fiframe.html%3Fid%3Dcomponents-mgt-tasks--tasks&amp;data=04%7C01%7CElise.Yang%40microsoft.com%7Ca81f0f07873240d8571b08d7dac329d4%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637218404083382869%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&amp;sdata=Vk5IhPb%2FNbni7c6bteEveIdQNn%2BPm6AchwewCJ%2Fkmzk%3D&amp;reserved=0) |
| Получить мои мероприятия на следующую неделю | [https://mgt.dev/iframe.html?id=components-mgt-agenda—get-events-for-next-week](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fmgt.dev%2Fiframe.html%3Fid%3Dcomponents-mgt-agenda--get-events-for-next-week&amp;data=04%7C01%7CElise.Yang%40microsoft.com%7Ca81f0f07873240d8571b08d7dac329d4%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637218404083382869%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&amp;sdata=VVFcx3gXMmg%2B%2BdQCZXjAmkCk5zKcrntK6fI35jbdN94%3D&amp;reserved=0) |
| Получение своей фотографии | [https://mgt.dev/iframe.html?id=components-mgt-person—person-photo-only](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fmgt.dev%2Fiframe.html%3Fid%3Dcomponents-mgt-person--person-photo-only&amp;data=04%7C01%7CElise.Yang%40microsoft.com%7Ca81f0f07873240d8571b08d7dac329d4%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637218404083392872%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&amp;sdata=aI%2BUqciLPOxEqlIpbjT8wtWBgcaJWM6sqooRlLVspZ0%3D&amp;reserved=0) |

![Снимок экрана, показывающий выделенную вкладку "Компоненты Toolkit" с кодом для создания компонента](./images/get-graph-toolkit-card.png)

### <a name="adaptive-cards-integration"></a>Интеграция адаптивных карточек

[Адаптивные карточки](https://adaptivecards.io/) — это платформо-независимые фрагменты пользовательского интерфейса, созданные в формате JSON, которыми можно открыто обмениваться в приложениях и службах. При запуске запроса и при наличии доступной адаптивной карты на вкладке **Адаптивные карты** появляется синяя точка.

![Снимок экрана вкладки адаптивных карт в песочнице Graph с выделенными данными ответа](./images/adaptive-cards.png)

## <a name="customize-the-theme-in-graph-explorer"></a>Настройка темы в песочнице Graph

Выберите тему для песочницы Graph, щелкнув раздел **Изменение темы**, который можно открыть, выбрав шестеренку "Параметры". Варианты тем: светлая, темная и контрастная.

![Снимок экрана изменения темы в песочнице Graph с выделенными вариантами темы](./images/change-theme.png)

## <a name="storing-and-sharing-queries"></a>Хранение запросов и предоставление доступа к ним

Запросы, запущенные в песочнице Graph, сохраняются в течение 30 дней на вкладке **Журнал**. На вкладке "Журнал" можно:

1.  Экспортировать все записи журнала в формате `.har`.
2.  Удалить все записи журнала.
3.  Просмотреть запись журнала.
4.  Выполнить запрос
5.  Экспортировать запись журнала в формате `.har`.
6.  Удалить запись журнала.

![Снимок экрана вкладки "Журнал" с выделенными параметрами](./images/storing-and-sharing-queries.png)

Чтобы предоставить кому-либо доступ к созданному вами запросу, щелкните кнопку "Поделиться запросом" в панели ответа и выберите **Копировать**. Будет скопирована ссылка для обмена, которая позволит другим пользователям увидеть ваш запрос и результаты.

![Снимок экрана песочницы Graph с выделенными командами "Поделиться" и "Копировать"](./images/share-query.png)

## <a name="graph-explorer-ui-features"></a>Возможности пользовательского интерфейса песочницы Graph

Компонент боковой панели в песочнице Graph можно развернуть или, наоборот, свернуть, если требуется расширить области запроса и ответа. Чтобы свернуть компонент боковой панели, выберите значок гамбургера в верхней левой части боковой панели.

![Снимок экрана песочницы Graph с выделенными командами "Развернуть" и "Свернуть"](./images/expand-collapse-sidebar-component.png)

Развернуть и свернуть предварительный просмотр ответа можно, выбрав стрелку расширения в окне предварительного просмотра ответа.

![Снимок экрана области ответа с выделенными командами "Развернуть" и "Свернуть"](./images/expand-collapse-response-preview.png)

На сайт программы для разработчиков Microsoft 365 удобно заходить из пользовательского интерфейса песочницы Graph, получая бесплатную песочницу с образцами данных для экспериментов. Нажмите на шестеренку, чтобы войти в раздел настроек, и выберите **Получить песочницу с образцом данных**.

![Снимок экрана песочницы Graph с выделенной командой "Получить песочницу с образцом данных"](./images/link-to-m365-dev-program.png)


## <a name="next-steps"></a>Дальнейшие действия

- Зайти в [песочницу Graph](https://developer.microsoft.com/graph/graph-explorer/) и ознакомиться с примерами запросов.
- Ознакомиться с [документацией Microsoft Graph Toolkit](../toolkit/overview.md).
- Добавить пример или оставить отзыв или предложение в [репозитории GitHub песочницы Graph](https://github.com/microsoftgraph/microsoft-graph-explorer-v4/issues/new/choose).
