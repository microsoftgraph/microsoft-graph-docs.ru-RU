---
title: Тип ресурса recentNotebookLinks
description: Ссылки для открытия записной книжки OneNote. Этот тип ресурса существует как свойство ресурса recentNotebook.
localization_priority: Normal
ms.openlocfilehash: 7a906d0ece395aec191702bcd1b27d2cbea01af2
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2019
ms.locfileid: "35236680"
---
# <a name="recentnotebooklinks-resource-type"></a><span data-ttu-id="4fadf-104">Тип ресурса recentNotebookLinks</span><span class="sxs-lookup"><span data-stu-id="4fadf-104">recentNotebookLinks resource type</span></span>

<span data-ttu-id="4fadf-105">Ссылки для открытия записной книжки OneNote.</span><span class="sxs-lookup"><span data-stu-id="4fadf-105">Links for opening a OneNote notebook.</span></span> <span data-ttu-id="4fadf-106">Этот тип ресурса существует как свойство ресурса [recentNotebook](recentnotebook.md).</span><span class="sxs-lookup"><span data-stu-id="4fadf-106">This resource type exists as a property on a [recentNotebook](recentnotebook.md) resource.</span></span>

## <a name="properties"></a><span data-ttu-id="4fadf-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="4fadf-107">Properties</span></span>
| <span data-ttu-id="4fadf-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="4fadf-108">Property</span></span>     | <span data-ttu-id="4fadf-109">Тип</span><span class="sxs-lookup"><span data-stu-id="4fadf-109">Type</span></span>   |<span data-ttu-id="4fadf-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4fadf-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4fadf-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="4fadf-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="4fadf-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="4fadf-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="4fadf-113">Открывает записную книжку в собственном клиенте OneNote, если он установлен.</span><span class="sxs-lookup"><span data-stu-id="4fadf-113">Opens the notebook in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="4fadf-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="4fadf-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="4fadf-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="4fadf-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="4fadf-116">Открывает записную книжку в OneNote в Интернете.</span><span class="sxs-lookup"><span data-stu-id="4fadf-116">Opens the notebook in OneNote on the web.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4fadf-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4fadf-117">JSON representation</span></span>

<span data-ttu-id="4fadf-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4fadf-118">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "recentNotebookLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
