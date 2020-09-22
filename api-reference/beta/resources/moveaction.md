---
author: daspek
description: Наличие ресурса MoveAction в ресурсе itemActivity указывает, что в результате выполнения действия элемент был перемещен.
ms.date: 09/14/2017
title: MoveAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 547a49e17a74be43500a9cf52aaa3a375272b810
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021289"
---
# <a name="moveaction-resource-type"></a>Тип ресурса MoveAction

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Наличие ресурса **MoveAction** в ресурсе [**itemActivity**][activity] указывает, что в результате выполнения действия элемент был перемещен.

[activity]: itemactivity.md

## <a name="json-representation"></a>Представление JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.moveAction"
}-->

```json
{
  "from": "string",
  "to": "string"
}
```

## <a name="properties"></a>Свойства

| Имя свойства | Тип   | Описание
|:--------------|:-------|:----------------------------------------------------
| from          | string | Имя расположения, из которого был перемещен элемент.
| to            | string | Имя расположения, в которое был перемещен элемент.

## <a name="remarks"></a>Замечания

На данный момент записи о действиях над элементом доступны только в SharePoint и OneDrive для бизнеса.

<!--
{
  "type": "#page.annotation",
  "description": "The MoveAction object provides information about an activity that moved an item.",
  "keywords": "activities,activity,action,move,moved",
  "section": "documentation",
  "tocPath": "Resources/MoveAction",
  "suppressions": []
}
-->


