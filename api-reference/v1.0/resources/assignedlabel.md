---
title: тип ресурса assignedLabel
description: Представляет метку конфиденциальности, назначенную Microsoft 365 группе.
localization_priority: Normal
author: Jordanndahl
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 197ea28fa330c9a91e158cd915d8fb4bb72bca3940dd1d867776424d0cbb116a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54135374"
---
# <a name="assignedlabel-resource-type"></a>тип ресурса assignedLabel

Пространство имен: microsoft.graph

Представляет метку конфиденциальности, назначенную Microsoft 365 группе. Метки конфиденциальности позволяют администраторам применять определенные групповые параметры в группе, назначая классификацию группе (например, конфиденциальность, высокая конфиденциальность или общие). Метки конфиденциальности публикуются администраторами в центре Microsoft 365 безопасности & в рамках Microsoft Information Protection возможностей. Дополнительные сведения о метки конфиденциальности см. в обзоре [меток sensitivity.](/microsoft-365/compliance/sensitivity-labels?view=o365-worldwide)

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