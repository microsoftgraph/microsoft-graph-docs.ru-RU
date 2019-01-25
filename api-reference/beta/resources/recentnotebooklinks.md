---
title: Тип ресурса recentNotebookLinks
description: Ссылки на открытие записной книжке OneNote. Этот тип ресурса существует как свойство ресурса recentNotebook.
localization_priority: Normal
ms.openlocfilehash: 328f337d63645cdd52722a4216006920c493f9e7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525887"
---
# <a name="recentnotebooklinks-resource-type"></a><span data-ttu-id="4912e-104">Тип ресурса recentNotebookLinks</span><span class="sxs-lookup"><span data-stu-id="4912e-104">recentNotebookLinks resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4912e-105">Ссылки на открытие записной книжке OneNote.</span><span class="sxs-lookup"><span data-stu-id="4912e-105">Links to open a OneNote notebook.</span></span> <span data-ttu-id="4912e-106">Этот тип ресурса существует как свойство ресурса [recentNotebook](recentnotebook.md).</span><span class="sxs-lookup"><span data-stu-id="4912e-106">This resource type exists as a property on a [recentNotebook](recentnotebook.md) resource.</span></span>

## <a name="properties"></a><span data-ttu-id="4912e-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="4912e-107">Properties</span></span>
| <span data-ttu-id="4912e-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="4912e-108">Property</span></span>     | <span data-ttu-id="4912e-109">Тип</span><span class="sxs-lookup"><span data-stu-id="4912e-109">Type</span></span>   |<span data-ttu-id="4912e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4912e-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4912e-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="4912e-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="4912e-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="4912e-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="4912e-113">Открывает записную книжку в клиент OneNote, если она установлена.</span><span class="sxs-lookup"><span data-stu-id="4912e-113">Opens the notebook in the OneNote client, if it's installed.</span></span>|
|<span data-ttu-id="4912e-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="4912e-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="4912e-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="4912e-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="4912e-116">Открывает записную книжку в OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="4912e-116">Opens the notebook in OneNote Online.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4912e-117">Описание в формате JSON</span><span class="sxs-lookup"><span data-stu-id="4912e-117">JSON representation</span></span>

<span data-ttu-id="4912e-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4912e-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recentNotebookLinks"
}-->

```json
{
  "oneNoteClientUrl": {"@odata.type": "microsoft.graph.externalLink"},
  "oneNoteWebUrl": {"@odata.type": "microsoft.graph.externalLink"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "recentNotebookLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/recentnotebooklinks.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
