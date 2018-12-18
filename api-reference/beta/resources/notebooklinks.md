---
title: Тип ресурса notebookLinks
description: Ссылки для открытия записной книжки OneNote.
author: Jewan-microsoft
ms.openlocfilehash: 88ad146dc4b1499882a2605605c5bb725b6ed531
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27345236"
---
# <a name="notebooklinks-resource-type"></a><span data-ttu-id="4fafa-103">Тип ресурса notebookLinks</span><span class="sxs-lookup"><span data-stu-id="4fafa-103">notebookLinks resource type</span></span>

> <span data-ttu-id="4fafa-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4fafa-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4fafa-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4fafa-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4fafa-106">Ссылки для открытия записной книжки OneNote.</span><span class="sxs-lookup"><span data-stu-id="4fafa-106">Links for opening a OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4fafa-107">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="4fafa-107">JSON representation</span></span>

<span data-ttu-id="4fafa-108">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4fafa-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="4fafa-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="4fafa-109">Properties</span></span>
| <span data-ttu-id="4fafa-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="4fafa-110">Property</span></span>     | <span data-ttu-id="4fafa-111">Тип</span><span class="sxs-lookup"><span data-stu-id="4fafa-111">Type</span></span>   |<span data-ttu-id="4fafa-112">Описание</span><span class="sxs-lookup"><span data-stu-id="4fafa-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4fafa-113">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="4fafa-113">oneNoteClientUrl</span></span>|[<span data-ttu-id="4fafa-114">externalLink</span><span class="sxs-lookup"><span data-stu-id="4fafa-114">externalLink</span></span>](externallink.md)|<span data-ttu-id="4fafa-115">Открывает записную книжку в собственном клиенте OneNote, если он установлен.</span><span class="sxs-lookup"><span data-stu-id="4fafa-115">Opens the notebook in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="4fafa-116">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="4fafa-116">oneNoteWebUrl</span></span>|[<span data-ttu-id="4fafa-117">externalLink</span><span class="sxs-lookup"><span data-stu-id="4fafa-117">externalLink</span></span>](externallink.md)|<span data-ttu-id="4fafa-118">Открывает записную книжку в OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="4fafa-118">Opens the notebook in OneNote Online.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "notebookLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->