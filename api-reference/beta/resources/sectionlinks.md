---
title: Тип ресурса Сектионлинкс
description: Ссылки для открытия раздела OneNote.
localization_priority: Normal
ms.openlocfilehash: 2c3744e08c492a8857600dc9e51dc205ae387bad
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2019
ms.locfileid: "35236512"
---
# <a name="sectionlinks-resource-type"></a><span data-ttu-id="915af-103">Тип ресурса Сектионлинкс</span><span class="sxs-lookup"><span data-stu-id="915af-103">sectionLinks resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="915af-104">Ссылки для открытия раздела OneNote.</span><span class="sxs-lookup"><span data-stu-id="915af-104">Links for opening a OneNote section.</span></span>

## <a name="json-representation"></a><span data-ttu-id="915af-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="915af-105">JSON representation</span></span>

<span data-ttu-id="915af-106">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="915af-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="915af-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="915af-107">Properties</span></span>
| <span data-ttu-id="915af-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="915af-108">Property</span></span>     | <span data-ttu-id="915af-109">Тип</span><span class="sxs-lookup"><span data-stu-id="915af-109">Type</span></span>   |<span data-ttu-id="915af-110">Описание</span><span class="sxs-lookup"><span data-stu-id="915af-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="915af-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="915af-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="915af-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="915af-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="915af-113">Открывает раздел в собственном клиенте OneNote, если он установлен.</span><span class="sxs-lookup"><span data-stu-id="915af-113">Opens the section in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="915af-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="915af-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="915af-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="915af-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="915af-116">Открывает раздел в OneNote в Интернете.</span><span class="sxs-lookup"><span data-stu-id="915af-116">Opens the section in OneNote on the web.</span></span>|

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
