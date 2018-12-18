---
title: Тип ресурса notebookLinks
description: Ссылки для открытия записной книжки OneNote.
author: Jewan-microsoft
ms.openlocfilehash: f263a255199dea844f62d322b4be010111c9c823
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27357178"
---
# <a name="notebooklinks-resource-type"></a><span data-ttu-id="fbbe9-103">Тип ресурса notebookLinks</span><span class="sxs-lookup"><span data-stu-id="fbbe9-103">notebookLinks resource type</span></span>

<span data-ttu-id="fbbe9-104">Ссылки для открытия записной книжки OneNote.</span><span class="sxs-lookup"><span data-stu-id="fbbe9-104">Links for opening a OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fbbe9-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="fbbe9-105">JSON representation</span></span>

<span data-ttu-id="fbbe9-106">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fbbe9-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.notebookLinks"
}-->

```json
{
  "oneNoteClientUrl": {"@odata.type": "microsoft.graph.externalLink"},
  "oneNoteWebUrl": {"@odata.type": "microsoft.graph.externalLink"}
}

```
## <a name="properties"></a><span data-ttu-id="fbbe9-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="fbbe9-107">Properties</span></span>
| <span data-ttu-id="fbbe9-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="fbbe9-108">Property</span></span>     | <span data-ttu-id="fbbe9-109">Тип</span><span class="sxs-lookup"><span data-stu-id="fbbe9-109">Type</span></span>   |<span data-ttu-id="fbbe9-110">Описание</span><span class="sxs-lookup"><span data-stu-id="fbbe9-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fbbe9-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="fbbe9-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="fbbe9-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="fbbe9-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="fbbe9-113">Открывает записную книжку в собственном клиенте OneNote, если он установлен.</span><span class="sxs-lookup"><span data-stu-id="fbbe9-113">Opens the notebook in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="fbbe9-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="fbbe9-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="fbbe9-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="fbbe9-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="fbbe9-116">Открывает записную книжку в OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="fbbe9-116">Opens the notebook in OneNote Online.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "notebookLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->