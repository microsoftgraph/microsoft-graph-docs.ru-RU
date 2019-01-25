---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: VersionAction
localization_priority: Normal
ms.openlocfilehash: c65b3cf021321a7e021c5fa4193abdcdce6c635a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520608"
---
# <a name="versionaction-resource-type"></a><span data-ttu-id="7c7f9-102">Тип ресурса VersionAction</span><span class="sxs-lookup"><span data-stu-id="7c7f9-102">VersionAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7c7f9-103">Наличие ресурса **VersionAction** в ресурсе [**itemActivity**][activity] указывает, что в результате выполнения действия была создана другая версия.</span><span class="sxs-lookup"><span data-stu-id="7c7f9-103">The presence of the **VersionAction** resource on an [**itemActivity**][activity] indicates that the activity caused a new version to be created.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="7c7f9-104">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="7c7f9-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="7c7f9-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="7c7f9-105">Properties</span></span>

| <span data-ttu-id="7c7f9-106">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="7c7f9-106">Property name</span></span> | <span data-ttu-id="7c7f9-107">Тип</span><span class="sxs-lookup"><span data-stu-id="7c7f9-107">Type</span></span>   | <span data-ttu-id="7c7f9-108">Описание</span><span class="sxs-lookup"><span data-stu-id="7c7f9-108">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="7c7f9-109">newVersion</span><span class="sxs-lookup"><span data-stu-id="7c7f9-109">newVersion</span></span>    | <span data-ttu-id="7c7f9-110">string</span><span class="sxs-lookup"><span data-stu-id="7c7f9-110">string</span></span> | <span data-ttu-id="7c7f9-111">Имя новой версии, созданной при выполнении этого действия.</span><span class="sxs-lookup"><span data-stu-id="7c7f9-111">The name of the new version that was created by this action.</span></span>

## <a name="remarks"></a><span data-ttu-id="7c7f9-112">Замечания</span><span class="sxs-lookup"><span data-stu-id="7c7f9-112">Remarks</span></span>

<span data-ttu-id="7c7f9-113">На данный момент записи о действиях над элементом доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="7c7f9-113">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The VersionAction object provides information about an activity that resulted in a new item version.",
  "keywords": "activities,activity,action,version",
  "section": "documentation",
  "tocPath": "Resources/VersionAction",
  "suppressions": [
    "Error: /api-reference/beta/resources/versionaction.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
