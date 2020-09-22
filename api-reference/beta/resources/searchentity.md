---
title: Тип ресурса Сеарчентити
description: Объект верхнего уровня, представляющий конечную точку API Microsoft Search.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: cb6d5bdd5288a3f6098f33d3432a0e4f0d7ac8bd
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193968"
---
# <a name="searchentity-resource-type"></a>Тип ресурса Сеарчентити

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Объект верхнего уровня, представляющий конечную точку API Microsoft Search. Он не работает как другой ресурс в Graph, но служит привязкой к действию [запроса](../api/search-query.md) . 

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[query](../api/search-query.md) |Коллекция [сеарчреспонсе](searchresponse.md) | Выполняет запрос, указанный в теле запроса.  |

## <a name="properties"></a>Свойства
Нет

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
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


## <a name="next-steps"></a>Дальнейшие действия

Изучите действие [запроса](../api/search-query.md) .


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "A top level object representing the Microsoft Search API endpoint.",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


