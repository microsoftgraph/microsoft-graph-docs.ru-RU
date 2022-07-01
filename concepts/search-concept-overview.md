---
title: Обзор Microsoft Search API в Microsoft Graph
description: Используйте Microsoft Search API в Microsoft Graph, чтобы расширить возможности Microsoft Search в своих приложениях. Запрашивайте данные, которые Microsoft Search индексирует и включает настраиваемые внешние данные.
ms.localizationpriority: high
ms.prod: search
author: snlraju-msft
scenarios: getting-started
ms.openlocfilehash: ee2a62e6be739122140ccadefd993e069fa9e6cd
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66446093"
---
# <a name="overview-of-the-microsoft-search-api-in-microsoft-graph"></a>Обзор API Поиска (Майкрософт) в Microsoft Graph

Поиск (Майкрософт) — это корпоративная поисковая система, обеспечивающая повышение производительности и релевантные результаты поиска для организации. Она использует наработки и возможности организации и отображает актуальный релевантный контент для пользователей. Поиск (Майкрософт) доступен в различных программах, включая Office, SharePoint, Delve, Windows и Bing. Вы можете использовать API Поиска (Майкрософт) в Microsoft Graph, чтобы Поиск (Майкрософт) распространялся и на ваши приложения.  

<!-- markdownlint-disable MD026 -->
## <a name="why-use-the-microsoft-search-api"></a>Зачем использовать API Поиска (Майкрософт)?

### <a name="one-unified-search-endpoint-for-microsoft-cloud-data"></a>Единая конечная точка поиска для данных Microsoft Cloud

Microsoft Search API предоставляет одну унифицированную конечную точку поиска, которую можно использовать для [запроса](/graph/api/search-query) данных в облачных&mdash;сообщениях Microsoft и событиях в почтовых ящиках Outlook и файлах в OneDrive и SharePoint&mdash;, которые Microsoft Search уже индексирует.

### <a name="include-custom-external-data-in-search-experience"></a>Включение настраиваемых внешних данных в интерфейс поиска

Используйте [соединители Microsoft Graph](/microsoftsearch/connectors-overview), чтобы включить данные, не входящие в Microsoft Cloud, в возможности поиска. Например, можно подключиться к базе данных отдела кадров организации или к каталогу продукции. Затем используйте API Поиска (Майкрософт), чтобы [запрашивать](/graph/api/search-query) внешний источник данных.

Просмотрите [коллекцию соединителей Microsoft Graph](/microsoftsearch/connectors-gallery), чтобы найти готовые к использованию соединители. Вы также можете [создавать собственные соединители](/graph/api/resources/indexing-api-overview#common-use-cases), чтобы индексировать внешние настраиваемые элементы и отправлять запросы к определенным внешним источникам данных.

### <a name="consistent-up-to-date-search-experience"></a>Единый актуальный интерфейс поиска

При использовании API Поиска (Майкрософт) пользователи получают персонализированные релевантные результаты благодаря Microsoft Graph. Поиск в ваших приложениях вернет результаты, согласованные с поиском в приложениях Office.

## <a name="what-data-can-i-add-or-access-by-using-the-microsoft-search-api"></a>Какие данные можно добавить и к каким получить доступ с помощью API Поиска (Майкрософт)?

API Поиска (Майкрософт) поддерживает поиск следующего контента в Microsoft Cloud: 

- Ресурсы [message](/graph/api/resources/message) почты Outlook и [event](/graph/api/resources/event) календаря.
- Файлы и папки в SharePoint и OneDrive (ресурсы [driveItem](/graph/api/resources/driveitem)), ресурсы [list](/graph/api/resources/list), [listItem](/graph/api/resources/listitem), [site](/graph/api/resources/site) и [drive](/graph/api/resources/drive).
- Ресурсы [person](/graph/api/resources/person) в организации, наиболее релевантные для пользователя.
- Содержимое, отправляемое через платформу соединителей Microsoft Graph: ресурсы [externalItem](/graph/api/resources/externalitem).
- Ресурсы ответов административного поиска: ресурсы [acronyms](/graph/api/resources/search-acronym), [bookmarks](/graph/api/resources/search-bookmark) и [QnA](/graph/api/resources/search-qna).

## <a name="api-reference"></a>Справочные материалы по API

Ищете справочные материалы по API для этой службы?

- [Используйте Microsoft Search API для запроса данных версии 1.0](/graph/api/resources/search-api-overview?view=graph-rest-1.0&preserve-view=true)
- [Используйте Microsoft Search API для запроса бета-данных](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true)
- [Использование API Поиска (Майкрософт) для индексирования данных](/graph/api/resources/indexing-api-overview)
- [Используйте Microsoft Search API для управления бета-версией административных ответов на поиск](/graph/api/resources/search-api-answers-overview?view=graph-rest-beta&preserve-view=true) (предварительная версия)

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
  - [Использование шаблонов запросов](search-concept-query-template.md) (предварительная версия)
  - [Обрезка повторяющихся результатов поиска](search-concept-trim-duplicate.md) (предварительная версия)
- Узнайте больше об API поиска в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer).
- Скачайте [образец соединителя поиска](https://github.com/microsoftgraph/msgraph-search-connector-sample) в GitHub.
- Участвуйте в работе сообщества на сайте [Вопросы и ответы Майкрософт](/answers/products/m365#microsoft-graph) или на GitHub.
