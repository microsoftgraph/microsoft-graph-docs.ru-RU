---
title: Тип ресурса Сектионлинкс
description: Ссылки для открытия раздела OneNote.
localization_priority: Normal
ms.openlocfilehash: 2054e2a7a61d6c715146b51fb97c02516d8b638e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343425"
---
# <a name="sectionlinks-resource-type"></a><span data-ttu-id="1fcb6-103">Тип ресурса Сектионлинкс</span><span class="sxs-lookup"><span data-stu-id="1fcb6-103">sectionLinks resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1fcb6-104">Ссылки для открытия раздела OneNote.</span><span class="sxs-lookup"><span data-stu-id="1fcb6-104">Links for opening a OneNote section.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1fcb6-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1fcb6-105">JSON representation</span></span>

<span data-ttu-id="1fcb6-106">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1fcb6-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.sectionLinks"
}-->

```json
{
  "oneNoteClientUrl": {"@odata.type": "microsoft.graph.externalLink"},
  "oneNoteWebUrl": {"@odata.type": "microsoft.graph.externalLink"}
}

```
## <a name="properties"></a><span data-ttu-id="1fcb6-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="1fcb6-107">Properties</span></span>
| <span data-ttu-id="1fcb6-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="1fcb6-108">Property</span></span>     | <span data-ttu-id="1fcb6-109">Тип</span><span class="sxs-lookup"><span data-stu-id="1fcb6-109">Type</span></span>   |<span data-ttu-id="1fcb6-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1fcb6-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1fcb6-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="1fcb6-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="1fcb6-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="1fcb6-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="1fcb6-113">Открывает раздел в собственном клиенте OneNote, если он установлен.</span><span class="sxs-lookup"><span data-stu-id="1fcb6-113">Opens the section in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="1fcb6-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="1fcb6-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="1fcb6-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="1fcb6-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="1fcb6-116">Открывает раздел в OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="1fcb6-116">Opens the section in OneNote Online.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "sectionLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
