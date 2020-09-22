---
author: daspek
description: Наличие ресурса DeleteAction в ресурсе itemActivity указывает, что в результате выполнения действия элемент был удален.
ms.date: 09/14/2017
title: DeleteAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: b8f00827a37ba9c010acd1b52e751bd55638afb3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48049886"
---
# <a name="deleteaction-resource-type"></a><span data-ttu-id="b8862-103">Тип ресурса DeleteAction</span><span class="sxs-lookup"><span data-stu-id="b8862-103">DeleteAction resource type</span></span>

<span data-ttu-id="b8862-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b8862-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b8862-105">Наличие ресурса **DeleteAction** в ресурсе [**itemActivity**][activity] указывает, что в результате выполнения действия элемент был удален.</span><span class="sxs-lookup"><span data-stu-id="b8862-105">The presence of the **DeleteAction** resource on an [**itemActivity**][activity] indicates that the activity deleted an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="b8862-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b8862-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="b8862-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b8862-107">Properties</span></span>

| <span data-ttu-id="b8862-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="b8862-108">Property name</span></span> | <span data-ttu-id="b8862-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b8862-109">Type</span></span>   | <span data-ttu-id="b8862-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b8862-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="b8862-111">name</span><span class="sxs-lookup"><span data-stu-id="b8862-111">name</span></span>          | <span data-ttu-id="b8862-112">string</span><span class="sxs-lookup"><span data-stu-id="b8862-112">string</span></span> | <span data-ttu-id="b8862-113">Имя элемента, который был удален.</span><span class="sxs-lookup"><span data-stu-id="b8862-113">The name of the item that was deleted.</span></span>
| <span data-ttu-id="b8862-114">objectType</span><span class="sxs-lookup"><span data-stu-id="b8862-114">objectType</span></span>    | <span data-ttu-id="b8862-115">string</span><span class="sxs-lookup"><span data-stu-id="b8862-115">string</span></span> | <span data-ttu-id="b8862-116">`File` или `Folder` , в зависимости от типа удаленного элемента.</span><span class="sxs-lookup"><span data-stu-id="b8862-116">`File` or `Folder`, depending on the type of the deleted item.</span></span>

## <a name="remarks"></a><span data-ttu-id="b8862-117">Замечания</span><span class="sxs-lookup"><span data-stu-id="b8862-117">Remarks</span></span>

<span data-ttu-id="b8862-118">На данный момент записи о действиях над элементом доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="b8862-118">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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


