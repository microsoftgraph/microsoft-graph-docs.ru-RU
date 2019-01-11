---
title: Тип ресурса sectionLinks
description: Ссылки для открытия раздела OneNote.
localization_priority: Normal
ms.openlocfilehash: afc740aebc494aa6f204febbce1be4433005a4b1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839937"
---
# <a name="sectionlinks-resource-type"></a><span data-ttu-id="cc957-103">Тип ресурса sectionLinks</span><span class="sxs-lookup"><span data-stu-id="cc957-103">sectionLinks resource type</span></span>

<span data-ttu-id="cc957-104">Ссылки для открытия раздела OneNote.</span><span class="sxs-lookup"><span data-stu-id="cc957-104">Links for opening a OneNote section.</span></span>

## <a name="json-representation"></a><span data-ttu-id="cc957-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="cc957-105">JSON representation</span></span>

<span data-ttu-id="cc957-106">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cc957-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="cc957-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="cc957-107">Properties</span></span>
| <span data-ttu-id="cc957-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="cc957-108">Property</span></span>     | <span data-ttu-id="cc957-109">Тип</span><span class="sxs-lookup"><span data-stu-id="cc957-109">Type</span></span>   |<span data-ttu-id="cc957-110">Описание</span><span class="sxs-lookup"><span data-stu-id="cc957-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cc957-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="cc957-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="cc957-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="cc957-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="cc957-113">Открывает раздел в собственном клиенте OneNote (если он установлен).</span><span class="sxs-lookup"><span data-stu-id="cc957-113">Opens the section in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="cc957-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="cc957-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="cc957-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="cc957-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="cc957-116">Открывает раздел в OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="cc957-116">Opens the section in OneNote Online.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sectionLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
