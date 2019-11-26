---
title: Обзор API Поиска (предварительная версия)
description: Узнайте, как использовать API Поиска (Майкрософт) для индексирования контента и добавления в приложения функций поиска в Office и индексированном контенте.
localization_priority: Priority
ms.prod: search
author: snlraju-msft
scenarios: getting-started
ms.openlocfilehash: 6d18decc6e704f5190dd832d78eabf8809a2ca1e
ms.sourcegitcommit: f359d8d3946af55dc76a02bb7bf522a4d50a2707
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/26/2019
ms.locfileid: "39263256"
---
# <a name="overview-for-extending-the-microsoft-search-experience-for-apps-on-microsoft-graph-preview"></a>Обзор расширенных возможностей Поиска (Майкрософт) для приложений в Microsoft Graph (предварительная версия)

Поиск (Майкрософт) — это корпоративная поисковая система, обеспечивающая повышение производительности и релевантные результаты поиска для организации. Она использует наработки и возможности организации и отображает актуальный релевантный контент для пользователей. Поиск (Майкрософт) доступен в различных программах, включая Office, SharePoint, Delve, Windows и Bing. API Поиска (Майкрософт) позволяет приложениям расширять аналогичный интерфейс поиска для пользователей приложений. 

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

<!-- markdownlint-disable MD026 -->
## <a name="why-use-the-microsoft-search-api"></a>Зачем использовать API Поиска (Майкрософт)?

### <a name="one-unified-search-endpoint-for-microsoft-cloud-data"></a>Единая конечная точка поиска для данных Microsoft Cloud

API Поиска (Майкрософт) предоставляет единую конечную точку поиска, позволяющую разработчикам [запрашивать](/graph/api/search-query?view=graph-rest-beta) в Microsoft Cloud данные (сообщения и события в почтовых ящиках Outlook, а также файлы в OneDrive и SharePoint), индексированные в Поиске (Майкрософт).

### <a name="include-custom-external-data-in-search-experience"></a>Включение настраиваемых внешних данных в интерфейс поиска

Пользователи, желающие включить в свой поиск данные, не входящие в Microsoft Cloud, могут использовать [соединители](/microsoftsearch/connectors-overview), чтобы подключиться к определенному источнику данных, такому как база данных отдела кадров организации или каталог продуктов, и использовать API Поиска (Майкрософт) для [запроса](/graph/api/search-query?view=graph-rest-beta) внешнего источника данных. [Коллекция соединителей Microsoft Graph](/microsoftsearch/connectors-gallery) включает ряд готовых к использованию соединителей. Пользователи также могут [создавать соединители](/graph/api/resources/indexing-api-overview?view=graph-rest-beta#common-use-cases), индексировать внешние настраиваемые элементы и файлы и запрашивать определенные внешние источники данных.

### <a name="consistent-up-to-date-search-experience"></a>Единый актуальный интерфейс поиска

Используя API Поиска (Майкрософт), клиенты получают персонализированные релевантные результаты благодаря Microsoft Graph. Кроме того, поиск в ваших приложениях возвращает результаты, согласованные с поиском в приложениях Office.

## <a name="what-data-can-i-add-or-access-by-using-these-apis"></a>Какие данные можно добавить и к каким получить доступ с помощью этих API?

Поиск (Майкрософт) поддерживает поиск следующего контента в Microsoft Cloud:

- Объекты [message](/graph/api/resources/message?view=graph-rest-beta) и [event](/graph/api/resources/event?view=graph-rest-beta) в Outlook
- Файловые объекты [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta) в SharePoint и OneDrive

Кроме того, вы можете индексировать и искать внешний контент:

- Объекты [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta) настраиваемого типа
- Объекты [externalFile](/graph/api/resources/externalfile?view=graph-rest-beta) известного типа

## <a name="api-reference"></a>Справочные материалы по API

Ищете справочные материалы по API для этой службы?

- [Использование API Поиска (Майкрософт) для запроса данных](/graph/api/resources/search-api-overview?view=graph-rest-beta)
- [Использование API Поиска (Майкрософт) для индексирования данных](/graph/api/resources/indexing-api-overview?view=graph-rest-beta)

## <a name="next-steps"></a>Дальнейшие действия

- Подробнее о [Поиске (Майкрософт)](/microsoftsearch/).
- Подробнее о некоторых основных вариантах использования:
  - [Поиск сообщений Outlook](search-concept-messages.md)
  - [Поиск событий календаря](search-concept-events.md)
  - [Управление подключениями для индексирования внешнего контента](search-index-manage-connections.md)
  - [Индексирование внешнего контента](search-index-manage-items.md)
  - [Поиск объектов настраиваемого типа (externalItem)](search-concept-custom-types.md)
  - [Поиск файлов (включая externalFile)](search-concept-files.md)
- Узнайте больше об API в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer).
- Скачайте [образец соединителя поиска](https://github.com/microsoftgraph/msgraph-search-connector-sample) в GitHub.

## <a name="see-also"></a>См. также

Взаимодействие с сообществом:

- [Обсуждения на сайте StackOverflow](https://stackoverflow.com/questions/tagged/microsoft-search)
