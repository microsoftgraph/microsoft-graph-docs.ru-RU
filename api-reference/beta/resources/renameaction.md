---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: RenameAction
localization_priority: Normal
ms.openlocfilehash: bc731a94167e16518c8dd9eaea7deabd5f519f7b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563112"
---
# <a name="renameaction-resource-type"></a><span data-ttu-id="1b10c-102">Тип ресурса RenameAction</span><span class="sxs-lookup"><span data-stu-id="1b10c-102">RenameAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1b10c-103">Наличие ресурса **RenameAction** в ресурсе [**itemActivity**][activity] указывает, что в результате выполнения действия элемент был переименован.</span><span class="sxs-lookup"><span data-stu-id="1b10c-103">The presence of the **RenameAction** resource on an [**itemActivity**][activity] indicates that the activity renamed an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="1b10c-104">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="1b10c-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="1b10c-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="1b10c-105">Properties</span></span>

| <span data-ttu-id="1b10c-106">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="1b10c-106">Property name</span></span> | <span data-ttu-id="1b10c-107">Тип</span><span class="sxs-lookup"><span data-stu-id="1b10c-107">Type</span></span>   | <span data-ttu-id="1b10c-108">Описание</span><span class="sxs-lookup"><span data-stu-id="1b10c-108">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="1b10c-109">oldName</span><span class="sxs-lookup"><span data-stu-id="1b10c-109">oldName</span></span>       | <span data-ttu-id="1b10c-110">string</span><span class="sxs-lookup"><span data-stu-id="1b10c-110">string</span></span> | <span data-ttu-id="1b10c-111">Предыдущее имя элемента.</span><span class="sxs-lookup"><span data-stu-id="1b10c-111">The previous name of the item.</span></span>
| <span data-ttu-id="1b10c-112">Новое</span><span class="sxs-lookup"><span data-stu-id="1b10c-112">newName</span></span>       | <span data-ttu-id="1b10c-113">string</span><span class="sxs-lookup"><span data-stu-id="1b10c-113">string</span></span> | <span data-ttu-id="1b10c-114">Новое имя элемента.</span><span class="sxs-lookup"><span data-stu-id="1b10c-114">The new name of the item.</span></span>

## <a name="remarks"></a><span data-ttu-id="1b10c-115">Замечания</span><span class="sxs-lookup"><span data-stu-id="1b10c-115">Remarks</span></span>

<span data-ttu-id="1b10c-116">На данный момент записи о действиях над элементом доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="1b10c-116">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The RenameAction object provides information about an activity that renamed an item.",
  "keywords": "activities,activity,action,rename,renamed",
  "section": "documentation",
  "tocPath": "Resources/RenameAction",
  "suppressions": [
    "Error: /api-reference/beta/resources/renameaction.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
