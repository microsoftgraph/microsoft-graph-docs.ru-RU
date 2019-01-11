---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: RenameAction
localization_priority: Normal
ms.openlocfilehash: 88fa2738c014f028ebd2cc6e37f83151c7fc984a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27835709"
---
# <a name="renameaction-resource-type"></a><span data-ttu-id="f6d2b-102">Тип ресурса RenameAction</span><span class="sxs-lookup"><span data-stu-id="f6d2b-102">RenameAction resource type</span></span>

> <span data-ttu-id="f6d2b-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f6d2b-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f6d2b-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6d2b-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f6d2b-105">Наличие ресурса **RenameAction** в ресурсе [**itemActivity**][activity] указывает, что в результате выполнения действия элемент был переименован.</span><span class="sxs-lookup"><span data-stu-id="f6d2b-105">The presence of the **RenameAction** resource on an [**itemActivity**][activity] indicates that the activity renamed an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="f6d2b-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="f6d2b-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="f6d2b-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f6d2b-107">Properties</span></span>

| <span data-ttu-id="f6d2b-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="f6d2b-108">Property name</span></span> | <span data-ttu-id="f6d2b-109">Тип</span><span class="sxs-lookup"><span data-stu-id="f6d2b-109">Type</span></span>   | <span data-ttu-id="f6d2b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f6d2b-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="f6d2b-111">oldName</span><span class="sxs-lookup"><span data-stu-id="f6d2b-111">oldName</span></span>       | <span data-ttu-id="f6d2b-112">string</span><span class="sxs-lookup"><span data-stu-id="f6d2b-112">string</span></span> | <span data-ttu-id="f6d2b-113">Предыдущее имя элемента.</span><span class="sxs-lookup"><span data-stu-id="f6d2b-113">The previous name of the item.</span></span>
| <span data-ttu-id="f6d2b-114">параметр newName</span><span class="sxs-lookup"><span data-stu-id="f6d2b-114">newName</span></span>       | <span data-ttu-id="f6d2b-115">string</span><span class="sxs-lookup"><span data-stu-id="f6d2b-115">string</span></span> | <span data-ttu-id="f6d2b-116">Новое имя элемента.</span><span class="sxs-lookup"><span data-stu-id="f6d2b-116">The new name of the item.</span></span>

## <a name="remarks"></a><span data-ttu-id="f6d2b-117">Замечания</span><span class="sxs-lookup"><span data-stu-id="f6d2b-117">Remarks</span></span>

<span data-ttu-id="f6d2b-118">На данный момент записи о действиях над элементом доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="f6d2b-118">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The RenameAction object provides information about an activity that renamed an item.",
  "keywords": "activities,activity,action,rename,renamed",
  "section": "documentation",
  "tocPath": "Resources/RenameAction"
} -->
