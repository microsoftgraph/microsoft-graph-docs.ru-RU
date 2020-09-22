---
title: Тип ресурса Сеарчрекуест
description: Запрос поиска, отправляемый конечной точке запроса. Он содержит тип сущностей, ожидаемых в ответе, базовые источники, параметры разбиения по страницам, запрос полей и фактический поисковый запрос.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: a504edc53962b6ab2d6f62e39e23542588252566
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193262"
---
# <a name="searchrequest-resource-type"></a>Тип ресурса Сеарчрекуест

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [search-api-deprecation](../../includes/search-api-deprecation.md)]

Запрос поиска, отформатированный в большом двоичном объекте JSON. 

Большой двоичный объект JSON содержит типы ресурсов, ожидаемых в ответе, базовые источники, параметры разбиения по страницам, параметры сортировки, запрошенные агрегаты и поля, а также фактический поисковый запрос. В этой статье приведены [примеры](#see-also) запросов на поиск в различных ресурсах.

> [!NOTE]
> Помните об [известных ограничениях](search-api-overview.md#known-limitations) на поиск определенных комбинаций типов сущностей, сортировку или статистическую обработку результатов поиска.


## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|:------------|
|Aggregations|Коллекция [аггрегатионоптион](aggregationOption.md)|Задает агрегаты (также известные как уточнения), которые будут возвращены вместе с результатами поиска. Необязательно.|
|аггрегатионфилтерс|Коллекция String|Содержит один или несколько фильтров для получения результатов поиска, сгруппированных и отфильтрованных по определенному значению поля. Необязательно.<br>Постройте этот фильтр на основе предыдущего поиска, который объединяется по одному полю. В ответе предыдущего поиска Определите [сеарчбуккет](searchBucket.md) , который фильтрует результаты по определенному значению поля, используйте строку в свойстве **аггрегатионфилтертокен** и создайте строку фильтра статистической обработки в формате **"{Field}: \\ " {аггрегатионфилтертокен} \\ ""**. <br>Например, при поиске и статистической обработке элементов диска по типу файла возвращается объект **сеарчбуккет** для типа файла `docx` в ответе. Вы можете удобно использовать **аггрегатионфилтертокен** , возвращенный для этого **сеарчбуккет** в последующих запросах поиска, и фильтр соответствует элементам `docx` типа файла. В [примере 1](/graph/search-concept-aggregation#example-1-request-aggregations-by-string-fields) и [2](/graph/search-concept-aggregation#example-2-apply-an-aggregation-filter-based-on-a-previous-request) показаны фактические запросы и ответы.|
|contentSources|Коллекция String|Содержит подключение, которое необходимо задать. <br>Соблюдается следующий формат: `/external/connections/connectionid` где `connectionid` — это коннектионид, определенные в администрировании соединителей. <br> Note: contentSource применяется, только если entityType = `externalItem` . Необязательно.|
|enableTopResults|Логическое|Это запускает гибридную сортировку для сообщений: первые 3 сообщения наиболее актуальны. Это свойство применяется только к entityType = `message` . Необязательно.|
|entityTypes|Коллекция entityType| Один или несколько типов ресурсов, ожидаемых в отклике. Возможные значения: `list`, `site`, `listItem`, `message`, `event`, `drive`, `driveItem`, `externalItem`. Ознакомьтесь с [известными ограничениями](search-api-overview.md#known-limitations) для этих комбинаций двух или более типов сущностей, которые поддерживаются в одном поисковом запросе. Обязательно.|
|fields|Коллекция String |Содержит поля, возвращаемые для объекта ресурса еарч, указанного в **EntityType**, что позволяет настраивать поля, возвращаемые по умолчанию, в том числе дополнительные поля, такие как настраиваемые управляемые свойства из SharePoint и OneDrive, или настраиваемые поля в **екстерналитем** из контента, полученного с помощью графических соединителей. Необязательно.|
|from|Int32|Задает смещение результатов поиска. Смещение 0 возвращает самый первый результат. Необязательно.|
|Запрос|[searchQuery](searchquery.md)|Содержит термины запроса. Обязательно.|
|size|Int32|Размер извлекаемой страницы. Необязательно.|
|сортпропертиес|Коллекция [сортпроперти](sortProperty.md)|Содержит упорядоченную коллекцию полей и направление для сортировки результатов. В коллекции может быть не более 5 свойств сортировки. Необязательно.|
|stored_fields (устаревшее)|Коллекция String |Теперь оно заменяется свойством **Fields** . |


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
- Поиск в [сообщениях электронной почты](/graph/search-concept-messages)
- Поиск [событий календаря](/graph/search-concept-events)
- Поиск контента в SharePoint и OneDrive ([файлы, списки и сайты](/graph/search-concept-files))
- Данные о [настраиваемых типах поиска (соединители Graph)](/graph/search-concept-custom-types)
- [Сортировка](/graph/search-concept-sort) результатов поиска
- Использование [агрегатов](/graph/search-concept-aggregations) для уточнения результатов поиска


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


