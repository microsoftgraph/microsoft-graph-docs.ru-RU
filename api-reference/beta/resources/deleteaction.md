---
author: daspek
description: Наличие ресурса DeleteAction в ресурсе itemActivity указывает, что в результате выполнения действия элемент был удален.
ms.date: 09/14/2017
title: DeleteAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: c5617c61f3221351930ab8d4bf940eaf1efa0629
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973851"
---
# <a name="deleteaction-resource-type"></a><span data-ttu-id="c00b6-103">Тип ресурса DeleteAction</span><span class="sxs-lookup"><span data-stu-id="c00b6-103">DeleteAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c00b6-104">Наличие ресурса **DeleteAction** в ресурсе [**itemActivity**][activity] указывает, что в результате выполнения действия элемент был удален.</span><span class="sxs-lookup"><span data-stu-id="c00b6-104">The presence of the **DeleteAction** resource on an [**itemActivity**][activity] indicates that the activity deleted an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="c00b6-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c00b6-105">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.deleteAction"
}-->

```json
{
  "name": "string",
  "objectType": "File | Folder"
}
```

## <a name="properties"></a><span data-ttu-id="c00b6-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="c00b6-106">Properties</span></span>

| <span data-ttu-id="c00b6-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="c00b6-107">Property name</span></span> | <span data-ttu-id="c00b6-108">Тип</span><span class="sxs-lookup"><span data-stu-id="c00b6-108">Type</span></span>   | <span data-ttu-id="c00b6-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c00b6-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="c00b6-110">name</span><span class="sxs-lookup"><span data-stu-id="c00b6-110">name</span></span>          | <span data-ttu-id="c00b6-111">string</span><span class="sxs-lookup"><span data-stu-id="c00b6-111">string</span></span> | <span data-ttu-id="c00b6-112">Имя элемента, который был удален.</span><span class="sxs-lookup"><span data-stu-id="c00b6-112">The name of the item that was deleted.</span></span>
| <span data-ttu-id="c00b6-113">objectType</span><span class="sxs-lookup"><span data-stu-id="c00b6-113">objectType</span></span>    | <span data-ttu-id="c00b6-114">string</span><span class="sxs-lookup"><span data-stu-id="c00b6-114">string</span></span> | <span data-ttu-id="c00b6-115">`File`или `Folder`, в зависимости от типа удаленного элемента.</span><span class="sxs-lookup"><span data-stu-id="c00b6-115">`File` or `Folder`, depending on the type of the deleted item.</span></span>

## <a name="remarks"></a><span data-ttu-id="c00b6-116">Замечания</span><span class="sxs-lookup"><span data-stu-id="c00b6-116">Remarks</span></span>

<span data-ttu-id="c00b6-117">На данный момент записи о действиях над элементом доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="c00b6-117">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The DeleteAction object provides information about the deletion of an item.",
  "keywords": "activities,activity,action,delete,deletion",
  "section": "documentation",
  "tocPath": "Resources/DeleteAction",
  "suppressions": []
}
-->
