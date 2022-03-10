---
title: Обзор API Поиска (Майкрософт) в Microsoft Graph
description: Используйте API Поиска (Майкрософт) для индексирования контента и добавления в приложения функций поиска в Office и индексированном контенте.
ms.localizationpriority: high
ms.prod: search
author: snlraju-msft
scenarios: getting-started
ms.openlocfilehash: 5e50b61d2989f01eefd61d1d318da174c9a53421
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63336216"
---
# <a name="overview-of-the-microsoft-search-api-in-microsoft-graph"></a>Обзор API Поиска (Майкрософт) в Microsoft Graph

Поиск (Майкрософт) — это корпоративная поисковая система, обеспечивающая повышение производительности и релевантные результаты поиска для организации. Она использует наработки и возможности организации и отображает актуальный релевантный контент для пользователей. Поиск (Майкрософт) доступен в различных программах, включая Office, SharePoint, Delve, Windows и Bing. Вы можете использовать API Поиска (Майкрософт) в Microsoft Graph, чтобы Поиск (Майкрософт) распространялся и на ваши приложения.  

<!-- markdownlint-disable MD026 -->
## <a name="why-use-the-microsoft-search-api"></a>Зачем использовать API Поиска (Майкрософт)?

### <a name="one-unified-search-endpoint-for-microsoft-cloud-data"></a>Единая конечная точка поиска для данных Microsoft Cloud

API Поиска (Майкрософт) предоставляет единую конечную точку поиска, которую можно использовать для [запроса](/graph/api/search-query) в Microsoft Cloud данных (сообщений и событий в почтовых ящиках Outlook, а также файлов в OneDrive и SharePoint), индексированных в Поиске (Майкрософт).

### <a name="include-custom-external-data-in-search-experience"></a>Включение настраиваемых внешних данных в интерфейс поиска

Используйте [соединители Microsoft Graph](/microsoftsearch/connectors-overview), чтобы включить данные, не входящие в Microsoft Cloud, в возможности поиска. Например, можно подключиться к базе данных отдела кадров организации или к каталогу продукции. Затем используйте API Поиска (Майкрософт), чтобы [запрашивать](/graph/api/search-query) внешний источник данных. 

Просмотрите [коллекцию соединителей Microsoft Graph](/microsoftsearch/connectors-gallery), чтобы найти готовые к использованию соединители. Вы также можете [создавать собственные соединители](/graph/api/resources/indexing-api-overview?view=graph-rest-beta&preserve-view=true#common-use-cases), чтобы индексировать внешние настраиваемые элементы и отправлять запросы к определенным внешним источникам данных.

### <a name="consistent-up-to-date-search-experience"></a>Единый актуальный интерфейс поиска

При использовании API Поиска (Майкрософт) пользователи получают персонализированные релевантные результаты благодаря Microsoft Graph. Поиск в ваших приложениях вернет результаты, согласованные с поиском в приложениях Office.

## <a name="what-data-can-i-add-or-access-by-using-the-microsoft-search-api"></a>Какие данные можно добавить и к каким получить доступ с помощью API Поиска (Майкрософт)?

API Поиска (Майкрософт) поддерживает поиск следующего контента в Microsoft Cloud: 

- Ресурсы [message](/graph/api/resources/message) почты Outlook и [event](/graph/api/resources/event) календаря.
- Файлы и папки в SharePoint и OneDrive (ресурсы [driveItem](/graph/api/resources/driveitem)), ресурсы [list](/graph/api/resources/list), [listItem](/graph/api/resources/listitem), [site](/graph/api/resources/site) и [drive](/graph/api/resources/drive).
- Ресурсы [person](/graph/api/resources/person) в организации, наиболее релевантные для пользователя.
- Содержимое, отправляемое через платформу соединителей Microsoft Graph: ресурсы [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true).
- Ресурсы ответов административного поиска: ресурсы [acronyms](/graph/api/resources/search-acronym), [bookmarks](/graph/api/resources/search-bookmark) и [QnA](/graph/api/resources/search-qna).

## <a name="api-reference"></a>Справочные материалы по API

Ищете справочные материалы по API для этой службы?

- [Использование API Поиска (Майкрософт) для запроса данных](/graph/api/resources/search-api-overview?view=graph-rest-1.0&preserve-view=true)(версия 1.0)
- [Использование API Поиска (Майкрософт) для запроса данных](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true)(предварительная версия)
- [Использование API Поиска (Майкрософт) для индексирования данных](/graph/api/resources/indexing-api-overview) (предварительная версия)
- [Используйте API Поиска (Майкрософт) для управления ответами административного поиска](/graph/api/resources/search-api-answers-overview?view=graph-rest-beta&preserve-view=true) (предварительная версия)

## <a name="next-steps"></a>Дальнейшие действия

- Подробнее о [Поиске (Майкрософт)](/microsoftsearch/).
- Подробнее о некоторых основных вариантах использования:
  - [Управление подключениями для индексирования внешнего контента](connecting-external-content-manage-connections.md)
  - [Индексирование внешнего контента](connecting-external-content-manage-items.md)
  - [Поиск сообщений Outlook](search-concept-messages.md)
  - [Поиск событий календаря](search-concept-events.md)
  - [Поиск содержимого в OneDrive и SharePoint](search-concept-files.md)
  - [Поиск внешнего контента](search-concept-custom-types.md)
  - [Поиск человека](search-concept-person.md) (предварительная версия)
  - [Управление ответами административного поиска](search-concept-answers.md) (предварительная версия)
  - [Управление макетом результатов поиска](search-concept-display-layout.md) (предварительная версия)
  - [Уточнение результатов поиска](search-concept-aggregation.md)
  - [Исправление орфографии в запросе](search-concept-speller.md) (предварительная версия)
  - [Сортировка результатов поиска](search-concept-sort.md)
- Узнайте больше об API поиска в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer).
- Скачайте [образец соединителя поиска](https://github.com/microsoftgraph/msgraph-search-connector-sample) в GitHub.
- Участвуйте в работе сообщества на сайте [Вопросы и ответы Майкрософт](/answers/products/m365#microsoft-graph) или на GitHub.
