---
title: Тип ресурса searchRequest
description: Поисковый запрос, который будет отправлен в конечную точку запроса. Содержит тип сущностями, ожидаемыми в ответе, основные источники, параметры подкатки, запрос полей и фактический поисковый запрос.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 3bda8b317e1bc42e21943c23ca8a841572cf8cd0
ms.sourcegitcommit: 1d2adc4062c8e83d23768682cf66a731bccd313c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/16/2021
ms.locfileid: "49883188"
---
# <a name="searchrequest-resource-type"></a>Тип ресурса searchRequest

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [search-api-deprecation](../../includes/search-api-deprecation.md)]

Запрос поиска, отформатированный в BLOB-оке JSON. 

Большой объем JSON содержит типы ресурсов, ожидаемых в ответе, основные источники, параметры разбития на поля, параметры сортировки, запрашиваемую агрегацию и поля, а также фактический поисковый запрос. См. [примеры](#see-also) запросов поиска на различных ресурсах.

> [!NOTE]
> Следует помнить об [известных ограничениях](search-api-overview.md#known-limitations) поиска определенных комбинаций типов сущностей, а также сортировки или агрегации результатов поиска.


## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|:------------|
|aggregations|[коллекция aggregationOption](aggregationOption.md)|Указывает агрегации (также известные как уточнения), которые должны возвращаться вместе с результатами поиска. Необязательное свойство.|
|aggregationFilters|Коллекция String|Содержит один или несколько фильтров для получения результатов поиска, агрегированных и отфильтрованных по определенному значению поля. Необязательное свойство.<br>Создайте этот фильтр на основе предыдущего поиска, агрегированного по одному полю. В ответе предыдущего поиска определите [объект searchBucket,](searchBucket.md) который фильтрует результаты по определенному значению поля, используйте строку в свойстве **aggregationFilterToken** и создайте строку фильтра агрегации в формате **"{field}: \\ "{aggregationFilterToken} \\ ""**. <br>Если необходимо увести несколько значений для одного поля, используйте строки в его свойстве **aggregationFilterToken** и создайте строку фильтра агрегации в формате **"{field}:or( \\ "{aggregationFilterToken1} \\ ", \\ "{aggregationFilterToken2} \\ ")"**. <br>Например, при поиске и агрегации элементов диска по типу файла возвращается **объект searchBucket** для типа файла `docx` в ответе. Вы можете удобно использовать **aggregationFilterToken,** возвращенный для этого **searchBucket,** в последующем поисковом запросе и фильтре совпадений вниз для элементов типа `docx` файла. [В примере 1](/graph/search-concept-aggregation#example-1-request-aggregations-by-string-fields) [и примере 2](/graph/search-concept-aggregation#example-2-apply-an-aggregation-filter-based-on-a-previous-request) показываются фактические запросы и ответы.|
|contentSources|Коллекция String|Содержит подключение, которое необходимо нацелить. <br>Соблюдает следующий формат: `/external/connections/connectionid` `connectionid` где находится ConnectionId, определенный в администрировании соединитеителей. <br> Примечание. contentSource применимо только в том случае, если entityType= `externalItem` . Необязательное свойство.|
|enableTopResults|Логический|Это запускает гибридную сортировку для сообщений: первые 3 сообщения наиболее релевантны. Это свойство применимо только к entityType= `message` . Необязательное свойство.|
|entityTypes|Коллекция entityType| Один или несколько типов ресурсов, ожидаемых в ответе. Возможные значения: `list`, `site`, `listItem`, `message`, `event`, `drive`, `driveItem`, `externalItem`. См. [известные ограничения](search-api-overview.md#known-limitations) для этих комбинаций двух или более типов су субъектов, которые поддерживаются в одном поисковом запросе. Обязательный.|
|fields|Коллекция String |Содержит поля, возвращаемые для каждого объекта ресурса, указанного в **entityTypes,** что позволяет настраивать поля, возвращаемые по умолчанию, в противном случае, включая дополнительные поля, такие как настраиваемые управляемые свойства из SharePoint и OneDrive, или настраиваемые поля в **externalItem** из содержимого, посеяно соединителю Graph. Необязательное свойство.|
|from|Int32|Указывает смещение результатов поиска. Смещение 0 возвращает самый первый результат. Необязательное свойство.|
|Запрос|[searchQuery](searchquery.md)|Содержит термины запроса. Обязательный.|
|size|Int32|Размер извлекаемой страницы. Необязательное свойство.|
|sortProperties|[Коллекция sortProperty](sortProperty.md)|Содержит упорядоченную коллекцию полей и направление сортировки результатов. В коллекции может быть не более 5 свойств сортировки. Необязательное свойство.|
|stored_fields (неподготовлено)|Коллекция String |Теперь это свойство заменяется **свойством fields.** |


## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchRequest",
  "baseType": null
}-->

```json
{
  "entityTypes": ["String"],
  "contentSources": ["String"],
  "query": {"@odata.type": "microsoft.graph.searchQuery"},
  "from": 1024,
  "size": 1024,
  "fields": ["String"],
  "sortProperties": [{"@odata.type": "microsoft.graph.sortProperty"}],
  "aggregations": [{"@odata.type": "microsoft.graph.aggregationOption"}],
  "aggregationFilters": ["String"],
  "enableTopResults": true  
}
```

## <a name="see-also"></a>См. также
- Поиск [в почтовых сообщениях](/graph/search-concept-messages)
- Поиск [событий календаря](/graph/search-concept-events)
- Поиск контента в SharePoint и OneDrive ([файлы, списки и сайты)](/graph/search-concept-files)
- Поиск [пользовательских типов, импортируемых с помощью соединители)](/graph/search-concept-custom-types) данных
- [Сортировка](/graph/search-concept-sort) результатов поиска
- Использование [агрегаций для](/graph/search-concept-aggregations) уточнения результатов поиска


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


