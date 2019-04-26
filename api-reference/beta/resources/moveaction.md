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
# <a name="moveaction-resource-type"></a><span data-ttu-id="dd1d6-102">Тип ресурса MoveAction</span><span class="sxs-lookup"><span data-stu-id="dd1d6-102">MoveAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dd1d6-103">Наличие ресурса **MoveAction** в ресурсе [**itemActivity**][activity] указывает, что в результате выполнения действия элемент был перемещен.</span><span class="sxs-lookup"><span data-stu-id="dd1d6-103">The presence of the **MoveAction** resource on an [**itemActivity**][activity] indicates that the activity moved an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="dd1d6-104">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="dd1d6-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="dd1d6-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="dd1d6-105">Properties</span></span>

| <span data-ttu-id="dd1d6-106">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="dd1d6-106">Property name</span></span> | <span data-ttu-id="dd1d6-107">Тип</span><span class="sxs-lookup"><span data-stu-id="dd1d6-107">Type</span></span>   | <span data-ttu-id="dd1d6-108">Описание</span><span class="sxs-lookup"><span data-stu-id="dd1d6-108">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="dd1d6-109">from</span><span class="sxs-lookup"><span data-stu-id="dd1d6-109">from</span></span>          | <span data-ttu-id="dd1d6-110">string</span><span class="sxs-lookup"><span data-stu-id="dd1d6-110">string</span></span> | <span data-ttu-id="dd1d6-111">Имя расположения, из которого был перемещен элемент.</span><span class="sxs-lookup"><span data-stu-id="dd1d6-111">The name of the location the item was moved from.</span></span>
| <span data-ttu-id="dd1d6-112">to</span><span class="sxs-lookup"><span data-stu-id="dd1d6-112">to</span></span>            | <span data-ttu-id="dd1d6-113">string</span><span class="sxs-lookup"><span data-stu-id="dd1d6-113">string</span></span> | <span data-ttu-id="dd1d6-114">Имя расположения, в которое был перемещен элемент.</span><span class="sxs-lookup"><span data-stu-id="dd1d6-114">The name of the location the item was moved to.</span></span>

## <a name="remarks"></a><span data-ttu-id="dd1d6-115">Замечания</span><span class="sxs-lookup"><span data-stu-id="dd1d6-115">Remarks</span></span>

<span data-ttu-id="dd1d6-116">На данный момент записи о действиях над элементом доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="dd1d6-116">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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
