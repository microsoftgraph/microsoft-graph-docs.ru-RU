---
title: тип ресурса searchRequest
description: Запрос на поиск, который будет отправлен в конечную точку запроса. Он содержит тип сущностями, ожидаемыми в ответе, основные источники, параметры paging, запрос полей и фактический запрос поиска.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 4a797126a1dc6bc5fbecc9aad050711b499945ff
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53207989"
---
# <a name="searchrequest-resource-type"></a>тип ресурса searchRequest

Пространство имен: microsoft.graph

Запрос поиска, отформатированный в blob JSON. 

BLOB JSON содержит типы ресурсов, ожидаемых в ответе, основные источники, параметры paging, параметры сортировки, запрашиваемая агрегация и поля, а также фактический поисковый запрос. Примеры [запросов](#see-also) на поиск см. на различных ресурсах.

> [!NOTE]
> Будьте в курсе [известных ограничений](search-api-overview.md#known-limitations) на поиск определенных комбинаций типов сущностей, а также сортировку или агрегирование результатов поиска.


## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |             |
|:-------------|:------------|:------------|:------------|
|contentSources|Коллекция строк|Содержит адресное подключение.|
|enableTopResults|Логический|Это вызывает гибридную сортировку сообщений: первые 3 сообщения являются наиболее актуальными. Это свойство применимо только к entityType= `message` . Необязательно.|
|entityTypes|Коллекция entityType| Один или несколько типов ресурсов, ожидаемых в ответе. Возможные значения: `list`, `site`, `listItem`, `message`, `event`, `drive`, `driveItem`, `externalItem`. См. [известные ограничения](search-api-overview.md#known-limitations) для этих комбинаций двух или более типов сущности, поддерживаемых в одном запросе поиска. Обязательно.|
|fields|Коллекция строк |Содержит поля, возвращаемые для каждого объекта ресурса, указанного в **entityTypes,** что позволяет настраивать поля, возвращаемые по умолчанию, в том числе дополнительные поля, такие как настраиваемые управляемые свойства из SharePoint и OneDrive. Необязательно.|
|from|Int32|Указывает смещение результатов поиска. Смещение 0 возвращает самый первый результат. Необязательно.|
|Запрос|[searchQuery](searchquery.md)|Содержит термины запроса. Обязательно.|
|size|Int32|Размер извлекаемой страницы. Необязательно.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

```json
{
  "entityTypes": ["String"],
  "contentSources": ["String"],
  "query": {"@odata.type": "microsoft.graph.searchQuery"},
  "from": 1024,
  "size": 1024,
  "fields": ["String"],
  "enableTopResults": true  
}
```

## <a name="see-also"></a>См. также
- Поиск [сообщений почты](/graph/search-concept-messages)
- События [календаря поиска](/graph/search-concept-events)
- Поиск контента в SharePoint и OneDrive[(файлы, списки и сайты)](/graph/search-concept-files)



<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


