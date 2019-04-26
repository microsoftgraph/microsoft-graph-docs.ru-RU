---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: MoveAction
localization_priority: Normal
ms.openlocfilehash: 0715f8e9743c4384e8fbd851fe88563e9eaf9666
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342224"
---
# <a name="moveaction-resource-type"></a><span data-ttu-id="3e958-102">Тип ресурса MoveAction</span><span class="sxs-lookup"><span data-stu-id="3e958-102">MoveAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e958-103">Наличие ресурса **MoveAction** в ресурсе [**itemActivity**][activity] указывает, что в результате выполнения действия элемент был перемещен.</span><span class="sxs-lookup"><span data-stu-id="3e958-103">The presence of the **MoveAction** resource on an [**itemActivity**][activity] indicates that the activity moved an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="3e958-104">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="3e958-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="3e958-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="3e958-105">Properties</span></span>

| <span data-ttu-id="3e958-106">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="3e958-106">Property name</span></span> | <span data-ttu-id="3e958-107">Тип</span><span class="sxs-lookup"><span data-stu-id="3e958-107">Type</span></span>   | <span data-ttu-id="3e958-108">Описание</span><span class="sxs-lookup"><span data-stu-id="3e958-108">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="3e958-109">from</span><span class="sxs-lookup"><span data-stu-id="3e958-109">from</span></span>          | <span data-ttu-id="3e958-110">string</span><span class="sxs-lookup"><span data-stu-id="3e958-110">string</span></span> | <span data-ttu-id="3e958-111">Имя расположения, из которого был перемещен элемент.</span><span class="sxs-lookup"><span data-stu-id="3e958-111">The name of the location the item was moved from.</span></span>
| <span data-ttu-id="3e958-112">to</span><span class="sxs-lookup"><span data-stu-id="3e958-112">to</span></span>            | <span data-ttu-id="3e958-113">string</span><span class="sxs-lookup"><span data-stu-id="3e958-113">string</span></span> | <span data-ttu-id="3e958-114">Имя расположения, в которое был перемещен элемент.</span><span class="sxs-lookup"><span data-stu-id="3e958-114">The name of the location the item was moved to.</span></span>

## <a name="remarks"></a><span data-ttu-id="3e958-115">Замечания</span><span class="sxs-lookup"><span data-stu-id="3e958-115">Remarks</span></span>

<span data-ttu-id="3e958-116">На данный момент записи о действиях над элементом доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="3e958-116">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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
