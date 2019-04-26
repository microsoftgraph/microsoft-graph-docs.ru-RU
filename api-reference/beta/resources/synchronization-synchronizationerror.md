---
title: Тип ресурса Синчронизатионеррор
description: Представляет сообщение об ошибке, возникшей во время процесса синхронизации.
localization_priority: Normal
ms.openlocfilehash: 7f678cdbd48a3d5f013c22120d01c28bb61738e6
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33324755"
---
# <a name="synchronizationerror-resource-type"></a>Тип ресурса Синчронизатионеррор

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сообщение об ошибке, возникшей во время процесса синхронизации.

## <a name="properties"></a>Свойства

<!-- Add descriptions for the properties. -->
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|code|String||
|message|String||
|Тенантактионабле|Логический||

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
