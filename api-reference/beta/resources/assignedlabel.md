---
title: тип ресурса assignedLabel
description: Представляет метку конфиденциальности, назначенную Microsoft 365 группе. Метки конфиденциальности позволяют администраторам применять определенные групповые параметры в группе, назначая классификацию группе (например, конфиденциальность, высокая конфиденциальность или общие).
ms.localizationpriority: medium
author: psaffaie
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 52b3954982b35e2882092ca76870ba832a7e54f5
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2022
ms.locfileid: "64588836"
---
# <a name="assignedlabel-resource-type"></a>тип ресурса assignedLabel

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет метку конфиденциальности, назначенную Microsoft 365 группе. Метки конфиденциальности позволяют администраторам применять определенные групповые параметры в группе, назначая классификацию группе (например, конфиденциальность, высокая конфиденциальность или общие). Метки конфиденциальности публикуются администраторами в центре Microsoft 365 безопасности & соответствия требованиям в Microsoft Information Protection возможностей. Дополнительные сведения о метки конфиденциальности см. в обзоре [меток Sensitivity](/Office365/SecurityCompliance/sensitivity-labels).

## <a name="properties"></a>Свойства

| Свойство    | Тип   | Описание                               |
| :---------- | :----- | :---------------------------------------- |
| labelId     | Строка | Уникальный идентификатор метки.       |
| displayName | Строка | Имя отображения метки. Только для чтения. |

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.assignedLabel"
}-->

```json
{
  "labelId": "String",
  "displayName": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "assignedLabel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
