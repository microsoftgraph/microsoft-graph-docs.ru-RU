---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: RestoreAction
localization_priority: Normal
ms.openlocfilehash: f04f9811cefba60d0b06b99605774fb8fbfa0125
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514077"
---
# <a name="restoreaction-resource-type"></a>Тип ресурса RestoreAction

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Наличие ресурса **RestoreAction** в ресурсе [**itemActivity**][activity] указывает, что в результате выполнения действия элемент был восстановлен.

**Примечание.** На данный момент этот ресурс пуст, но в будущих редакциях API в него могут быть добавлены дополнительные свойства.

[activity]: itemactivity.md

## <a name="json-representation"></a>Представление в формате JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.restoreAction"
}-->

```json
{
}
```

## <a name="properties"></a>Свойства

Нет. Этот аспект принимает нулевое или ненулевое значение и не содержит свойств.

## <a name="remarks"></a>Замечания

На данный момент записи о действиях над элементом доступны только в SharePoint и OneDrive для бизнеса.

<!--
{
  "type": "#page.annotation",
  "description": "The RestoreAction object provides information about an activity that restored an item.",
  "keywords": "activities,activity,action,restore,undelete",
  "section": "documentation",
  "tocPath": "Resources/RestoreAction",
  "suppressions": [
    "Error: /api-reference/beta/resources/restoreaction.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
