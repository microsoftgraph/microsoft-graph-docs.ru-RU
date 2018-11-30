---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: RenameAction
ms.openlocfilehash: 12956ab51923f6d9f175b25203bf2921a64a8a6b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078145"
---
# <a name="renameaction-resource-type"></a><span data-ttu-id="c2e71-102">Тип ресурса RenameAction</span><span class="sxs-lookup"><span data-stu-id="c2e71-102">RenameAction resource type</span></span>

> <span data-ttu-id="c2e71-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c2e71-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c2e71-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2e71-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c2e71-105">Наличие ресурса **RenameAction** в ресурсе [**itemActivity**][activity] указывает, что в результате выполнения действия элемент был переименован.</span><span class="sxs-lookup"><span data-stu-id="c2e71-105">The presence of the **RenameAction** resource on an [**itemActivity**][activity] indicates that the activity renamed an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="c2e71-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c2e71-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="c2e71-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="c2e71-107">Properties</span></span>

| <span data-ttu-id="c2e71-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="c2e71-108">Property name</span></span> | <span data-ttu-id="c2e71-109">Тип</span><span class="sxs-lookup"><span data-stu-id="c2e71-109">Type</span></span>   | <span data-ttu-id="c2e71-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c2e71-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="c2e71-111">oldName</span><span class="sxs-lookup"><span data-stu-id="c2e71-111">oldName</span></span>       | <span data-ttu-id="c2e71-112">string</span><span class="sxs-lookup"><span data-stu-id="c2e71-112">string</span></span> | <span data-ttu-id="c2e71-113">Предыдущее имя элемента.</span><span class="sxs-lookup"><span data-stu-id="c2e71-113">The previous name of the item.</span></span>
| <span data-ttu-id="c2e71-114">параметр newName</span><span class="sxs-lookup"><span data-stu-id="c2e71-114">newName</span></span>       | <span data-ttu-id="c2e71-115">string</span><span class="sxs-lookup"><span data-stu-id="c2e71-115">string</span></span> | <span data-ttu-id="c2e71-116">Новое имя элемента.</span><span class="sxs-lookup"><span data-stu-id="c2e71-116">The new name of the item.</span></span>

## <a name="remarks"></a><span data-ttu-id="c2e71-117">Замечания</span><span class="sxs-lookup"><span data-stu-id="c2e71-117">Remarks</span></span>

<span data-ttu-id="c2e71-118">На данный момент записи о действиях над элементом доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="c2e71-118">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The RenameAction object provides information about an activity that renamed an item.",
  "keywords": "activities,activity,action,rename,renamed",
  "section": "documentation",
  "tocPath": "Resources/RenameAction"
} -->
