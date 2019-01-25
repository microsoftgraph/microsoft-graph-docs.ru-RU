---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: EditAction
localization_priority: Normal
ms.openlocfilehash: e319f6889b520f90d9414c4115060edbe2e2f0cc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526769"
---
# <a name="editaction-resource-type"></a><span data-ttu-id="2e9ce-102">Тип ресурса EditAction</span><span class="sxs-lookup"><span data-stu-id="2e9ce-102">EditAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2e9ce-103">Наличие ресурса **EditAction** в ресурсе [**itemActivity**][activity] указывает, что в результате выполнения действия элемент был изменен.</span><span class="sxs-lookup"><span data-stu-id="2e9ce-103">The presence of the **EditAction** resource on an [**itemActivity**][activity] indicates that the activity edited an item.</span></span>

<span data-ttu-id="2e9ce-104">**Примечание.** На данный момент этот ресурс пуст, но в будущих редакциях API в него могут быть добавлены дополнительные свойства.</span><span class="sxs-lookup"><span data-stu-id="2e9ce-104">**Note**: While this resource is empty today, in future API revisions it may be populated with additional properties.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="2e9ce-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="2e9ce-105">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.editAction"
}-->

```json
{
}
```

## <a name="properties"></a><span data-ttu-id="2e9ce-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="2e9ce-106">Properties</span></span>

<span data-ttu-id="2e9ce-107">Нет.</span><span class="sxs-lookup"><span data-stu-id="2e9ce-107">None.</span></span> <span data-ttu-id="2e9ce-108">Этот аспект принимает нулевое или ненулевое значение и не содержит свойств.</span><span class="sxs-lookup"><span data-stu-id="2e9ce-108">This facet is a null or not-null value and contains no properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="2e9ce-109">Замечания</span><span class="sxs-lookup"><span data-stu-id="2e9ce-109">Remarks</span></span>

<span data-ttu-id="2e9ce-110">На данный момент записи о действиях над элементом доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="2e9ce-110">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The EditAction object provides information about an activity that edited an item.",
  "keywords": "activities,activity,action,edit,modify",
  "section": "documentation",
  "tocPath": "Resources/EditAction",
  "suppressions": [
    "Error: /api-reference/beta/resources/editaction.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
