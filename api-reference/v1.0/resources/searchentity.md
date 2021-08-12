---
title: Тип ресурса searchEntity
description: Объект верхнего уровня, представляющий конечную Поиск (Майкрософт) API.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 4ef8b062b044ed08112b68c0a61c46f1147db9c751f42c7f500f269d79afea63
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54163750"
---
# <a name="searchentity-resource-type"></a>Тип ресурса searchEntity

Пространство имен: microsoft.graph

Объект верхнего уровня, представляющий конечную Поиск (Майкрософт) API. Он не ведет себя как любой другой ресурс в Graph, но служит якорем для [действия запроса.](../api/search-query.md) 

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[query](../api/search-query.md) |[коллекция searchResponse](searchresponse.md) | Выполняет запрос, указанный в теле запроса.  |

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

Ознакомьтесь [с действием запроса.](../api/search-query.md)


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "A top level object representing the Microsoft Search API endpoint.",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


