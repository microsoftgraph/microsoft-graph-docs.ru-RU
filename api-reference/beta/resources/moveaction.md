---
author: daspek
description: Наличие ресурса MoveAction в ресурсе itemActivity указывает, что в результате выполнения действия элемент был перемещен.
ms.date: 09/14/2017
title: MoveAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: a42ef869a32cfe01a03344d3f155880bd528c462
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522619"
---
# <a name="moveaction-resource-type"></a><span data-ttu-id="c7757-103">Тип ресурса MoveAction</span><span class="sxs-lookup"><span data-stu-id="c7757-103">MoveAction resource type</span></span>

<span data-ttu-id="c7757-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c7757-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7757-105">Наличие ресурса **MoveAction** в ресурсе [**itemActivity**][activity] указывает, что в результате выполнения действия элемент был перемещен.</span><span class="sxs-lookup"><span data-stu-id="c7757-105">The presence of the **MoveAction** resource on an [**itemActivity**][activity] indicates that the activity moved an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="c7757-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c7757-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="c7757-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="c7757-107">Properties</span></span>

| <span data-ttu-id="c7757-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="c7757-108">Property name</span></span> | <span data-ttu-id="c7757-109">Тип</span><span class="sxs-lookup"><span data-stu-id="c7757-109">Type</span></span>   | <span data-ttu-id="c7757-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c7757-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="c7757-111">from</span><span class="sxs-lookup"><span data-stu-id="c7757-111">from</span></span>          | <span data-ttu-id="c7757-112">строка</span><span class="sxs-lookup"><span data-stu-id="c7757-112">string</span></span> | <span data-ttu-id="c7757-113">Имя расположения, из которого был перемещен элемент.</span><span class="sxs-lookup"><span data-stu-id="c7757-113">The name of the location the item was moved from.</span></span>
| <span data-ttu-id="c7757-114">to</span><span class="sxs-lookup"><span data-stu-id="c7757-114">to</span></span>            | <span data-ttu-id="c7757-115">string</span><span class="sxs-lookup"><span data-stu-id="c7757-115">string</span></span> | <span data-ttu-id="c7757-116">Имя расположения, в которое был перемещен элемент.</span><span class="sxs-lookup"><span data-stu-id="c7757-116">The name of the location the item was moved to.</span></span>

## <a name="remarks"></a><span data-ttu-id="c7757-117">Замечания</span><span class="sxs-lookup"><span data-stu-id="c7757-117">Remarks</span></span>

<span data-ttu-id="c7757-118">На данный момент записи о действиях над элементом доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="c7757-118">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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
