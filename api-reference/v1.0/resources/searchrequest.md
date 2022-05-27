---
title: Тип ресурса searchRequest
description: Поисковый запрос, отправляемый в конечную точку запроса. Он содержит тип сущностей, ожидаемых в ответе, базовые источники, параметры разбиения на страницы, запрос полей и фактический поисковый запрос.
ms.localizationpriority: medium
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 0f981aedcea282e2956859412d4d9c7ad8730323
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2022
ms.locfileid: "65694407"
---
# <a name="searchrequest-resource-type"></a>Тип ресурса searchRequest

Пространство имен: microsoft.graph

Поисковый запрос, отформатированный в BLOB-объекте JSON. 

Большой двоичный объект JSON содержит типы ресурсов, ожидаемых в ответе, базовые источники, параметры разбиения на страницы, параметры сортировки, запрашиваемые агрегаты и поля, а также фактический поисковый запрос. См [. примеры поисковых](#see-also) запросов на различных ресурсах.

> [!NOTE]
> Помните об [известных ограничениях](search-api-overview.md#known-limitations) поиска определенных сочетаний типов сущностей, а также сортировки или агрегирования результатов поиска.


## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание| 
|:-------------|:------------|:------------|
|aggregationFilters|Коллекция String|Содержит один или несколько фильтров для получения результатов поиска, агрегированных и отфильтрованных по определенному значению поля. Необязательно.<br>Создайте этот фильтр на основе предыдущего поиска, который агрегирует по одному полю. В ответе предыдущего поиска определите [searchBucket](searchBucket.md), который фильтрует результаты по определенному значению поля, используйте строку в свойстве **aggregationFilterToken** и создайте строку фильтра агрегирования в формате **"{field}:\\"{aggregationFilterToken}\\".** <br>Если необходимо указать несколько значений для одного поля, используйте строки в свойстве **aggregationFilterToken** и создайте строку фильтра агрегирования в формате **"{field}:or(\\"{aggregationFilterToken1}\\",\\"{aggregationFilterToken2}\\")"**. <br>Например, поиск и агрегирование элементов диска по типу файла возвращает **searchBucket** `docx` для типа файла в ответе. Вы можете удобно использовать **aggregationFilterToken**, возвращенный для этого **searchBucket**`docx`, в последующем поисковом запросе и фильтре совпадений вниз для элементов типа файла. [В примере 1](/graph/search-concept-aggregation#example-1-request-aggregations-by-string-fields) [и примере 2](/graph/search-concept-aggregation#example-2-apply-an-aggregation-filter-based-on-a-previous-request) показаны фактические запросы и ответы.|
|aggregations|[Коллекция aggregationOption](aggregationOption.md)|Указывает агрегаты (также называемые уточнением), которые должны возвращаться вместе с результатами поиска. Необязательно.|
|contentSources|Коллекция строк|Содержит целевое подключение.|
|enableTopResults|Логический|Это активирует гибридную сортировку сообщений: первые 3 сообщения являются наиболее актуальными. Это свойство применимо только к entityType=`message`. Необязательно.|
|entityTypes|Коллекция entityType| Один или несколько типов ресурсов, ожидаемых в ответе. Возможные значения: `list`, `site`, `listItem`, `message`, `event`, `drive`, `driveItem`, `externalItem`. [Ознакомьтесь с известными ограничениями](search-api-overview.md#known-limitations) для этих сочетаний двух или более типов сущностей, которые поддерживаются в одном и том же поисковом запросе. Обязательный аргумент.|
|fields|Коллекция String |Содержит поля, возвращаемые для каждого объекта ресурса, указанного в **entityTypes**, что позволяет настраивать поля, возвращаемые по умолчанию; в противном случае, включая дополнительные поля, такие как настраиваемые управляемые свойства из SharePoint и OneDrive, или настраиваемые поля **в externalItem** из содержимого, которое Graph соединители Microsoft Graph. Свойство **fields** может использовать [семантические метки](/microsoftsearch/configure-connector#step-6-assign-property-labels) , примененные к свойствам. Например, если свойство помечено как заголовок, его можно получить с помощью следующего синтаксиса: `label_title`. Необязательно.|
|from|Int32|Задает смещение для результатов поиска. Смещение 0 возвращает первый результат. Необязательно.|
|Запрос|[searchQuery](searchquery.md)|Содержит условия запроса. Обязательный аргумент.|
|queryAlterationOptions|[searchAlterationOptions](searchalterationoptions.md)|Параметры изменения запроса, отформатированные в BLOB-объекте JSON, который содержит два необязательных флага, связанных с исправлением орфографии. Необязательно. |
|resultTemplateOptions|[Коллекция resultTemplateOption](resulttemplateoption.md)|Предоставляет параметры шаблона результатов поиска для отображения результатов поиска из соединителей.|
|size|Int32|Размер извлекаемой страницы. Максимальное значение — 1000. Необязательно.|
|sortProperties|[Коллекция sortProperty](sortProperty.md)|Содержит упорядоченную коллекцию полей и направление сортировки результатов. В коллекции может быть не более 5 свойств сортировки. Необязательно.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

```json
{
  "aggregationFilters": ["String"],
  "aggregations": {"@odata.type": "microsoft.graph.aggregationOption"},
  "enableTopResults": "Boolean",
  "entityTypes": ["String"],
  "contentSources": ["String"],
  "fields": ["String"],
  "from": "Int32",
  "query": {"@odata.type": "microsoft.graph.searchQuery"},
  "queryAlterationOptions": {"@odata.type": "microsoft.graph.searchAlterationOptions"},
  "resultTemplateOptions": [{"@odata.type": "microsoft.graph.resultTemplateOption"}],
  "size": "Int32"
}
```

## <a name="see-also"></a>См. также
- Поиск [почтовых сообщений](/graph/search-concept-messages)
- Поиск [событий календаря](/graph/search-concept-events)
- Поиск контента в SharePoint и OneDrive ([файлы, списки и сайты](/graph/search-concept-files))
- [Сортировка](/graph/search-concept-sort) результатов поиска
- Использование [агрегатов для уточнения](/graph/search-concept-aggregations) результатов поиска
- Использование [макета дисплея](/graph/search-concept-display-layout.md)
- Включение [исправлений орфографии](/graph/search-concept-speller) в результатах поиска


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


