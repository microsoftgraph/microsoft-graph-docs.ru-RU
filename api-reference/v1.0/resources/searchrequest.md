---
title: Тип ресурса Сеарчрекуест
description: Запрос поиска, отправляемый конечной точке запроса. Он содержит тип сущностей, ожидаемых в ответе, базовые источники, параметры разбиения по страницам, запрос полей и фактический поисковый запрос.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: f673c551ce27c16fd4fddabc26e55cd234a9f19e
ms.sourcegitcommit: 5345c2f3265ede107fa0faaff7a3f1c2afee3810
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378023"
---
# <a name="searchrequest-resource-type"></a>Тип ресурса Сеарчрекуест

Пространство имен: microsoft.graph

Запрос поиска, отформатированный в большом двоичном объекте JSON. 

Большой двоичный объект JSON содержит типы ресурсов, ожидаемых в ответе, базовые источники, параметры разбиения по страницам, параметры сортировки, запрошенные агрегаты и поля, а также фактический поисковый запрос. В этой статье приведены [примеры](#see-also) запросов на поиск в различных ресурсах.

> [!NOTE]
> Помните об [известных ограничениях](search-api-overview.md#known-limitations) на поиск определенных комбинаций типов сущностей, сортировку или статистическую обработку результатов поиска.


## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|:------------|
|contentSources|Коллекция String|Содержит подключение, которое необходимо задать.|
|enableTopResults|Boolean|Это запускает гибридную сортировку для сообщений: первые 3 сообщения наиболее актуальны. Это свойство применяется только к entityType = `message` . Необязательный параметр.|
|entityTypes|Коллекция entityType| Один или несколько типов ресурсов, ожидаемых в отклике. Возможные значения: `list`, `site`, `listItem`, `message`, `event`, `drive`, `driveItem`. Ознакомьтесь с [известными ограничениями](search-api-overview.md#known-limitations) для этих комбинаций двух или более типов сущностей, которые поддерживаются в одном поисковом запросе. Обязательный.|
|fields|Коллекция String |Содержит поля, возвращаемые для каждого объекта ресурса, указанного в **EntityType**, что позволяет настраивать поля, возвращаемые по умолчанию, в том числе дополнительные поля, такие как настраиваемые управляемые свойства, из SharePoint и OneDrive. Необязательный параметр.|
|from|Int32|Задает смещение результатов поиска. Смещение 0 возвращает самый первый результат. Необязательный параметр.|
|Запрос|[searchQuery](searchquery.md)|Содержит термины запроса. Обязательный.|
|size|Int32|Размер извлекаемой страницы. Необязательный параметр.|

## <a name="json-representation"></a>Представление в формате JSON

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
- Поиск в [сообщениях электронной почты](/graph/search-concept-messages)
- Поиск [событий календаря](/graph/search-concept-events)
- Поиск контента в SharePoint и OneDrive ([файлы, списки и сайты](/graph/search-concept-files))



<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


