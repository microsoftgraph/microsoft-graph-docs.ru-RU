---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: MoveAction
localization_priority: Normal
ms.openlocfilehash: 40049b506c72af5aacddf461b22e1ddd280d7ad4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27852901"
---
# <a name="moveaction-resource-type"></a><span data-ttu-id="24175-102">Тип ресурса MoveAction</span><span class="sxs-lookup"><span data-stu-id="24175-102">MoveAction resource type</span></span>

> <span data-ttu-id="24175-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="24175-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="24175-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24175-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="24175-105">Наличие ресурса **MoveAction** в ресурсе [**itemActivity**][activity] указывает, что в результате выполнения действия элемент был перемещен.</span><span class="sxs-lookup"><span data-stu-id="24175-105">The presence of the **MoveAction** resource on an [**itemActivity**][activity] indicates that the activity moved an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="24175-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="24175-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="24175-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="24175-107">Properties</span></span>

| <span data-ttu-id="24175-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="24175-108">Property name</span></span> | <span data-ttu-id="24175-109">Тип</span><span class="sxs-lookup"><span data-stu-id="24175-109">Type</span></span>   | <span data-ttu-id="24175-110">Описание</span><span class="sxs-lookup"><span data-stu-id="24175-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="24175-111">from</span><span class="sxs-lookup"><span data-stu-id="24175-111">from</span></span>          | <span data-ttu-id="24175-112">string</span><span class="sxs-lookup"><span data-stu-id="24175-112">string</span></span> | <span data-ttu-id="24175-113">Имя расположения, из которого был перемещен элемент.</span><span class="sxs-lookup"><span data-stu-id="24175-113">The name of the location the item was moved from.</span></span>
| <span data-ttu-id="24175-114">to</span><span class="sxs-lookup"><span data-stu-id="24175-114">to</span></span>            | <span data-ttu-id="24175-115">string</span><span class="sxs-lookup"><span data-stu-id="24175-115">string</span></span> | <span data-ttu-id="24175-116">Имя расположения, в которое был перемещен элемент.</span><span class="sxs-lookup"><span data-stu-id="24175-116">The name of the location the item was moved to.</span></span>

## <a name="remarks"></a><span data-ttu-id="24175-117">Замечания</span><span class="sxs-lookup"><span data-stu-id="24175-117">Remarks</span></span>

<span data-ttu-id="24175-118">На данный момент записи о действиях над элементом доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="24175-118">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The MoveAction object provides information about an activity that moved an item.",
  "keywords": "activities,activity,action,move,moved",
  "section": "documentation",
  "tocPath": "Resources/MoveAction"
} -->
