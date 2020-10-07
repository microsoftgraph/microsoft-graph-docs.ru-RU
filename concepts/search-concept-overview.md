---
title: Обзор API Поиска (Майкрософт) в Microsoft Graph (предварительная версия)
description: Используйте API Поиска (Майкрософт) для индексирования контента и добавления в приложения функций поиска в Office и индексированном контенте.
localization_priority: Priority
ms.prod: search
author: snlraju-msft
scenarios: getting-started
ms.openlocfilehash: d4c16bd0175f8ae0cd9d8e03f549bea9eff3db63
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/07/2020
ms.locfileid: "48373505"
---
# <a name="overview-of-the-microsoft-search-api-in-microsoft-graph-preview"></a>Обзор API Поиска (Майкрософт) в Microsoft Graph (предварительная версия)

Поиск (Майкрософт) — это корпоративная поисковая система, обеспечивающая повышение производительности и релевантные результаты поиска для организации. Она использует наработки и возможности организации и отображает актуальный релевантный контент для пользователей. Поиск (Майкрософт) доступен в различных программах, включая Office, SharePoint, Delve, Windows и Bing. Вы можете использовать API Поиска (Майкрософт) в Microsoft Graph, чтобы Поиск (Майкрософт) распространялся и на ваши приложения.  

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

<!-- markdownlint-disable MD026 -->
## <a name="why-use-the-microsoft-search-api"></a>Зачем использовать API Поиска (Майкрософт)?

### <a name="one-unified-search-endpoint-for-microsoft-cloud-data"></a>Единая конечная точка поиска для данных Microsoft Cloud

API Поиска (Майкрософт) предоставляет единую конечную точку поиска, которую можно использовать для [запроса](/graph/api/search-query?view=graph-rest-beta&preserve-view=true) в Microsoft Cloud данных (сообщений и событий в почтовых ящиках Outlook, а также файлов в OneDrive и SharePoint), индексированных в Поиске (Майкрософт).

### <a name="include-custom-external-data-in-search-experience"></a>Включение настраиваемых внешних данных в интерфейс поиска

Пользователи, желающие включить в свой поиск данные, не входящие в Microsoft Cloud, могут использовать [соединители](/microsoftsearch/connectors-overview), чтобы подключиться к определенному источнику данных, такому как база данных отдела кадров организации или каталог продуктов, и использовать API Поиска (Майкрософт) для [запроса](/graph/api/search-query?view=graph-rest-beta&preserve-view=true) внешнего источника данных. [Коллекция соединителей Microsoft Graph](/microsoftsearch/connectors-gallery) включает ряд готовых к использованию соединителей. Пользователи также могут [создавать соединители](/graph/api/resources/indexing-api-overview?view=graph-rest-beta&preserve-view=true#common-use-cases), индексировать внешние настраиваемые элементы и запрашивать определенные внешние источники данных.

### <a name="consistent-up-to-date-search-experience"></a>Единый актуальный интерфейс поиска

При использовании API Поиска (Майкрософт) пользователи получают персонализированные релевантные результаты благодаря Microsoft Graph. Поиск в ваших приложениях вернет результаты, согласованные с поиском в приложениях Office.

## <a name="what-data-can-i-add-or-access-by-using-the-microsoft-search-api"></a>Какие данные можно добавить и к каким получить доступ с помощью API Поиска (Майкрософт)?

API Поиска (Майкрософт) поддерживает поиск следующего контента в Microsoft Cloud:

- Объекты [сообщений](/graph/api/resources/message?view=graph-rest-beta&preserve-view=true) электронной почты и [события](/graph/api/resources/event?view=graph-rest-beta&preserve-view=true) календаря Outlook
- Файлы и папки в SharePoint и OneDrive ([driveItem](/graph/api/resources/driveitem?view=graph-rest-beta&preserve-view=true)), [списки](/graph/api/resources/list?view=graph-rest-beta&preserve-view=true), [listItem](/graph/api/resources/listitem?view=graph-rest-beta&preserve-view=true) [сайты](/graph/api/resources/site?view=graph-rest-beta&preserve-view=true) и [диски.](/graph/api/resources/drive?view=graph-rest-beta&preserve-view=true)
- Содержимое, отправляемое через платформу Graph Connectors: [externalItems](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true)

## <a name="api-reference"></a>Справочные материалы по API

Ищете справочные материалы по API для этой службы?

- [Использование API Поиска (Майкрософт) для запроса данных](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true)
- [Использование API Поиска (Майкрософт) для индексирования данных](/graph/api/resources/indexing-api-overview?view=graph-rest-beta&preserve-view=true)

## <a name="next-steps"></a>Дальнейшие действия

- Подробнее о [Поиске (Майкрософт)](/microsoftsearch/).
- Подробнее о некоторых основных вариантах использования:
  - [Управление подключениями для индексирования внешнего контента](search-index-manage-connections.md)
  - [Индексирование внешнего контента](search-index-manage-items.md)
  - [Поиск сообщений Outlook](search-concept-messages.md)
  - [Поиск событий календаря](search-concept-events.md)
  - [Поиск содержимого в OneDrive и SharePoint](search-concept-files.md)
  - [Поиск внешнего контента](search-concept-custom-types.md)
  - [Сортировка результатов поиска](search-concept-sort.md)
  - [Уточнение результатов поиска](search-concept-aggregation.md)
  
- Узнайте больше об API в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer).
- Скачайте [образец соединителя поиска](https://github.com/microsoftgraph/msgraph-search-connector-sample) в GitHub.

## <a name="see-also"></a>См. также

- Участвуйте в работе сообщества на [Stack Overflow](https://stackoverflow.com/questions/tagged/microsoft-graph-search) или на GitHub.
