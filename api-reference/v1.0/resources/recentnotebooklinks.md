---
title: Тип ресурса recentNotebookLinks
description: Ссылки для открытия записной книжки OneNote. Этот тип ресурса существует как свойство ресурса recentNotebook.
localization_priority: Normal
ms.openlocfilehash: 846047bd602d19cb4745e0a63f0326aaf7bfb512
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32579482"
---
# <a name="recentnotebooklinks-resource-type"></a><span data-ttu-id="b33dc-104">Тип ресурса recentNotebookLinks</span><span class="sxs-lookup"><span data-stu-id="b33dc-104">recentNotebookLinks resource type</span></span>

<span data-ttu-id="b33dc-105">Ссылки для открытия записной книжки OneNote.</span><span class="sxs-lookup"><span data-stu-id="b33dc-105">Links for opening a OneNote notebook.</span></span> <span data-ttu-id="b33dc-106">Этот тип ресурса существует как свойство ресурса [recentNotebook](recentnotebook.md).</span><span class="sxs-lookup"><span data-stu-id="b33dc-106">This resource type exists as a property on a [recentNotebook](recentnotebook.md) resource.</span></span>

## <a name="properties"></a><span data-ttu-id="b33dc-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b33dc-107">Properties</span></span>
| <span data-ttu-id="b33dc-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="b33dc-108">Property</span></span>     | <span data-ttu-id="b33dc-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b33dc-109">Type</span></span>   |<span data-ttu-id="b33dc-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b33dc-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b33dc-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="b33dc-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="b33dc-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="b33dc-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="b33dc-113">Открывает записную книжку в собственном клиенте OneNote, если он установлен.</span><span class="sxs-lookup"><span data-stu-id="b33dc-113">Opens the notebook in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="b33dc-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="b33dc-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="b33dc-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="b33dc-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="b33dc-116">Открывает записную книжку в OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="b33dc-116">Opens the notebook in OneNote Online.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b33dc-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b33dc-117">JSON representation</span></span>

<span data-ttu-id="b33dc-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b33dc-118">The following is a JSON representation of the resource.</span></span>

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
