---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: MoveAction
localization_priority: Normal
ms.openlocfilehash: aa20816165ed4f41e8b89af106e3f781b1be8dd7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562605"
---
# <a name="moveaction-resource-type"></a>Тип ресурса MoveAction

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Наличие ресурса **MoveAction** в ресурсе [**itemActivity**][activity] указывает, что в результате выполнения действия элемент был перемещен.

[activity]: itemactivity.md

## <a name="json-representation"></a>Представление в формате JSON

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
  "suppressions": [
    "Error: /api-reference/beta/resources/moveaction.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
