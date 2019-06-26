---
title: Тип ресурса Пажелинкс
description: Ссылки для открытия страницы OneNote.
localization_priority: Normal
ms.openlocfilehash: 54121a6232ae02d12571f925909be5b92a2bb0cd
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2019
ms.locfileid: "35236610"
---
# <a name="pagelinks-resource-type"></a><span data-ttu-id="1e297-103">Тип ресурса Пажелинкс</span><span class="sxs-lookup"><span data-stu-id="1e297-103">pageLinks resource type</span></span>

<span data-ttu-id="1e297-104">Ссылки для открытия страницы OneNote.</span><span class="sxs-lookup"><span data-stu-id="1e297-104">Links for opening a OneNote page.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1e297-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1e297-105">JSON representation</span></span>

<span data-ttu-id="1e297-106">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1e297-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="1e297-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="1e297-107">Properties</span></span>
| <span data-ttu-id="1e297-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="1e297-108">Property</span></span>     | <span data-ttu-id="1e297-109">Тип</span><span class="sxs-lookup"><span data-stu-id="1e297-109">Type</span></span>   |<span data-ttu-id="1e297-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1e297-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1e297-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="1e297-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="1e297-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="1e297-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="1e297-113">Открывает страницу в собственном клиенте OneNote, если она установлена.</span><span class="sxs-lookup"><span data-stu-id="1e297-113">Opens the page in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="1e297-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="1e297-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="1e297-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="1e297-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="1e297-116">Открывает страницу в OneNote в Интернете.</span><span class="sxs-lookup"><span data-stu-id="1e297-116">Opens the page in OneNote on the web.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "pageLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
