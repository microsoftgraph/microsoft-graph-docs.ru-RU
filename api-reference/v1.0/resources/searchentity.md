---
title: Тип ресурса Сеарчентити
description: Объект верхнего уровня, представляющий конечную точку API Microsoft Search.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 4382deb0b23d051eb7b713661c3a61035e5ceafa
ms.sourcegitcommit: 5345c2f3265ede107fa0faaff7a3f1c2afee3810
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378029"
---
# <a name="searchentity-resource-type"></a>Тип ресурса Сеарчентити

Пространство имен: microsoft.graph

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


