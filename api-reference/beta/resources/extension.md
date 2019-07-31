---
title: Тип ресурса extension
description: Абстрактный тип для поддержки открытого типа openTypeExtension в OData 4-й версии.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 48b48eb4e87be79c65636320f5d93d4e5c6c800b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973587"
---
# <a name="extension-resource-type"></a>Тип ресурса extension

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
|id|String| Только для чтения.|

## <a name="relationships"></a>Отношения
Нет


## <a name="methods"></a>Методы

Фактически поддерживаемые методы указаны в описании производного типа [openTypeExtension](opentypeextension.md).


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "extension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
