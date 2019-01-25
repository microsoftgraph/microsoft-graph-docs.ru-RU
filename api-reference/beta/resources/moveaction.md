---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: MoveAction
localization_priority: Normal
ms.openlocfilehash: aa20816165ed4f41e8b89af106e3f781b1be8dd7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29530085"
---
# <a name="moveaction-resource-type"></a><span data-ttu-id="0ad08-102">Тип ресурса MoveAction</span><span class="sxs-lookup"><span data-stu-id="0ad08-102">MoveAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ad08-103">Наличие ресурса **MoveAction** в ресурсе [**itemActivity**][activity] указывает, что в результате выполнения действия элемент был перемещен.</span><span class="sxs-lookup"><span data-stu-id="0ad08-103">The presence of the **MoveAction** resource on an [**itemActivity**][activity] indicates that the activity moved an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="0ad08-104">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="0ad08-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="0ad08-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="0ad08-105">Properties</span></span>

| <span data-ttu-id="0ad08-106">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="0ad08-106">Property name</span></span> | <span data-ttu-id="0ad08-107">Тип</span><span class="sxs-lookup"><span data-stu-id="0ad08-107">Type</span></span>   | <span data-ttu-id="0ad08-108">Описание</span><span class="sxs-lookup"><span data-stu-id="0ad08-108">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="0ad08-109">from</span><span class="sxs-lookup"><span data-stu-id="0ad08-109">from</span></span>          | <span data-ttu-id="0ad08-110">string</span><span class="sxs-lookup"><span data-stu-id="0ad08-110">string</span></span> | <span data-ttu-id="0ad08-111">Имя расположения, из которого был перемещен элемент.</span><span class="sxs-lookup"><span data-stu-id="0ad08-111">The name of the location the item was moved from.</span></span>
| <span data-ttu-id="0ad08-112">to</span><span class="sxs-lookup"><span data-stu-id="0ad08-112">to</span></span>            | <span data-ttu-id="0ad08-113">string</span><span class="sxs-lookup"><span data-stu-id="0ad08-113">string</span></span> | <span data-ttu-id="0ad08-114">Имя расположения, в которое был перемещен элемент.</span><span class="sxs-lookup"><span data-stu-id="0ad08-114">The name of the location the item was moved to.</span></span>

## <a name="remarks"></a><span data-ttu-id="0ad08-115">Замечания</span><span class="sxs-lookup"><span data-stu-id="0ad08-115">Remarks</span></span>

<span data-ttu-id="0ad08-116">На данный момент записи о действиях над элементом доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="0ad08-116">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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
