---
author: daspek
ms.author: dspektor
title: Тип ресурса moveAction
description: Объект MoveAction предоставляет сведения о действии, которое переместит элемент.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 525558d040109e637e2f3532d16c308a197e45fb
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2019
ms.locfileid: "33970817"
---
# <a name="moveaction-resource-type"></a>Тип ресурса moveAction

Присутствие ресурса **moveAction** в [**itemActivity**] [ activity] указывает на то, что действие переместило элемент.

>**Примечание:** Записи действий элементов в настоящее время доступны только в SharePoint и OneDrive для бизнеса.

[activity]: itemactivity.md

## <a name="properties"></a>Свойства

| Имя свойства | Тип   | Описание
|:--------------|:-------|:----------------------------------------------------
| from          | string | Имя расположения, из которого был перемещен элемент.
| to            | string | Имя расположения, в которое был перемещен элемент.

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
