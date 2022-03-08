---
title: Тип ресурса searchEntity
description: Объект верхнего уровня, представляющий конечную Поиск (Майкрософт) API.
ms.localizationpriority: medium
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 39f5213e9be29f9fd87332513c3d0b090e3d3e1f
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63335187"
---
# <a name="searchentity-resource-type"></a>Тип ресурса searchEntity

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Объект верхнего уровня, который представляет конечную Поиск (Майкрософт) API.

Он служит якорем для отношений действий [запроса](../api/search-query.md) и ответов на поиск, таких как [](../resources/search-bookmark.md)аббревиатуры[,](../resources/search-acronym.md) закладки и [qnas](../resources/search-qna.md). 

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[query](../api/search-query.md) |[коллекция searchResponse](searchresponse.md) | Запустите указанный поисковый запрос.   |

## <a name="properties"></a>Свойства
Нет

## <a name="relationships"></a>Связи
| Связь | Тип |Описание|
|:---------------|:--------|:----------|
| аббревиатуры | [коллекция microsoft.graph.search.acronym](../resources/search-acronym.md) | Административный ответ в Поиск (Майкрософт), чтобы определить общие аббревиатуры в организации.  |
| закладки | [коллекция microsoft.graph.search.bookmark](../resources/search-bookmark.md) | Административный ответ в Поиск (Майкрософт) результатов для общих поисковых запросов в организации. |
| qnas | [коллекция microsoft.graph.search.qna](../resources/search-qna.md) | Административный ответ в Поиск (Майкрософт) результатов, которые предоставляют ответы на определенные ключевые слова поиска в организации. |


## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.searchEntity",
  "baseType": "microsoft.graph.entity"
}
-->
``` json
{
  
}
```


## <a name="see-also"></a>См. также

[query](../api/search-query.md)


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "A top level object representing the Microsoft Search API endpoint.",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


