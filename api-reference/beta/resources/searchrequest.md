---
title: тип ресурса searchRequest
description: Запрос на поиск, который будет отправлен в конечную точку запроса. Он содержит тип сущностями, ожидаемыми в ответе, основные источники, параметры paging, запрос полей и фактический запрос поиска.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 6e660db18986498ce639a1db14a284a878d57a1f
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054247"
---
# <a name="searchrequest-resource-type"></a>тип ресурса searchRequest

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [search-api-deprecation](../../includes/search-api-deprecation.md)]

Запрос поиска, отформатированный в blob JSON. 

BLOB JSON содержит типы ресурсов, ожидаемых в ответе, основные источники, параметры paging, параметры сортировки, запрашиваемая агрегация и поля, а также фактический поисковый запрос. Примеры [запросов](#see-also) на поиск см. на различных ресурсах.

> [!NOTE]
> Будьте в курсе [известных ограничений](search-api-overview.md#known-limitations) на поиск определенных комбинаций типов сущностей, а также сортировку или агрегирование результатов поиска.


## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|:------------|
|aggregations|[коллекция aggregationOption](aggregationOption.md)|Указывает агрегации (также известные как переработчики), которые будут возвращены вместе с результатами поиска. Необязательное.|
|aggregationFilters|Коллекция объектов string|Содержит один или несколько фильтров для получения результатов поиска, агрегированных и отфильтрованных до определенного значения поля. Необязательное.<br>Создайте этот фильтр на основе предварительного поиска, который агрегируется в одном поле. В ответе предварительного поиска определите строку [searchBucket,](searchBucket.md) которая фильтрует результаты до определенного значения поля, используйте строку в свойстве **aggregationFilterToken** и создайте строку фильтра агрегации в формате **"{field}: \\ "{aggregationFilterToken} \\ ""**. <br>Если необходимо предоставлять несколько значений для одного поля, используйте строки в свойстве **aggregationFilterToken** и создайте строку фильтра агрегации в формате **"{field}:or" \\ ({aggregationFilterToken1} \\ ", \\ "{aggregationFilterToken2} \\ ") ".** <br>Например, поиск и агрегирование элементов диска по типу файла возвращает **searchBucket** для типа файла `docx` в ответе. Вы можете удобно использовать **aggregationFilterToken,** возвращенный для этого **searchBucket** в последующем запросе поиска и фильтрации совпадений вниз, чтобы диск элементов `docx` типа файла. [В примере 1](/graph/search-concept-aggregation#example-1-request-aggregations-by-string-fields) [и в примере 2 покажите](/graph/search-concept-aggregation#example-2-apply-an-aggregation-filter-based-on-a-previous-request) фактические запросы и ответы.|
|contentSources|Коллекция объектов string|Содержит адресное подключение. <br>Соблюдает следующий формат: `/external/connections/connectionid` где `connectionid` определяется ConnectionId в администрировании соединители. <br> Примечание: contentSource применим только в том случае, если entityType= `externalItem` . Необязательное.|
|enableTopResults|Логический|Это вызывает гибридную сортировку сообщений: первые 3 сообщения являются наиболее актуальными. Это свойство применимо только к entityType= `message` . Необязательное.|
|entityTypes|Коллекция entityType| Один или несколько типов ресурсов, ожидаемых в ответе. Возможные значения: `list`, `site`, `listItem`, `message`, `event`, `drive`, `driveItem`, `externalItem`. См. [известные ограничения](search-api-overview.md#known-limitations) для этих комбинаций двух или более типов сущности, поддерживаемых в одном запросе поиска. Обязательный.|
|fields|Коллекция объектов string |Содержит поля, возвращаемые для каждого объекта ресурса, указанного в **entityTypes,** что позволяет настраивать поля, возвращаемые по умолчанию, в том числе дополнительные поля, такие как настраиваемые управляемые свойства из SharePoint и OneDrive, или настраиваемые поля в **externalItem** из контента, который приносят соединиттели Microsoft Graph. <br>Свойство полей может использовать семантические [метки,](https://docs.microsoft.com/microsoftsearch/configure-connector#step-5-assign-property-labels) применяемые к свойствам. Например, если свойство помечено как название, его можно получить с помощью следующего синтаксиса : label_title.<br>Необязательное.|
|from|Int32|Указывает смещение результатов поиска. Смещение 0 возвращает самый первый результат. Необязательное.|
|Запрос|[searchQuery](searchquery.md)|Содержит термины запроса. Обязательный.|
|size|Int32|Размер извлекаемой страницы. Необязательное.|
|sortProperties|[коллекция sortProperty](sortProperty.md)|Содержит упорядоченный набор полей и направлений для сортировки результатов. В коллекции может быть не более 5 свойств сортировки. Необязательное.|
|stored_fields (обесценилось)|Коллекция объектов string |Теперь это свойство полей **заменяется.** |


## <a name="json-representation"></a>Представление в формате JSON

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
- Поиск [сообщений почты](/graph/search-concept-messages)
- События [календаря поиска](/graph/search-concept-events)
- Поиск контента в SharePoint и OneDrive[(файлы, списки и сайты)](/graph/search-concept-files)
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


