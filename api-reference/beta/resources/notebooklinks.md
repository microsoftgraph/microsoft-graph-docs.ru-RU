---
title: Тип ресурса notebookLinks
description: Ссылки для открытия записной книжки OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: da6896fccbea412fb29d88e02088dd7a52e25173
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956180"
---
# <a name="notebooklinks-resource-type"></a><span data-ttu-id="e3507-103">Тип ресурса notebookLinks</span><span class="sxs-lookup"><span data-stu-id="e3507-103">notebookLinks resource type</span></span>

> <span data-ttu-id="e3507-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e3507-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e3507-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3507-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e3507-106">Ссылки для открытия записной книжки OneNote.</span><span class="sxs-lookup"><span data-stu-id="e3507-106">Links for opening a OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e3507-107">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e3507-107">JSON representation</span></span>

<span data-ttu-id="e3507-108">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e3507-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="e3507-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="e3507-109">Properties</span></span>
| <span data-ttu-id="e3507-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="e3507-110">Property</span></span>     | <span data-ttu-id="e3507-111">Тип</span><span class="sxs-lookup"><span data-stu-id="e3507-111">Type</span></span>   |<span data-ttu-id="e3507-112">Описание</span><span class="sxs-lookup"><span data-stu-id="e3507-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e3507-113">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="e3507-113">oneNoteClientUrl</span></span>|[<span data-ttu-id="e3507-114">externalLink</span><span class="sxs-lookup"><span data-stu-id="e3507-114">externalLink</span></span>](externallink.md)|<span data-ttu-id="e3507-115">Открывает записную книжку в собственном клиенте OneNote, если он установлен.</span><span class="sxs-lookup"><span data-stu-id="e3507-115">Opens the notebook in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="e3507-116">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="e3507-116">oneNoteWebUrl</span></span>|[<span data-ttu-id="e3507-117">externalLink</span><span class="sxs-lookup"><span data-stu-id="e3507-117">externalLink</span></span>](externallink.md)|<span data-ttu-id="e3507-118">Открывает записную книжку в OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="e3507-118">Opens the notebook in OneNote Online.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "notebookLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
