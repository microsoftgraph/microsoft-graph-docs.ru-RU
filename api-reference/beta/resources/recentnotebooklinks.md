---
title: Тип ресурса recentNotebookLinks
description: Ссылки для открытия записной книжки OneNote. Этот тип ресурса существует как свойство ресурса recentNotebook.
localization_priority: Normal
ms.openlocfilehash: b68602f1fb8933f02e8f2c0957162d21a20d0e4b
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2019
ms.locfileid: "35236547"
---
# <a name="recentnotebooklinks-resource-type"></a><span data-ttu-id="753b9-104">Тип ресурса recentNotebookLinks</span><span class="sxs-lookup"><span data-stu-id="753b9-104">recentNotebookLinks resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="753b9-105">Ссылки для открытия записной книжки OneNote.</span><span class="sxs-lookup"><span data-stu-id="753b9-105">Links to open a OneNote notebook.</span></span> <span data-ttu-id="753b9-106">Этот тип ресурса существует как свойство ресурса [recentNotebook](recentnotebook.md).</span><span class="sxs-lookup"><span data-stu-id="753b9-106">This resource type exists as a property on a [recentNotebook](recentnotebook.md) resource.</span></span>

## <a name="properties"></a><span data-ttu-id="753b9-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="753b9-107">Properties</span></span>
| <span data-ttu-id="753b9-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="753b9-108">Property</span></span>     | <span data-ttu-id="753b9-109">Тип</span><span class="sxs-lookup"><span data-stu-id="753b9-109">Type</span></span>   |<span data-ttu-id="753b9-110">Описание</span><span class="sxs-lookup"><span data-stu-id="753b9-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="753b9-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="753b9-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="753b9-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="753b9-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="753b9-113">Открывает записную книжку в клиенте OneNote, если она установлена.</span><span class="sxs-lookup"><span data-stu-id="753b9-113">Opens the notebook in the OneNote client, if it's installed.</span></span>|
|<span data-ttu-id="753b9-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="753b9-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="753b9-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="753b9-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="753b9-116">Открывает записную книжку в OneNote в Интернете.</span><span class="sxs-lookup"><span data-stu-id="753b9-116">Opens the notebook in OneNote on the web.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="753b9-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="753b9-117">JSON representation</span></span>

<span data-ttu-id="753b9-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="753b9-118">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
