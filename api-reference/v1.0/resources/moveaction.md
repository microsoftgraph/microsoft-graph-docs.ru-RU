---
author: daspek
ms.author: dspektor
title: Тип ресурса moveAction
description: Объект MoveAction предоставляет сведения о действии, которое переместит элемент.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 525558d040109e637e2f3532d16c308a197e45fb
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2019
ms.locfileid: "33970817"
---
# <a name="moveaction-resource-type"></a><span data-ttu-id="97013-103">Тип ресурса moveAction</span><span class="sxs-lookup"><span data-stu-id="97013-103">moveAction resource type</span></span>

<span data-ttu-id="97013-104">Присутствие ресурса **moveAction** в [**itemActivity**] [ activity] указывает на то, что действие переместило элемент.</span><span class="sxs-lookup"><span data-stu-id="97013-104">The presence of the **moveAction** resource on an [**itemActivity**][activity] indicates that the activity moved an item.</span></span>

><span data-ttu-id="97013-105">**Примечание:** Записи действий элементов в настоящее время доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="97013-105">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="97013-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="97013-106">Properties</span></span>

| <span data-ttu-id="97013-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="97013-107">Property name</span></span> | <span data-ttu-id="97013-108">Тип</span><span class="sxs-lookup"><span data-stu-id="97013-108">Type</span></span>   | <span data-ttu-id="97013-109">Описание</span><span class="sxs-lookup"><span data-stu-id="97013-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="97013-110">from</span><span class="sxs-lookup"><span data-stu-id="97013-110">from</span></span>          | <span data-ttu-id="97013-111">string</span><span class="sxs-lookup"><span data-stu-id="97013-111">string</span></span> | <span data-ttu-id="97013-112">Имя расположения, из которого был перемещен элемент.</span><span class="sxs-lookup"><span data-stu-id="97013-112">The name of the location the item was moved from.</span></span>
| <span data-ttu-id="97013-113">to</span><span class="sxs-lookup"><span data-stu-id="97013-113">to</span></span>            | <span data-ttu-id="97013-114">string</span><span class="sxs-lookup"><span data-stu-id="97013-114">string</span></span> | <span data-ttu-id="97013-115">Имя расположения, в которое был перемещен элемент.</span><span class="sxs-lookup"><span data-stu-id="97013-115">The name of the location the item was moved to.</span></span>

## <a name="json-representation"></a><span data-ttu-id="97013-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="97013-116">JSON representation</span></span>

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
