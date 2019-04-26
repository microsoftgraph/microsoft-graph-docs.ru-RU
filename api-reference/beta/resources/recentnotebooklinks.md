---
title: Тип ресурса recentNotebookLinks
description: Ссылки для открытия записной книжки OneNote. Этот тип ресурса существует как свойство ресурса recentNotebook.
localization_priority: Normal
ms.openlocfilehash: c25ee3bc1e5096f7bbdf046090f8db9c0cc623fd
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343948"
---
# <a name="recentnotebooklinks-resource-type"></a><span data-ttu-id="bc85f-104">Тип ресурса recentNotebookLinks</span><span class="sxs-lookup"><span data-stu-id="bc85f-104">recentNotebookLinks resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bc85f-105">Ссылки для открытия записной книжки OneNote.</span><span class="sxs-lookup"><span data-stu-id="bc85f-105">Links to open a OneNote notebook.</span></span> <span data-ttu-id="bc85f-106">Этот тип ресурса существует как свойство ресурса [recentNotebook](recentnotebook.md).</span><span class="sxs-lookup"><span data-stu-id="bc85f-106">This resource type exists as a property on a [recentNotebook](recentnotebook.md) resource.</span></span>

## <a name="properties"></a><span data-ttu-id="bc85f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="bc85f-107">Properties</span></span>
| <span data-ttu-id="bc85f-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="bc85f-108">Property</span></span>     | <span data-ttu-id="bc85f-109">Тип</span><span class="sxs-lookup"><span data-stu-id="bc85f-109">Type</span></span>   |<span data-ttu-id="bc85f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="bc85f-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bc85f-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="bc85f-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="bc85f-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="bc85f-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="bc85f-113">Открывает записную книжку в клиенте OneNote, если она установлена.</span><span class="sxs-lookup"><span data-stu-id="bc85f-113">Opens the notebook in the OneNote client, if it's installed.</span></span>|
|<span data-ttu-id="bc85f-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="bc85f-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="bc85f-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="bc85f-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="bc85f-116">Открывает записную книжку в OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="bc85f-116">Opens the notebook in OneNote Online.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bc85f-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bc85f-117">JSON representation</span></span>

<span data-ttu-id="bc85f-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bc85f-118">The following is a JSON representation of the resource.</span></span>

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
