---
title: Тип ресурса notebookLinks
description: Ссылки для открытия записной книжки OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: d3def81fb9bb3b7f657be3ed04230a65235db5f3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27984257"
---
# <a name="notebooklinks-resource-type"></a><span data-ttu-id="6ccec-103">Тип ресурса notebookLinks</span><span class="sxs-lookup"><span data-stu-id="6ccec-103">notebookLinks resource type</span></span>

<span data-ttu-id="6ccec-104">Ссылки для открытия записной книжки OneNote.</span><span class="sxs-lookup"><span data-stu-id="6ccec-104">Links for opening a OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6ccec-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="6ccec-105">JSON representation</span></span>

<span data-ttu-id="6ccec-106">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6ccec-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="6ccec-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="6ccec-107">Properties</span></span>
| <span data-ttu-id="6ccec-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="6ccec-108">Property</span></span>     | <span data-ttu-id="6ccec-109">Тип</span><span class="sxs-lookup"><span data-stu-id="6ccec-109">Type</span></span>   |<span data-ttu-id="6ccec-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6ccec-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6ccec-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="6ccec-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="6ccec-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="6ccec-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="6ccec-113">Открывает записную книжку в собственном клиенте OneNote, если он установлен.</span><span class="sxs-lookup"><span data-stu-id="6ccec-113">Opens the notebook in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="6ccec-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="6ccec-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="6ccec-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="6ccec-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="6ccec-116">Открывает записную книжку в OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="6ccec-116">Opens the notebook in OneNote Online.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "notebookLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
