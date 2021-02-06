---
title: Тип ресурса synchronizationError
description: Представляет ошибку, которая произошла в процессе синхронизации.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: a49f2cf9b9d3e621533490127a5b2674ab43bf14
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131490"
---
# <a name="synchronizationerror-resource-type"></a>Тип ресурса synchronizationError

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет ошибку, которая произошла в процессе синхронизации.

## <a name="properties"></a>Свойства

<!-- Add descriptions for the properties. -->
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|code|Строка||
|message|String||
|tenantActionable|Boolean||

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationError"
}-->

```json
{
  "code": "String",
  "message": "String",
  "tenantActionable": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


