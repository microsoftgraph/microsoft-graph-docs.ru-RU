---
title: Тип ресурса pageLinks
description: Ссылки для открытия страницы OneNote.
localization_priority: Normal
ms.openlocfilehash: a5950366f6c6079443338b68db258c5762c15a7a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27872949"
---
# <a name="pagelinks-resource-type"></a><span data-ttu-id="8bb3d-103">Тип ресурса pageLinks</span><span class="sxs-lookup"><span data-stu-id="8bb3d-103">pageLinks resource type</span></span>

<span data-ttu-id="8bb3d-104">Ссылки для открытия страницы OneNote.</span><span class="sxs-lookup"><span data-stu-id="8bb3d-104">Links for opening a OneNote page.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8bb3d-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="8bb3d-105">JSON representation</span></span>

<span data-ttu-id="8bb3d-106">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8bb3d-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="8bb3d-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="8bb3d-107">Properties</span></span>
| <span data-ttu-id="8bb3d-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="8bb3d-108">Property</span></span>     | <span data-ttu-id="8bb3d-109">Тип</span><span class="sxs-lookup"><span data-stu-id="8bb3d-109">Type</span></span>   |<span data-ttu-id="8bb3d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8bb3d-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8bb3d-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="8bb3d-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="8bb3d-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="8bb3d-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="8bb3d-113">Открывает страницу в собственном клиенте OneNote (если он установлен).</span><span class="sxs-lookup"><span data-stu-id="8bb3d-113">Opens the page in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="8bb3d-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="8bb3d-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="8bb3d-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="8bb3d-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="8bb3d-116">Открывает страницу в OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="8bb3d-116">Opens the page in OneNote Online.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "pageLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
