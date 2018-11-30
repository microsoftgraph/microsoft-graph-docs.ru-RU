---
title: Тип ресурса pageLinks
description: Ссылки для открытия страницы OneNote.
ms.openlocfilehash: 598e39f5cf2b6bbd722b07b72f4fa63ad7fd8302
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081599"
---
# <a name="pagelinks-resource-type"></a><span data-ttu-id="d4612-103">Тип ресурса pageLinks</span><span class="sxs-lookup"><span data-stu-id="d4612-103">pageLinks resource type</span></span>

> <span data-ttu-id="d4612-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d4612-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d4612-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4612-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d4612-106">Ссылки для открытия страницы OneNote.</span><span class="sxs-lookup"><span data-stu-id="d4612-106">Links for opening a OneNote page.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d4612-107">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="d4612-107">JSON representation</span></span>

<span data-ttu-id="d4612-108">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d4612-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="d4612-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="d4612-109">Properties</span></span>
| <span data-ttu-id="d4612-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="d4612-110">Property</span></span>     | <span data-ttu-id="d4612-111">Тип</span><span class="sxs-lookup"><span data-stu-id="d4612-111">Type</span></span>   |<span data-ttu-id="d4612-112">Описание</span><span class="sxs-lookup"><span data-stu-id="d4612-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d4612-113">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="d4612-113">oneNoteClientUrl</span></span>|[<span data-ttu-id="d4612-114">externalLink</span><span class="sxs-lookup"><span data-stu-id="d4612-114">externalLink</span></span>](externallink.md)|<span data-ttu-id="d4612-115">Открывает страницу в собственном клиенте OneNote (если он установлен).</span><span class="sxs-lookup"><span data-stu-id="d4612-115">Opens the page in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="d4612-116">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="d4612-116">oneNoteWebUrl</span></span>|[<span data-ttu-id="d4612-117">externalLink</span><span class="sxs-lookup"><span data-stu-id="d4612-117">externalLink</span></span>](externallink.md)|<span data-ttu-id="d4612-118">Открывает страницу в OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="d4612-118">Opens the page in OneNote Online.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "pageLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->