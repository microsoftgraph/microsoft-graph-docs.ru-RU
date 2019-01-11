---
title: Тип ресурса recentNotebookLinks
description: Ссылки для открытия записной книжки OneNote. Этот тип ресурса существует как свойство ресурса recentNotebook.
localization_priority: Normal
ms.openlocfilehash: 846047bd602d19cb4745e0a63f0326aaf7bfb512
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810586"
---
# <a name="recentnotebooklinks-resource-type"></a><span data-ttu-id="0b0cc-104">Тип ресурса recentNotebookLinks</span><span class="sxs-lookup"><span data-stu-id="0b0cc-104">recentNotebookLinks resource type</span></span>

<span data-ttu-id="0b0cc-105">Ссылки для открытия записной книжки OneNote.</span><span class="sxs-lookup"><span data-stu-id="0b0cc-105">Links for opening a OneNote notebook.</span></span> <span data-ttu-id="0b0cc-106">Этот тип ресурса существует как свойство ресурса [recentNotebook](recentnotebook.md).</span><span class="sxs-lookup"><span data-stu-id="0b0cc-106">This resource type exists as a property on a [recentNotebook](recentnotebook.md) resource.</span></span>

## <a name="properties"></a><span data-ttu-id="0b0cc-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="0b0cc-107">Properties</span></span>
| <span data-ttu-id="0b0cc-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="0b0cc-108">Property</span></span>     | <span data-ttu-id="0b0cc-109">Тип</span><span class="sxs-lookup"><span data-stu-id="0b0cc-109">Type</span></span>   |<span data-ttu-id="0b0cc-110">Описание</span><span class="sxs-lookup"><span data-stu-id="0b0cc-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0b0cc-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="0b0cc-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="0b0cc-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="0b0cc-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="0b0cc-113">Открывает записную книжку в собственном клиенте OneNote, если он установлен.</span><span class="sxs-lookup"><span data-stu-id="0b0cc-113">Opens the notebook in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="0b0cc-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="0b0cc-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="0b0cc-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="0b0cc-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="0b0cc-116">Открывает записную книжку в OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="0b0cc-116">Opens the notebook in OneNote Online.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0b0cc-117">Описание в формате JSON</span><span class="sxs-lookup"><span data-stu-id="0b0cc-117">JSON representation</span></span>

<span data-ttu-id="0b0cc-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0b0cc-118">The following is a JSON representation of the resource.</span></span>

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
