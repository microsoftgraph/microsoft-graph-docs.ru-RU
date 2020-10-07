---
title: Тип ресурса Сеарчбуккет
description: Предоставляет определенную статистическую функцию в отклике, значение определенного сегмента.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: a6b26c01133f519b0308ffee430d85c9df6d868b
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/07/2020
ms.locfileid: "48373855"
---
# <a name="searchbucket-resource-type"></a>Тип ресурса Сеарчбуккет

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет контейнер для одного или нескольких результатов поиска, которые имеют одно и то же значение для поля сущности, в котором они объединены. 

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|key|String| Дискретное значение поля, для которого рассчитано агрегирование.|
|count|Int32| Приблизительное количество совпадений поиска с одинаковым значением, указанным в свойстве **Key** . Обратите внимание, что это число не является точным числом совпадений.|
|аггрегатионфилтертокен|String| Маркер, содержащий закодированный фильтр для объединения результатов поиска по определенному значению **ключа** . Чтобы использовать фильтр, передайте маркер в качестве части свойства **аггрегатионфилтер** объекта **сеарчрекуест** в формате **"{Field}: \\ " {аггрегатионфилтертокен} \\ ""**. См. [пример](/graph/search-concept-aggregation#example-2-apply-an-aggregation-filter-based-on-a-previous-request).|

## <a name="json-representation"></a>Представление в формате JSON

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
