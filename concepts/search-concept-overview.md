---
title: Обзор API Поиска (Майкрософт) в Microsoft Graph
description: Используйте API Поиска (Майкрософт) для индексирования контента и добавления в приложения функций поиска в Office и индексированном контенте.
ms.localizationpriority: high
ms.prod: search
author: snlraju-msft
scenarios: getting-started
ms.openlocfilehash: b936bc0dd26ae3287f0a186d3309cc972a184da4
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59129707"
---
# <a name="overview-of-the-microsoft-search-api-in-microsoft-graph"></a>Обзор API Поиска (Майкрософт) в Microsoft Graph

Поиск (Майкрософт) — это корпоративная поисковая система, обеспечивающая повышение производительности и релевантные результаты поиска для организации. Она использует наработки и возможности организации и отображает актуальный релевантный контент для пользователей. Поиск (Майкрософт) доступен в различных программах, включая Office, SharePoint, Delve, Windows и Bing. Вы можете использовать API Поиска (Майкрософт) в Microsoft Graph, чтобы Поиск (Майкрософт) распространялся и на ваши приложения.  

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

- Ресурсы [message](/graph/api/resources/message) почты Outlook и [event](/graph/api/resources/event) календаря.
- Файлы и папки в SharePoint и OneDrive (ресурсы [driveItem](/graph/api/resources/driveitem)), ресурсы [list](/graph/api/resources/list), [listItem](/graph/api/resources/listitem), [site](/graph/api/resources/site) и [drive](/graph/api/resources/drive).
- Ресурсы [person](/graph/api/resources/person) в организации, наиболее релевантные для пользователя.
- Содержимое, отправляемое через платформу соединителей Microsoft Graph: ресурсы [externalItems](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true).

## <a name="api-reference"></a>Справочные материалы по API

Ищете справочные материалы по API для этой службы?

- [Использование API Поиска (Майкрософт) для запроса данных](/graph/api/resources/search-api-overview?view=graph-rest-1.0&preserve-view=true)(версия 1.0)
- [Использование API Поиска (Майкрософт) для запроса данных](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true)(предварительная версия)
- [Использование API Поиска (Майкрософт) для индексирования данных](/graph/api/resources/indexing-api-overview) (предварительная версия)

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
  - [Сортировка результатов поиска](search-concept-sort.md) (предварительная версия)
  - [Уточнение результатов поиска](search-concept-aggregation.md) (предварительная версия)
  - [Исправление орфографии в запросе](search-concept-speller.md) (предварительная версия)
  - [Макет отображения при поиске](search-concept-display-layout.md) (предварительная версия)
 
  
- Узнайте больше об API в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer).
- Скачайте [образец соединителя поиска](https://github.com/microsoftgraph/msgraph-search-connector-sample) в GitHub.

## <a name="see-also"></a>См. также

- Участвуйте в работе сообщества на сайте [Вопросы и ответы Майкрософт](/answers/products/m365#microsoft-graph) или на GitHub.
