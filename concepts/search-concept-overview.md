---
title: Обзор API Поиска (Майкрософт) в Microsoft Graph
description: Используйте API Поиска (Майкрософт) для индексирования контента и добавления в приложения функций поиска в Office и индексированном контенте.
localization_priority: Priority
ms.prod: search
author: snlraju-msft
scenarios: getting-started
ms.openlocfilehash: 2d354a26d2d756ceddac9da0f00a271c595f9fdb
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472799"
---
# <a name="overview-of-the-microsoft-search-api-in-microsoft-graph"></a>Обзор API Поиска (Майкрософт) в Microsoft Graph

Поиск (Майкрософт) — это корпоративная поисковая система, обеспечивающая повышение производительности и релевантные результаты поиска для организации. Она использует наработки и возможности организации и отображает актуальный релевантный контент для пользователей. Поиск (Майкрософт) доступен в различных программах, включая Office, SharePoint, Delve, Windows и Bing. Вы можете использовать API Поиска (Майкрософт) в Microsoft Graph, чтобы Поиск (Майкрософт) распространялся и на ваши приложения.  

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

<!-- markdownlint-disable MD026 -->
## <a name="why-use-the-microsoft-search-api"></a>Зачем использовать API Поиска (Майкрософт)?

### <a name="one-unified-search-endpoint-for-microsoft-cloud-data"></a>Единая конечная точка поиска для данных Microsoft Cloud

API Поиска (Майкрософт) предоставляет единую конечную точку поиска, которую можно использовать для [запроса](/graph/api/search-query) в Microsoft Cloud данных (сообщений и событий в почтовых ящиках Outlook, а также файлов в OneDrive и SharePoint), индексированных в Поиске (Майкрософт).

### <a name="include-custom-external-data-in-search-experience-preview"></a>Включение настраиваемых внешних данных в интерфейс поиска (предварительная версия)

Используйте [соединители Microsoft Graph](/microsoftsearch/connectors-overview), чтобы включить данные из-за пределов облака Майкрософт в свой интерфейс поиска. Например, подключитесь к базе данных отдела кадров организации или к каталогу продуктов. Затем используйте API Поиска (Майкрософт), чтобы легко [запросить](/graph/api/search-query) внешний источник данных. 

Просмотрите [коллекцию соединителей Microsoft Graph](/microsoftsearch/connectors-gallery), чтобы найти готовые к использованию соединители. Вы также можете [создавать собственные соединители](/graph/api/resources/indexing-api-overview?view=graph-rest-beta&preserve-view=true#common-use-cases), чтобы индексировать внешние настраиваемые элементы и отправлять запросы к определенным внешним источникам данных.

### <a name="consistent-up-to-date-search-experience"></a>Единый актуальный интерфейс поиска

При использовании API Поиска (Майкрософт) пользователи получают персонализированные релевантные результаты благодаря Microsoft Graph. Поиск в ваших приложениях вернет результаты, согласованные с поиском в приложениях Office.

## <a name="what-data-can-i-add-or-access-by-using-the-microsoft-search-api"></a>Какие данные можно добавить и к каким получить доступ с помощью API Поиска (Майкрософт)?

API Поиска (Майкрософт) поддерживает поиск следующего контента в Microsoft Cloud:

- Объекты [сообщений](/graph/api/resources/message) электронной почты и [события](/graph/api/resources/event) календаря Outlook
- Файлы и папки в SharePoint и OneDrive ([driveItem](/graph/api/resources/driveitem)), [списки](/graph/api/resources/list), [listItem](/graph/api/resources/listitem) [сайты](/graph/api/resources/site) и [диски.](/graph/api/resources/drive)
- Содержимое, отправляемое через платформу Graph Connectors: [externalItems](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true) (предварительная версия)

## <a name="api-reference"></a>Справочные материалы по API

Ищете справочные материалы по API для этой службы?

- [Использование API Поиска (Майкрософт) для запроса данных](/graph/api/resources/search-api-overview?view=graph-rest-1.0)(версия 1.0)
- [Использование API Поиска (Майкрософт) для запроса данных](/graph/api/resources/search-api-overview?view=graph-rest-beta)(предварительная версия)
- [Использование API Поиска (Майкрософт) для индексирования данных](/graph/api/resources/indexing-api-overview) (предварительная версия)

## <a name="next-steps"></a>Дальнейшие действия

- Подробнее о [Поиске (Майкрософт)](/microsoftsearch/).
- Подробнее о некоторых основных вариантах использования:
  - [Управление подключениями для индексирования внешнего контента](search-index-manage-connections.md)
  - [Индексирование внешнего контента](search-index-manage-items.md)
  - [Поиск сообщений Outlook](search-concept-messages.md)
  - [Поиск событий календаря](search-concept-events.md)
  - [Поиск содержимого в OneDrive и SharePoint](search-concept-files.md)
  - [Поиск внешнего контента](search-concept-custom-types.md) (предварительная версия)
  - [Сортировка результатов поиска](search-concept-sort.md) (предварительная версия)
  - [Уточнение результатов поиска](search-concept-aggregation.md) (предварительная версия)
  
- Узнайте больше об API в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer).
- Скачайте [образец соединителя поиска](https://github.com/microsoftgraph/msgraph-search-connector-sample) в GitHub.

## <a name="see-also"></a>См. также

- Участвуйте в работе сообщества на сайте [Вопросы и ответы Майкрософт](https://aka.ms/askgraph) или на GitHub.
