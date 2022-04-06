---
title: тип ресурса searchRequest
description: Запрос на поиск, который будет отправлен в конечную точку запроса. Он содержит тип сущностями, ожидаемыми в ответе, основные источники, параметры paging, запрос полей и фактический запрос поиска.
ms.localizationpriority: medium
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: b8c91ce200e052850b0cbfefb7736e5bc3337e10
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589431"
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

| Свойство     | Тип        | Описание             
|:-------------|:------------|:------------
|aggregations|[коллекция aggregationOption](aggregationOption.md)|Указывает агрегации (также известные как переработчики), которые будут возвращены вместе с результатами поиска. Необязательно.|
|aggregationFilters|Коллекция строк|Содержит один или несколько фильтров для получения результатов поиска, агрегированных и отфильтрованных до определенного значения поля. Необязательно.<br>Создайте этот фильтр на основе предварительного поиска, который агрегируется в одном поле. В ответе предварительного поиска определите строку [searchBucket](searchBucket.md) , которая фильтрует результаты до определенного значения поля, используйте строку в свойстве **aggregationFilterToken** и создайте строку фильтра агрегации в формате **"{field}::\\"{aggregationFilterToken}\\"**. <br>Если требуется несколько значений для одного поля, используйте строки в свойстве **aggregationFilterToken** и создайте строку фильтра агрегации в формате **"{field}::or(\\{aggregationFilterToken1}\\",\\"{aggregationFilterToken2}\\")"**. <br>Например, поиск и агрегирование элементов диска по типу файла возвращает **searchBucket** `docx` для типа файла в ответе. Вы можете удобно использовать **aggregationFilterToken** , возвращенный для этого **searchBucket** `docx` в последующем запросе поиска и фильтрации совпадений вниз, чтобы диск элементов типа файла. [В примере 1](/graph/search-concept-aggregation#example-1-request-aggregations-by-string-fields) [и в примере 2 покажите](/graph/search-concept-aggregation#example-2-apply-an-aggregation-filter-based-on-a-previous-request) фактические запросы и ответы.|
|contentSources|Коллекция строк|Содержит адресное подключение. <br>Соблюдает следующий формат: `/external/connections/connectionid` где `connectionid` определяется ConnectionId в администрировании соединители. <br> Примечание: contentSource применим только при entityType=`externalItem`. Необязательно.|
|enableTopResults|Логическое|Это вызывает гибридную сортировку сообщений: первые 3 сообщения являются наиболее актуальными. Это свойство применимо только к entityType=`message`. Необязательно.|
|entityTypes|Коллекция entityType| Один или несколько типов ресурсов, ожидаемых в ответе. Возможные значения: `list`, `site`, `listItem`, `message`, `event`, `drive`, `driveItem`, `person`, `externalItem`. См [. известные ограничения](search-api-overview.md#known-limitations) для этих комбинаций двух или более типов сущности, поддерживаемых в одном запросе поиска. Обязательный аргумент.|
|fields|Коллекция строк |Содержит поля, возвращаемые для каждого объекта ресурса, указанного в **entityTypes**, что позволяет настраивать поля, возвращаемые по умолчанию, в том числе дополнительные поля, такие как настраиваемые управляемые свойства из SharePoint и OneDrive, или настраиваемые поля в **externalItem** из контента, который приносят соединиттели Microsoft Graph. <br>Свойство полей может использовать семантические [метки](/microsoftsearch/configure-connector#step-5-assign-property-labels) , применяемые к свойствам. Например, если свойство помечено как название, его можно получить с помощью следующего синтаксиса : label_title.<br>Необязательно.|
|from|Int32|Указывает смещение результатов поиска. Смещение 0 возвращает самый первый результат. Необязательно.|
|Запрос|[searchQuery](searchquery.md)|Содержит термины запроса. Обязательный аргумент.|
|queryAlterationOptions|[searchAlterationOptions](searchalterationoptions.md)|Предоставляет параметры изменения запросов, отформатированные как BLOB JSON, содержащий два необязательных флага, связанных с исправлением правописания. Необязательно. |
|resultTemplateOptions|[коллекция resultTemplateOption](resultTemplateOption.md)|Предоставляет параметры шаблонов результатов поиска для отрисовки результатов поиска соединители.|
|size|Int32|Размер извлекаемой страницы. Необязательно.|
|sortProperties|[коллекция sortProperty](sortProperty.md)|Содержит упорядоченный набор полей и направлений для сортировки результатов. В коллекции может быть не более 5 свойств сортировки. Необязательно.|
|trimDuplicates|Логический|Указывает, следует ли урезать дубликаты SharePoint из результатов поиска. Значение по умолчанию — `false`. Необязательно.|
|stored_fields (амортизации)|Коллекция строк |Теперь это свойство полей **заменяется** . |

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
  "aggregationFilters": ["String"],
  "aggregations": [{"@odata.type": "microsoft.graph.aggregationOption"}],
  "contentSources": ["String"],
  "enableTopResults": true,
  "entityTypes": ["String"],
  "fields": ["String"],
  "from": 1024,
  "query": {"@odata.type": "microsoft.graph.searchQuery"},
  "queryAlterationOptions": {"@odata.type": "microsoft.graph.searchAlterationOptions"},
  "resultTemplateOptions": [{"@odata.type": "microsoft.graph.resultTemplateOption"}],
  "size": 1024,
  "sortProperties": [{"@odata.type": "microsoft.graph.sortProperty"}],
  "trimDuplicates": false
}
```

## <a name="see-also"></a>См. также
- [Использование шаблонов запросов](/graph/search-concept-query-template)
- [Поиск сообщений почты](/graph/search-concept-messages)
- [Поиск событий календаря](/graph/search-concept-events)
- [Поиск человека](/graph/search-concept-person)
- [Поиск контента в SharePoint и OneDrive](/graph/search-concept-files) (файлы, списки и сайты)
- [Поиск пользовательских типов, импортированных с помощью соединителей](/graph/search-concept-custom-types)
- [Сортировка результатов поиска](/graph/search-concept-sort)
- [Обрезка дублирующих результатов поиска](/graph/search-concept-trim-duplicate) 
- [Использование агрегаций для](/graph/search-concept-aggregation) уточнения результатов поиска
- [Использование макета отображения](/graph/search-concept-display-layout)
- [Включить исправления орфографии](/graph/search-concept-speller) в результатах поиска


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
