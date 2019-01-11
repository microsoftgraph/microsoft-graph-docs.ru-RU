---
title: Тип ресурса extension
description: Абстрактный тип для поддержки открытого типа openTypeExtension в OData 4-й версии.
localization_priority: Normal
ms.openlocfilehash: 6a07a341e812ebb119c13b7003841450163cbdd2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869302"
---
# <a name="extension-resource-type"></a>Тип ресурса extension

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Абстрактный тип для поддержки открытого типа [openTypeExtension](opentypeextension.md) в OData 4-й версии.

## <a name="json-representation"></a>Представление JSON

Ниже показано представление JSON ресурса.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.extension"
}-->

```json
{
  "id": "string (identifier)"
}

```
## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|Строка| Только для чтения.|

## <a name="relationships"></a>Связи
Нет


## <a name="methods"></a>Методы

Фактически поддерживаемые методы указаны в описании производного типа [openTypeExtension](opentypeextension.md).


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "extension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
