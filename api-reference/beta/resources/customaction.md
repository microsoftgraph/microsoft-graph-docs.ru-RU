---
title: Тип ресурса customAction
description: Представляет все настраиваемые действия, которые могут предоставляться метке, если она настроена администратором.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5c71454a6647604d4155fc80c72ec48d22d85d03
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48050012"
---
# <a name="customaction-resource-type"></a>Тип ресурса customAction

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет все настраиваемые действия, которые могут предоставляться метке, если она настроена администратором. Настраиваемые действия могут быть определены как часть [информатионпротектионлабел](informationProtectionLabel.md) с помощью модуля PowerShell центра безопасности и соответствия требованиям Office 365. Приложение должно понимать действия, которые использует приложение.

## <a name="properties"></a>Свойства

| Свойство   | Тип                                       | Описание                                          |
| :--------- | :----------------------------------------- | :--------------------------------------------------- |
| name       | String                                     | Имя дополнительного действия.                           |
| properties | Коллекция [keyValuePair](keyvaluepair.md) | Свойства, в формате "комбинация значений ключей" действия. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.customAction",
  "baseType": "microsoft.graph.informationProtectionAction"
}-->

```json
{
  "name": "String",
  "properties": [{"@odata.type": "microsoft.graph.keyValuePair"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "customAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

