---
title: Тип ресурса synchronizationError
description: Представляет ошибки, возникшей во время синхронизации.
localization_priority: Normal
ms.openlocfilehash: cc6b58444ac56303bfd2e41f1fcae17658f6aea9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27847245"
---
# <a name="synchronizationerror-resource-type"></a>Тип ресурса synchronizationError

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Представляет ошибки, возникшей во время синхронизации.

## <a name="properties"></a>Свойства

<!-- Add descriptions for the properties. -->
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|code|Строка||
|message|String||
|tenantActionable|Логический||

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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
