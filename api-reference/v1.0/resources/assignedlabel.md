---
title: тип ресурса assignedLabel
description: Представляет метку конфиденциальности, назначенную группе Microsoft 365.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: fa95223aadc4a0b065a3227967a27c8b66b3bff1
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761523"
---
# <a name="assignedlabel-resource-type"></a>тип ресурса assignedLabel

Пространство имен: microsoft.graph

Представляет метку конфиденциальности, назначенную группе Microsoft 365. Метки конфиденциальности позволяют администраторам применять определенные групповые параметры в группе, назначая классификацию группе (например, конфиденциальность, высокая конфиденциальность или общие). Метки конфиденциальности публикуются администраторами в Центре безопасности Microsoft 365 & соответствия требованиям в рамках возможностей Microsoft Information Protection. Дополнительные сведения о метки конфиденциальности см. в обзоре [меток sensitivity.](/microsoft-365/compliance/sensitivity-labels?view=o365-worldwide)

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|labelId|String|Уникальный идентификатор метки.|
|displayName|String|Имя отображения метки. Только для чтения.|

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