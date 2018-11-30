---
title: Тип ресурса recentNotebookLinks
description: Ссылки для открытия записной книжки OneNote. Этот тип ресурса существует как свойство ресурса recentNotebook.
ms.openlocfilehash: 594616a790becd77086177157f71321ffdd36e24
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025412"
---
# <a name="recentnotebooklinks-resource-type"></a><span data-ttu-id="974a5-104">Тип ресурса recentNotebookLinks</span><span class="sxs-lookup"><span data-stu-id="974a5-104">recentNotebookLinks resource type</span></span>

<span data-ttu-id="974a5-105">Ссылки для открытия записной книжки OneNote.</span><span class="sxs-lookup"><span data-stu-id="974a5-105">Links for opening a OneNote notebook.</span></span> <span data-ttu-id="974a5-106">Этот тип ресурса существует как свойство ресурса [recentNotebook](recentnotebook.md).</span><span class="sxs-lookup"><span data-stu-id="974a5-106">This resource type exists as a property on a [recentNotebook](recentnotebook.md) resource.</span></span>

## <a name="properties"></a><span data-ttu-id="974a5-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="974a5-107">Properties</span></span>
| <span data-ttu-id="974a5-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="974a5-108">Property</span></span>     | <span data-ttu-id="974a5-109">Тип</span><span class="sxs-lookup"><span data-stu-id="974a5-109">Type</span></span>   |<span data-ttu-id="974a5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="974a5-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="974a5-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="974a5-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="974a5-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="974a5-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="974a5-113">Открывает записную книжку в собственном клиенте OneNote, если он установлен.</span><span class="sxs-lookup"><span data-stu-id="974a5-113">Opens the notebook in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="974a5-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="974a5-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="974a5-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="974a5-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="974a5-116">Открывает записную книжку в OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="974a5-116">Opens the notebook in OneNote Online.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="974a5-117">Описание в формате JSON</span><span class="sxs-lookup"><span data-stu-id="974a5-117">JSON representation</span></span>

<span data-ttu-id="974a5-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="974a5-118">The following is a JSON representation of the resource.</span></span>

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
