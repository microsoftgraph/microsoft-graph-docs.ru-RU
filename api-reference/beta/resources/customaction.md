---
title: Тип ресурса customAction
description: Представляет все настраиваемые действия, которые могут предоставляться метке, если она настроена администратором.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: bbb3fc99ce474752fd2382d5777afeb1c56f632e
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938872"
---
# <a name="customaction-resource-type"></a>Тип ресурса customAction

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