---
title: тип ресурса searchRequest
description: Запрос на поиск, который будет отправлен в конечную точку запроса. Он содержит тип сущностями, ожидаемыми в ответе, основные источники, параметры paging, запрос полей и фактический запрос поиска.
ms.localizationpriority: medium
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: d7801fc7ba8d1bcdfcb9fa6da5508fb5d973d3d9
ms.sourcegitcommit: b19b19bf192688f4c513492e8391e4d8dc104633
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/17/2022
ms.locfileid: "62878864"
---
# <a name="searchrequest-resource-type"></a>тип ресурса searchRequest

Пространство имен: microsoft.graph

Запрос поиска, отформатированный в blob JSON. 

BLOB JSON содержит типы ресурсов, ожидаемых в ответе, основные источники, параметры paging, параметры сортировки, запрашиваемая агрегация и поля, а также фактический поисковый запрос. Примеры [запросов](#see-also) на поиск см. на различных ресурсах.

> [!NOTE]
> Будьте в курсе [известных ограничений](search-api-overview.md#known-limitations) на поиск определенных комбинаций типов сущностей, а также сортировку или агрегирование результатов поиска.


## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание| 
|:-------------|:------------|:------------|
|aggregationFilters|Коллекция String|Содержит один или несколько фильтров для получения результатов поиска, агрегированных и отфильтрованных до определенного значения поля. Необязательное свойство.<br>Создайте этот фильтр на основе предварительного поиска, который агрегируется в одном поле. В ответе предварительного поиска определите строку [searchBucket](searchBucket.md) , которая фильтрует результаты до определенного значения поля, используйте строку в свойстве **aggregationFilterToken** и создайте строку фильтра агрегации в формате **"{field}::\\"{aggregationFilterToken}\\"**. <br>Если требуется несколько значений для одного поля, используйте строки в свойстве **aggregationFilterToken** и создайте строку фильтра агрегации в формате **"{field}::or(\\{aggregationFilterToken1}\\",\\"{aggregationFilterToken2}\\")"**. <br>Например, поиск и агрегирование элементов диска по типу файла возвращает **searchBucket** `docx` для типа файла в ответе. Вы можете удобно использовать **aggregationFilterToken** , возвращенный для этого **searchBucket** `docx` в последующем запросе поиска и фильтрации совпадений вниз, чтобы диск элементов типа файла. [В примере 1](/graph/search-concept-aggregation#example-1-request-aggregations-by-string-fields) [и в примере 2 покажите](/graph/search-concept-aggregation#example-2-apply-an-aggregation-filter-based-on-a-previous-request) фактические запросы и ответы.|
|aggregations|[коллекция aggregationOption](aggregationOption.md)|Указывает агрегации (также известные как переработчики), которые будут возвращены вместе с результатами поиска. Необязательное свойство.|
|contentSources|Коллекция объектов string|Содержит адресное подключение.|
|enableTopResults|Логический|Это вызывает гибридную сортировку сообщений: первые 3 сообщения являются наиболее актуальными. Это свойство применимо только к entityType=`message`. Необязательное свойство.|
|entityTypes|Коллекция entityType| Один или несколько типов ресурсов, ожидаемых в ответе. Возможные значения: `list`, `site`, `listItem`, `message`, `event`, `drive`, `driveItem`, `externalItem`. См [. известные ограничения](search-api-overview.md#known-limitations) для этих комбинаций двух или более типов сущности, поддерживаемых в одном запросе поиска. Обязательный элемент.|
|fields|Коллекция объектов string |Содержит поля, возвращаемые для каждого объекта ресурса, указанного в **entityTypes**, что позволяет настраивать поля, возвращаемые по умолчанию; в противном случае, в том числе дополнительные поля, такие как настраиваемые управляемые свойства из SharePoint и OneDrive, или настраиваемые поля **в externalItem** из контента, Graph подключатели Microsoft Graph. Свойство **полей** может использовать [семантические метки](/microsoftsearch/configure-connector#step-6-assign-property-labels) , применяемые к свойствам. Например, если свойство помечено как название, его можно получить с помощью следующего синтаксиса: `label_title`. Необязательное свойство.|
|from|Int32|Указывает смещение результатов поиска. Смещение 0 возвращает самый первый результат. Необязательное свойство.|
|Запрос|[searchQuery](searchquery.md)|Содержит термины запроса. Обязательный элемент.|
|queryAlterationOptions|[searchAlterationOptions](searchalterationoptions.md)|Параметры изменения запроса, отформатированные в BLOB JSON, который содержит два необязательных флага, связанных с исправлением орфографии. Необязательное свойство. |
|resultTemplateOptions|[коллекция resultTemplateOption](resulttemplateoption.md)|Предоставляет параметры шаблона результатов поиска для отображения результатов поиска из соединители.|
|size|Int32|Размер извлекаемой страницы. Необязательное свойство.|
|sortProperties|[коллекция sortProperty](sortProperty.md)|Содержит упорядоченный набор полей и направлений для сортировки результатов. В коллекции может быть не более 5 свойств сортировки. Необязательное свойство.|

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
- Поиск [сообщений почты](/graph/search-concept-messages)
- События [календаря поиска](/graph/search-concept-events)
- Поиск контента в SharePoint и OneDrive ([файлы, списки и сайты](/graph/search-concept-files))
- [Сортировка](/graph/search-concept-sort) результатов поиска
- Использование [агрегаций для](/graph/search-concept-aggregations) уточнения результатов поиска
- Использование [макета отображения](/graph/search-concept-display-layout.md)
- Включить [исправления орфографии](/graph/search-concept-speller) в результатах поиска


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


