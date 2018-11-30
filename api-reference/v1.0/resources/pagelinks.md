---
title: Тип ресурса pageLinks
description: Ссылки для открытия страницы OneNote.
ms.openlocfilehash: f1e4fe36d4356986bc88b744a9a62e28b8d368c5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024963"
---
# <a name="pagelinks-resource-type"></a><span data-ttu-id="d35cf-103">Тип ресурса pageLinks</span><span class="sxs-lookup"><span data-stu-id="d35cf-103">pageLinks resource type</span></span>

<span data-ttu-id="d35cf-104">Ссылки для открытия страницы OneNote.</span><span class="sxs-lookup"><span data-stu-id="d35cf-104">Links for opening a OneNote page.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d35cf-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="d35cf-105">JSON representation</span></span>

<span data-ttu-id="d35cf-106">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d35cf-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="d35cf-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="d35cf-107">Properties</span></span>
| <span data-ttu-id="d35cf-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="d35cf-108">Property</span></span>     | <span data-ttu-id="d35cf-109">Тип</span><span class="sxs-lookup"><span data-stu-id="d35cf-109">Type</span></span>   |<span data-ttu-id="d35cf-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d35cf-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d35cf-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="d35cf-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="d35cf-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="d35cf-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="d35cf-113">Открывает страницу в собственном клиенте OneNote (если он установлен).</span><span class="sxs-lookup"><span data-stu-id="d35cf-113">Opens the page in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="d35cf-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="d35cf-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="d35cf-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="d35cf-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="d35cf-116">Открывает страницу в OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="d35cf-116">Opens the page in OneNote Online.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "pageLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->