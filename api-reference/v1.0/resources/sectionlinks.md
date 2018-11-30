---
title: Тип ресурса sectionLinks
description: Ссылки для открытия раздела OneNote.
ms.openlocfilehash: 4ca6221992c75f410839538d8080c084c8486903
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025459"
---
# <a name="sectionlinks-resource-type"></a><span data-ttu-id="082f7-103">Тип ресурса sectionLinks</span><span class="sxs-lookup"><span data-stu-id="082f7-103">sectionLinks resource type</span></span>

<span data-ttu-id="082f7-104">Ссылки для открытия раздела OneNote.</span><span class="sxs-lookup"><span data-stu-id="082f7-104">Links for opening a OneNote section.</span></span>

## <a name="json-representation"></a><span data-ttu-id="082f7-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="082f7-105">JSON representation</span></span>

<span data-ttu-id="082f7-106">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="082f7-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="082f7-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="082f7-107">Properties</span></span>
| <span data-ttu-id="082f7-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="082f7-108">Property</span></span>     | <span data-ttu-id="082f7-109">Тип</span><span class="sxs-lookup"><span data-stu-id="082f7-109">Type</span></span>   |<span data-ttu-id="082f7-110">Описание</span><span class="sxs-lookup"><span data-stu-id="082f7-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="082f7-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="082f7-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="082f7-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="082f7-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="082f7-113">Открывает раздел в собственном клиенте OneNote (если он установлен).</span><span class="sxs-lookup"><span data-stu-id="082f7-113">Opens the section in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="082f7-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="082f7-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="082f7-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="082f7-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="082f7-116">Открывает раздел в OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="082f7-116">Opens the section in OneNote Online.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sectionLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->