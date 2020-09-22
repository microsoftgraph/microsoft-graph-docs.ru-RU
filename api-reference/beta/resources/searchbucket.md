---
title: Тип ресурса Сеарчбуккет
description: Предоставляет определенную статистическую функцию в отклике, значение определенного сегмента.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 3fe375ca2e9695a237b60e30cdd9e98a9e545d35
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193960"
---
# <a name="searchbucket-resource-type"></a>Тип ресурса Сеарчбуккет

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет контейнер для одного или нескольких результатов поиска, которые имеют одно и то же значение для поля сущности, в котором они объединены. 



## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|key|String| Дискретное значение поля, для которого рассчитано агрегирование.|
|count|Int32| Количество совпадений поиска, имеющих одно и то же значение, указанное в свойстве **Key** . |
|аггрегатионфилтертокен|String| Маркер, содержащий закодированный фильтр для объединения результатов поиска по определенному значению **ключа** . Чтобы использовать фильтр, передайте маркер в качестве части свойства **аггрегатионфилтер** объекта **сеарчрекуест** в формате **"{Field}: \\ " {аггрегатионфилтертокен} \\ ""**. См. [пример](/graph/search-concept-aggregation#example-2-apply-an-aggregation-filter-based-on-a-previous-request).|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchBucket",
  "baseType": null
}-->

```json
{
  "key": "String",
  "count": "10",  
  "aggregationFilterToken": "String"
}
```
