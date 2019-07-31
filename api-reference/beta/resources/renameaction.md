---
author: daspek
description: Наличие ресурса RenameAction в ресурсе itemActivity указывает, что в результате выполнения действия элемент был переименован.
ms.date: 09/14/2017
title: RenameAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: d62d3f7f836ece716bdc3e616e1943de8c040652
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965427"
---
# <a name="renameaction-resource-type"></a><span data-ttu-id="7c884-103">Тип ресурса RenameAction</span><span class="sxs-lookup"><span data-stu-id="7c884-103">RenameAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7c884-104">Наличие ресурса **RenameAction** в ресурсе [**itemActivity**][activity] указывает, что в результате выполнения действия элемент был переименован.</span><span class="sxs-lookup"><span data-stu-id="7c884-104">The presence of the **RenameAction** resource on an [**itemActivity**][activity] indicates that the activity renamed an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="7c884-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7c884-105">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.renameAction"
}-->

```json
{
  "oldName": "string",
  "newName": "string"
}
```

## <a name="properties"></a><span data-ttu-id="7c884-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="7c884-106">Properties</span></span>

| <span data-ttu-id="7c884-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="7c884-107">Property name</span></span> | <span data-ttu-id="7c884-108">Тип</span><span class="sxs-lookup"><span data-stu-id="7c884-108">Type</span></span>   | <span data-ttu-id="7c884-109">Описание</span><span class="sxs-lookup"><span data-stu-id="7c884-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="7c884-110">oldName</span><span class="sxs-lookup"><span data-stu-id="7c884-110">oldName</span></span>       | <span data-ttu-id="7c884-111">string</span><span class="sxs-lookup"><span data-stu-id="7c884-111">string</span></span> | <span data-ttu-id="7c884-112">Предыдущее имя элемента.</span><span class="sxs-lookup"><span data-stu-id="7c884-112">The previous name of the item.</span></span>
| <span data-ttu-id="7c884-113">Новое</span><span class="sxs-lookup"><span data-stu-id="7c884-113">newName</span></span>       | <span data-ttu-id="7c884-114">string</span><span class="sxs-lookup"><span data-stu-id="7c884-114">string</span></span> | <span data-ttu-id="7c884-115">Новое имя элемента.</span><span class="sxs-lookup"><span data-stu-id="7c884-115">The new name of the item.</span></span>

## <a name="remarks"></a><span data-ttu-id="7c884-116">Замечания</span><span class="sxs-lookup"><span data-stu-id="7c884-116">Remarks</span></span>

<span data-ttu-id="7c884-117">На данный момент записи о действиях над элементом доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="7c884-117">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The RenameAction object provides information about an activity that renamed an item.",
  "keywords": "activities,activity,action,rename,renamed",
  "section": "documentation",
  "tocPath": "Resources/RenameAction",
  "suppressions": []
}
-->
