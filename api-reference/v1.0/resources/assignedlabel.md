---
title: Тип ресурса assignedLabel
description: Представляет метку конфиденциальности, назначенную группе Microsoft 365.
ms.localizationpriority: medium
author: psaffaie
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: bcc89583a1611093c58f4cd7cbe2ec6907820945
ms.sourcegitcommit: 9adff6756e27aabbf36a9adbc2269b13c7fa74ef
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2022
ms.locfileid: "65883952"
---
# <a name="assignedlabel-resource-type"></a>Тип ресурса assignedLabel

Пространство имен: microsoft.graph

Представляет метку конфиденциальности, назначенную группе Microsoft 365. Метки конфиденциальности позволяют администраторам применять определенные параметры группы, назначая группе классификацию (например, "Конфиденциально", "Строго конфиденциально" или "Общие"). Метки конфиденциальности публикуются администраторами в Центре соответствия & безопасности Microsoft 365 в рамках возможностей Microsoft Purview Information Protection. Дополнительные сведения о метках конфиденциальности см. в [обзоре меток конфиденциальности](/microsoft-365/compliance/sensitivity-labels?view=o365-worldwide).

## <a name="properties"></a>Свойства

| Свойство    | Тип   | Описание                               |
| :---------- | :----- | :---------------------------------------- |
| labelId     | Строка | Уникальный идентификатор метки.       |
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
