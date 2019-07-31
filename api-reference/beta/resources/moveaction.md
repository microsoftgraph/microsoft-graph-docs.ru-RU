---
author: daspek
description: Наличие ресурса MoveAction в ресурсе itemActivity указывает, что в результате выполнения действия элемент был перемещен.
ms.date: 09/14/2017
title: MoveAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 9fbb19097b6a1401bd3c0b6dba4ce1fd5649e706
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009645"
---
# <a name="moveaction-resource-type"></a><span data-ttu-id="6fd28-103">Тип ресурса MoveAction</span><span class="sxs-lookup"><span data-stu-id="6fd28-103">MoveAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6fd28-104">Наличие ресурса **MoveAction** в ресурсе [**itemActivity**][activity] указывает, что в результате выполнения действия элемент был перемещен.</span><span class="sxs-lookup"><span data-stu-id="6fd28-104">The presence of the **MoveAction** resource on an [**itemActivity**][activity] indicates that the activity moved an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="6fd28-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6fd28-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="6fd28-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="6fd28-106">Properties</span></span>

| <span data-ttu-id="6fd28-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="6fd28-107">Property name</span></span> | <span data-ttu-id="6fd28-108">Тип</span><span class="sxs-lookup"><span data-stu-id="6fd28-108">Type</span></span>   | <span data-ttu-id="6fd28-109">Описание</span><span class="sxs-lookup"><span data-stu-id="6fd28-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="6fd28-110">from</span><span class="sxs-lookup"><span data-stu-id="6fd28-110">from</span></span>          | <span data-ttu-id="6fd28-111">string</span><span class="sxs-lookup"><span data-stu-id="6fd28-111">string</span></span> | <span data-ttu-id="6fd28-112">Имя расположения, из которого был перемещен элемент.</span><span class="sxs-lookup"><span data-stu-id="6fd28-112">The name of the location the item was moved from.</span></span>
| <span data-ttu-id="6fd28-113">to</span><span class="sxs-lookup"><span data-stu-id="6fd28-113">to</span></span>            | <span data-ttu-id="6fd28-114">string</span><span class="sxs-lookup"><span data-stu-id="6fd28-114">string</span></span> | <span data-ttu-id="6fd28-115">Имя расположения, в которое был перемещен элемент.</span><span class="sxs-lookup"><span data-stu-id="6fd28-115">The name of the location the item was moved to.</span></span>

## <a name="remarks"></a><span data-ttu-id="6fd28-116">Замечания</span><span class="sxs-lookup"><span data-stu-id="6fd28-116">Remarks</span></span>

<span data-ttu-id="6fd28-117">На данный момент записи о действиях над элементом доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="6fd28-117">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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
