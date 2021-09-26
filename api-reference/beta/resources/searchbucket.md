---
title: тип ресурса searchBucket
description: Представляет контейнер для одного или более результатов поиска, которые имеют одинаковое значение для поля сущности, которое их агрегируется.
ms.localizationpriority: medium
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: e9323bac249216cc1355e3944f4437d738da89b1
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59764593"
---
# <a name="searchbucket-resource-type"></a>тип ресурса searchBucket

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет контейнер для одного или более результатов поиска, которые имеют одинаковое значение для поля сущности, которое их агрегируется. 

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|aggregationFilterToken|Строка| Маркер, содержащий закодированный фильтр для агрегирования совпадений поиска по определенному **ключевому значению.** Чтобы использовать фильтр, передай маркер как часть свойства **aggregationFilter** в **объекте searchRequest** в формате **"{field}: \\ "{aggregationFilterToken} \\ ""**. См. [пример](/graph/search-concept-aggregation#example-2-apply-an-aggregation-filter-based-on-a-previous-request).|
|count|Int32| Приблизительное число совпадений поиска, которые имеют одинаковое значение, указанное в **свойстве ключа.** Обратите внимание, что это число не является точным числом совпадений.|
|ключа|Строка| Дискретное значение поля, на которое была вычислена агрегация.|

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
