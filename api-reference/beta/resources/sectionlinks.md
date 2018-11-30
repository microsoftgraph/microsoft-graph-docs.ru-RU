---
title: Тип ресурса sectionLinks
description: Ссылки для открытия раздела OneNote.
ms.openlocfilehash: 26dbffd6f3bde9c05efabc737852c3619cc1e275
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080132"
---
# <a name="sectionlinks-resource-type"></a><span data-ttu-id="c105f-103">Тип ресурса sectionLinks</span><span class="sxs-lookup"><span data-stu-id="c105f-103">sectionLinks resource type</span></span>

> <span data-ttu-id="c105f-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c105f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c105f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c105f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c105f-106">Ссылки для открытия раздела OneNote.</span><span class="sxs-lookup"><span data-stu-id="c105f-106">Links for opening a OneNote section.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c105f-107">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c105f-107">JSON representation</span></span>

<span data-ttu-id="c105f-108">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c105f-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="c105f-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="c105f-109">Properties</span></span>
| <span data-ttu-id="c105f-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="c105f-110">Property</span></span>     | <span data-ttu-id="c105f-111">Тип</span><span class="sxs-lookup"><span data-stu-id="c105f-111">Type</span></span>   |<span data-ttu-id="c105f-112">Описание</span><span class="sxs-lookup"><span data-stu-id="c105f-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c105f-113">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="c105f-113">oneNoteClientUrl</span></span>|[<span data-ttu-id="c105f-114">externalLink</span><span class="sxs-lookup"><span data-stu-id="c105f-114">externalLink</span></span>](externallink.md)|<span data-ttu-id="c105f-115">Открывает раздел в собственном клиенте OneNote (если он установлен).</span><span class="sxs-lookup"><span data-stu-id="c105f-115">Opens the section in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="c105f-116">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="c105f-116">oneNoteWebUrl</span></span>|[<span data-ttu-id="c105f-117">externalLink</span><span class="sxs-lookup"><span data-stu-id="c105f-117">externalLink</span></span>](externallink.md)|<span data-ttu-id="c105f-118">Открывает раздел в OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="c105f-118">Opens the section in OneNote Online.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sectionLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->