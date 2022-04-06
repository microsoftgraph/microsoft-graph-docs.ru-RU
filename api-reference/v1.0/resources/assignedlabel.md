---
title: тип ресурса assignedLabel
description: Представляет метку конфиденциальности, назначенную Microsoft 365 группе.
ms.localizationpriority: medium
author: psaffaie
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: a4992960d63c90efb06d3799944c9df66616759c
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2022
ms.locfileid: "64588325"
---
# <a name="assignedlabel-resource-type"></a>тип ресурса assignedLabel

Пространство имен: microsoft.graph

Представляет метку конфиденциальности, назначенную Microsoft 365 группе. Метки конфиденциальности позволяют администраторам применять определенные групповые параметры в группе, назначая классификацию группе (например, конфиденциальность, высокая конфиденциальность или общие). Метки конфиденциальности публикуются администраторами в центре Microsoft 365 безопасности & соответствия требованиям в Microsoft Information Protection возможностей. Дополнительные сведения о метки конфиденциальности см. в обзоре [меток Sensitivity](/microsoft-365/compliance/sensitivity-labels?view=o365-worldwide).

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
