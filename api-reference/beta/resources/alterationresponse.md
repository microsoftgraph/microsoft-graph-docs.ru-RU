---
title: тип ресурса alterationResponse
description: Предоставляет сведения, связанные с исправлениями орфографии в ответе на изменения.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: e23b94b4e35776b2278c7818efc71f14edcc6cbb
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52068236"
---
# <a name="alterationresponse-resource-type"></a>тип ресурса alterationResponse

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Предоставляет сведения, связанные с исправлениями орфографии в ответе на изменения.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|originalQueryString|String| Определяет исходную строку запроса пользователя.|
|queryAlteration|[searchAlteration](searchalteration.md)| Определяет сведения об изменениях для исправления орфографии.|
|queryAlterationType|searchAlterationType| Определяет тип коррекции орфографии. Возможные значения `suggestion` : `modification` .|

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.alterationResponse",
  "baseType": null
}-->

```json
{
  "originalQueryString": "String",
  "queryAlteration": "String",
  "queryAlterationType": "suggestion"
}
```
