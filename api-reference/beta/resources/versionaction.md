---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: VersionAction
localization_priority: Normal
ms.openlocfilehash: 59977b4ad84615f72dc008d671d64c62a2f4960f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345061"
---
# <a name="versionaction-resource-type"></a><span data-ttu-id="72ea1-102">Тип ресурса VersionAction</span><span class="sxs-lookup"><span data-stu-id="72ea1-102">VersionAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72ea1-103">Наличие ресурса **VersionAction** в ресурсе [**itemActivity**][activity] указывает, что в результате выполнения действия была создана другая версия.</span><span class="sxs-lookup"><span data-stu-id="72ea1-103">The presence of the **VersionAction** resource on an [**itemActivity**][activity] indicates that the activity caused a new version to be created.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="72ea1-104">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="72ea1-104">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.versionAction"
}-->

```json
{
  "newVersion": "string"
}
```

## <a name="properties"></a><span data-ttu-id="72ea1-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="72ea1-105">Properties</span></span>

| <span data-ttu-id="72ea1-106">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="72ea1-106">Property name</span></span> | <span data-ttu-id="72ea1-107">Тип</span><span class="sxs-lookup"><span data-stu-id="72ea1-107">Type</span></span>   | <span data-ttu-id="72ea1-108">Описание</span><span class="sxs-lookup"><span data-stu-id="72ea1-108">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="72ea1-109">newVersion</span><span class="sxs-lookup"><span data-stu-id="72ea1-109">newVersion</span></span>    | <span data-ttu-id="72ea1-110">string</span><span class="sxs-lookup"><span data-stu-id="72ea1-110">string</span></span> | <span data-ttu-id="72ea1-111">Имя новой версии, созданной при выполнении этого действия.</span><span class="sxs-lookup"><span data-stu-id="72ea1-111">The name of the new version that was created by this action.</span></span>

## <a name="remarks"></a><span data-ttu-id="72ea1-112">Замечания</span><span class="sxs-lookup"><span data-stu-id="72ea1-112">Remarks</span></span>

<span data-ttu-id="72ea1-113">На данный момент записи о действиях над элементом доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="72ea1-113">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The VersionAction object provides information about an activity that resulted in a new item version.",
  "keywords": "activities,activity,action,version",
  "section": "documentation",
  "tocPath": "Resources/VersionAction",
  "suppressions": []
}
-->
