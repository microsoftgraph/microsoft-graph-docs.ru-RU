---
title: изменен тип ресурсаQueryToken
description: Представляет измененные сегменты, связанные с исходным запросом пользователя.
ms.localizationpriority: medium
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: edd8a8d121fb28d129fb9a21bf18112ea37f545c
ms.sourcegitcommit: b19b19bf192688f4c513492e8391e4d8dc104633
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/17/2022
ms.locfileid: "62879297"
---
# <a name="alteredquerytoken-resource-type"></a>изменен тип ресурсаQueryToken

Пространство имен: microsoft.graph

Представляет измененные сегменты, связанные с исходным запросом пользователя.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|length|Int32| Определяет длину измененного сегмента.|
|смещение|Int32| Определяет смещение измененного сегмента.|
|предложение|String| Представляет строку исправленного сегмента.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.alteredQueryToken",
  "baseType": null
}-->

```json
{
  "length": "Int32",
  "offset": "Int32",
  "suggestion": "String"
}
```
