---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: MoveAction
ms.openlocfilehash: d31cfc9a45b83f74058073ca18ca2df15a9914ac
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075589"
---
# <a name="moveaction-resource-type"></a><span data-ttu-id="39c0f-102">Тип ресурса MoveAction</span><span class="sxs-lookup"><span data-stu-id="39c0f-102">MoveAction resource type</span></span>

> <span data-ttu-id="39c0f-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="39c0f-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="39c0f-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39c0f-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="39c0f-105">Наличие ресурса **MoveAction** в ресурсе [**itemActivity**][activity] указывает, что в результате выполнения действия элемент был перемещен.</span><span class="sxs-lookup"><span data-stu-id="39c0f-105">The presence of the **MoveAction** resource on an [**itemActivity**][activity] indicates that the activity moved an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="39c0f-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="39c0f-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="39c0f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="39c0f-107">Properties</span></span>

| <span data-ttu-id="39c0f-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="39c0f-108">Property name</span></span> | <span data-ttu-id="39c0f-109">Тип</span><span class="sxs-lookup"><span data-stu-id="39c0f-109">Type</span></span>   | <span data-ttu-id="39c0f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="39c0f-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="39c0f-111">from</span><span class="sxs-lookup"><span data-stu-id="39c0f-111">from</span></span>          | <span data-ttu-id="39c0f-112">string</span><span class="sxs-lookup"><span data-stu-id="39c0f-112">string</span></span> | <span data-ttu-id="39c0f-113">Имя расположения, из которого был перемещен элемент.</span><span class="sxs-lookup"><span data-stu-id="39c0f-113">The name of the location the item was moved from.</span></span>
| <span data-ttu-id="39c0f-114">to</span><span class="sxs-lookup"><span data-stu-id="39c0f-114">to</span></span>            | <span data-ttu-id="39c0f-115">string</span><span class="sxs-lookup"><span data-stu-id="39c0f-115">string</span></span> | <span data-ttu-id="39c0f-116">Имя расположения, в которое был перемещен элемент.</span><span class="sxs-lookup"><span data-stu-id="39c0f-116">The name of the location the item was moved to.</span></span>

## <a name="remarks"></a><span data-ttu-id="39c0f-117">Замечания</span><span class="sxs-lookup"><span data-stu-id="39c0f-117">Remarks</span></span>

<span data-ttu-id="39c0f-118">На данный момент записи о действиях над элементом доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="39c0f-118">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The MoveAction object provides information about an activity that moved an item.",
  "keywords": "activities,activity,action,move,moved",
  "section": "documentation",
  "tocPath": "Resources/MoveAction"
} -->
