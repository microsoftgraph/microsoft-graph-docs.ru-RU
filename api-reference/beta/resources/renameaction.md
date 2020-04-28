---
author: daspek
description: Наличие ресурса RenameAction в ресурсе itemActivity указывает, что в результате выполнения действия элемент был переименован.
ms.date: 09/14/2017
title: RenameAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 6745f932c0a2d9b92273f45e147439cfbd2ed911
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521133"
---
# <a name="renameaction-resource-type"></a><span data-ttu-id="22977-103">Тип ресурса RenameAction</span><span class="sxs-lookup"><span data-stu-id="22977-103">RenameAction resource type</span></span>

<span data-ttu-id="22977-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22977-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22977-105">Наличие ресурса **RenameAction** в ресурсе [**itemActivity**][activity] указывает, что в результате выполнения действия элемент был переименован.</span><span class="sxs-lookup"><span data-stu-id="22977-105">The presence of the **RenameAction** resource on an [**itemActivity**][activity] indicates that the activity renamed an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="22977-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="22977-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="22977-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="22977-107">Properties</span></span>

| <span data-ttu-id="22977-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="22977-108">Property name</span></span> | <span data-ttu-id="22977-109">Тип</span><span class="sxs-lookup"><span data-stu-id="22977-109">Type</span></span>   | <span data-ttu-id="22977-110">Описание</span><span class="sxs-lookup"><span data-stu-id="22977-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="22977-111">oldName</span><span class="sxs-lookup"><span data-stu-id="22977-111">oldName</span></span>       | <span data-ttu-id="22977-112">string</span><span class="sxs-lookup"><span data-stu-id="22977-112">string</span></span> | <span data-ttu-id="22977-113">Предыдущее имя элемента.</span><span class="sxs-lookup"><span data-stu-id="22977-113">The previous name of the item.</span></span>
| <span data-ttu-id="22977-114">Новое</span><span class="sxs-lookup"><span data-stu-id="22977-114">newName</span></span>       | <span data-ttu-id="22977-115">string</span><span class="sxs-lookup"><span data-stu-id="22977-115">string</span></span> | <span data-ttu-id="22977-116">Новое имя элемента.</span><span class="sxs-lookup"><span data-stu-id="22977-116">The new name of the item.</span></span>

## <a name="remarks"></a><span data-ttu-id="22977-117">Замечания</span><span class="sxs-lookup"><span data-stu-id="22977-117">Remarks</span></span>

<span data-ttu-id="22977-118">На данный момент записи о действиях над элементом доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="22977-118">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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
