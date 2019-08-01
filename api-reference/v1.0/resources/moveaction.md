---
author: daspek
ms.author: dspektor
title: Тип ресурса moveAction
description: Объект MoveAction предоставляет сведения о действии, которое переместит элемент.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 8ef93cd83c8fd020af91a9ea8c9288c1d27d5cf6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036073"
---
# <a name="moveaction-resource-type"></a><span data-ttu-id="4530a-103">Тип ресурса moveAction</span><span class="sxs-lookup"><span data-stu-id="4530a-103">moveAction resource type</span></span>

<span data-ttu-id="4530a-104">Присутствие ресурса **moveAction** в [**itemActivity**][activity] указывает на то, что действие переместило элемент.</span><span class="sxs-lookup"><span data-stu-id="4530a-104">The presence of the **moveAction** resource on an [**itemActivity**][activity] indicates that the activity moved an item.</span></span>

><span data-ttu-id="4530a-105">**Примечание:** Записи действий элементов в настоящее время доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="4530a-105">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="4530a-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="4530a-106">Properties</span></span>

| <span data-ttu-id="4530a-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="4530a-107">Property name</span></span> | <span data-ttu-id="4530a-108">Тип</span><span class="sxs-lookup"><span data-stu-id="4530a-108">Type</span></span>   | <span data-ttu-id="4530a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="4530a-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="4530a-110">from</span><span class="sxs-lookup"><span data-stu-id="4530a-110">from</span></span>          | <span data-ttu-id="4530a-111">string</span><span class="sxs-lookup"><span data-stu-id="4530a-111">string</span></span> | <span data-ttu-id="4530a-112">Имя расположения, из которого был перемещен элемент.</span><span class="sxs-lookup"><span data-stu-id="4530a-112">The name of the location the item was moved from.</span></span>
| <span data-ttu-id="4530a-113">to</span><span class="sxs-lookup"><span data-stu-id="4530a-113">to</span></span>            | <span data-ttu-id="4530a-114">string</span><span class="sxs-lookup"><span data-stu-id="4530a-114">string</span></span> | <span data-ttu-id="4530a-115">Имя расположения, в которое был перемещен элемент.</span><span class="sxs-lookup"><span data-stu-id="4530a-115">The name of the location the item was moved to.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4530a-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4530a-116">JSON representation</span></span>

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
