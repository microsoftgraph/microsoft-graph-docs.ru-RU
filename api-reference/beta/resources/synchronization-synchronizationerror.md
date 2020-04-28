---
title: Тип ресурса Синчронизатионеррор
description: Представляет сообщение об ошибке, возникшей во время процесса синхронизации.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 884c39273d8d474a228cd8f4a8f2b321950e8caf
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43217551"
---
# <a name="synchronizationerror-resource-type"></a>Тип ресурса Синчронизатионеррор

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сообщение об ошибке, возникшей во время процесса синхронизации.

## <a name="properties"></a>Свойства

<!-- Add descriptions for the properties. -->
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|code|String||
|message|String||
|тенантактионабле|Boolean||

## <a name="json-representation"></a>Представление JSON

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
