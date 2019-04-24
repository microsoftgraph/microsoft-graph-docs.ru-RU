---
title: Тип ресурса Пажелинкс
description: Ссылки для открытия страницы OneNote.
localization_priority: Normal
ms.openlocfilehash: a5950366f6c6079443338b68db258c5762c15a7a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462510"
---
# <a name="pagelinks-resource-type"></a><span data-ttu-id="a86a7-103">Тип ресурса Пажелинкс</span><span class="sxs-lookup"><span data-stu-id="a86a7-103">pageLinks resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a86a7-104">Ссылки для открытия страницы OneNote.</span><span class="sxs-lookup"><span data-stu-id="a86a7-104">Links for opening a OneNote page.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a86a7-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a86a7-105">JSON representation</span></span>

<span data-ttu-id="a86a7-106">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a86a7-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.pageLinks"
}-->

```json
{
  "oneNoteClientUrl": {"@odata.type": "microsoft.graph.externalLink"},
  "oneNoteWebUrl": {"@odata.type": "microsoft.graph.externalLink"}
}

```
## <a name="properties"></a><span data-ttu-id="a86a7-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="a86a7-107">Properties</span></span>
| <span data-ttu-id="a86a7-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="a86a7-108">Property</span></span>     | <span data-ttu-id="a86a7-109">Тип</span><span class="sxs-lookup"><span data-stu-id="a86a7-109">Type</span></span>   |<span data-ttu-id="a86a7-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a86a7-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a86a7-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="a86a7-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="a86a7-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="a86a7-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="a86a7-113">Открывает страницу в собственном клиенте OneNote, если она установлена.</span><span class="sxs-lookup"><span data-stu-id="a86a7-113">Opens the page in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="a86a7-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="a86a7-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="a86a7-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="a86a7-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="a86a7-116">Открывает страницу в OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="a86a7-116">Opens the page in OneNote Online.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "pageLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/pagelinks.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
