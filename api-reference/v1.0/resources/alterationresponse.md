---
title: тип ресурса alterationResponse
description: Предоставляет сведения, связанные с исправлениями орфографии в ответе на изменения.
ms.localizationpriority: medium
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: b26b3aee1db86018b8a32f5e2a4bb1b245ee7c5a
ms.sourcegitcommit: b19b19bf192688f4c513492e8391e4d8dc104633
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/17/2022
ms.locfileid: "62879289"
---
# <a name="alterationresponse-resource-type"></a>тип ресурса alterationResponse

Пространство имен: microsoft.graph

Предоставляет сведения, связанные с исправлениями орфографии в ответе на изменения.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|originalQueryString|String| Определяет исходную строку запроса пользователя.|
|queryAlteration|[searchAlteration](searchalteration.md)| Определяет сведения об изменениях для исправления орфографии.|
|queryAlterationType|searchAlterationType| Определяет тип коррекции орфографии. Возможные значения: `suggestion`, `modification`.|

## <a name="json-representation"></a>Представление JSON

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
  "queryAlterationType": "String"
}
```
