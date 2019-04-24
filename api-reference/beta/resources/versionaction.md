---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: VersionAction
localization_priority: Normal
ms.openlocfilehash: c65b3cf021321a7e021c5fa4193abdcdce6c635a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32453858"
---
# <a name="versionaction-resource-type"></a><span data-ttu-id="27335-102">Тип ресурса VersionAction</span><span class="sxs-lookup"><span data-stu-id="27335-102">VersionAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="27335-103">Наличие ресурса **VersionAction** в ресурсе [**itemActivity**][activity] указывает, что в результате выполнения действия была создана другая версия.</span><span class="sxs-lookup"><span data-stu-id="27335-103">The presence of the **VersionAction** resource on an [**itemActivity**][activity] indicates that the activity caused a new version to be created.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="27335-104">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="27335-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="27335-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="27335-105">Properties</span></span>

| <span data-ttu-id="27335-106">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="27335-106">Property name</span></span> | <span data-ttu-id="27335-107">Тип</span><span class="sxs-lookup"><span data-stu-id="27335-107">Type</span></span>   | <span data-ttu-id="27335-108">Описание</span><span class="sxs-lookup"><span data-stu-id="27335-108">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="27335-109">newVersion</span><span class="sxs-lookup"><span data-stu-id="27335-109">newVersion</span></span>    | <span data-ttu-id="27335-110">string</span><span class="sxs-lookup"><span data-stu-id="27335-110">string</span></span> | <span data-ttu-id="27335-111">Имя новой версии, созданной при выполнении этого действия.</span><span class="sxs-lookup"><span data-stu-id="27335-111">The name of the new version that was created by this action.</span></span>

## <a name="remarks"></a><span data-ttu-id="27335-112">Замечания</span><span class="sxs-lookup"><span data-stu-id="27335-112">Remarks</span></span>

<span data-ttu-id="27335-113">На данный момент записи о действиях над элементом доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="27335-113">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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
