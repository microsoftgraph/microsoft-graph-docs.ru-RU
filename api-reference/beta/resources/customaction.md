---
title: Тип ресурса customAction
description: Представляет любые настраиваемые действия, которые может предоставить метка, если настроен администратором.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 1d9c88715cba6fc8faede1419b3c8809c3ec3f54
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941808"
---
# <a name="customaction-resource-type"></a>Тип ресурса customAction

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет любые настраиваемые действия, которые может предоставить метка, если настроен администратором. Настраиваемые действия можно определить как часть [informationProtectionLabel](informationProtectionLabel.md) с помощью модуля PowerShell Центра безопасности и соответствия требованиям Office 365. Действия должны быть понятны потребляемого приложения.

## <a name="properties"></a>Свойства

| Свойство   | Тип                                       | Описание                                          |
| :--------- | :----------------------------------------- | :--------------------------------------------------- |
| name       | String                                     | Имя настраиваемого действия.                           |
| properties | Коллекция [keyValuePair](keyvaluepair.md) | Свойства в формате пары ключевых значений действия. |

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

