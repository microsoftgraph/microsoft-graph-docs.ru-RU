---
title: Тип ресурса assignedLabel
description: Представляет метку конфиденциальности, назначенную группе Microsoft 365.
ms.localizationpriority: medium
author: psaffaie
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 1088ad83b8f2a46d687c234a9b7c87d7e2943ef5
ms.sourcegitcommit: 6a4e81d2b8e7447771c9060998c7e1cc18a57902
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/03/2022
ms.locfileid: "66609740"
---
# <a name="assignedlabel-resource-type"></a>Тип ресурса assignedLabel

Пространство имен: microsoft.graph

Представляет метку конфиденциальности, назначенную группе Microsoft 365. Метки конфиденциальности позволяют администраторам применять определенные параметры группы, назначая группе классификацию (например, "Конфиденциально", "Строго конфиденциально" или "Общие"). Метки конфиденциальности публикуются администраторами в Центре соответствия & безопасности Microsoft 365 в Защита информации Microsoft Purview безопасности. Дополнительные сведения о метках конфиденциальности см. в [обзоре меток конфиденциальности](/microsoft-365/compliance/sensitivity-labels).

## <a name="properties"></a>Свойства

| Свойство    | Тип   | Описание                               |
| :---------- | :----- | :---------------------------------------- |
| labelId     | String | Уникальный идентификатор метки.       |
| displayName | String | Отображаемое имя метки. Только для чтения. |

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
