---
title: Тип ресурса sectionLinks
description: Ссылки для открытия раздела OneNote.
localization_priority: Normal
ms.openlocfilehash: 190842708979d62430a4716a8785fd40309cb189
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858942"
---
# <a name="sectionlinks-resource-type"></a><span data-ttu-id="a3c0b-103">Тип ресурса sectionLinks</span><span class="sxs-lookup"><span data-stu-id="a3c0b-103">sectionLinks resource type</span></span>

> <span data-ttu-id="a3c0b-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a3c0b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a3c0b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3c0b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a3c0b-106">Ссылки для открытия раздела OneNote.</span><span class="sxs-lookup"><span data-stu-id="a3c0b-106">Links for opening a OneNote section.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a3c0b-107">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="a3c0b-107">JSON representation</span></span>

<span data-ttu-id="a3c0b-108">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a3c0b-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="a3c0b-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="a3c0b-109">Properties</span></span>
| <span data-ttu-id="a3c0b-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="a3c0b-110">Property</span></span>     | <span data-ttu-id="a3c0b-111">Тип</span><span class="sxs-lookup"><span data-stu-id="a3c0b-111">Type</span></span>   |<span data-ttu-id="a3c0b-112">Описание</span><span class="sxs-lookup"><span data-stu-id="a3c0b-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a3c0b-113">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="a3c0b-113">oneNoteClientUrl</span></span>|[<span data-ttu-id="a3c0b-114">externalLink</span><span class="sxs-lookup"><span data-stu-id="a3c0b-114">externalLink</span></span>](externallink.md)|<span data-ttu-id="a3c0b-115">Открывает раздел в собственном клиенте OneNote (если он установлен).</span><span class="sxs-lookup"><span data-stu-id="a3c0b-115">Opens the section in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="a3c0b-116">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="a3c0b-116">oneNoteWebUrl</span></span>|[<span data-ttu-id="a3c0b-117">externalLink</span><span class="sxs-lookup"><span data-stu-id="a3c0b-117">externalLink</span></span>](externallink.md)|<span data-ttu-id="a3c0b-118">Открывает раздел в OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="a3c0b-118">Opens the section in OneNote Online.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sectionLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
