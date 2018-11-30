---
title: Тип ресурса externalLink
description: URL-адрес, который открывает страницу или записную книжку OneNote.
ms.openlocfilehash: 8f0af6b3bfd327dff0d228ea181443d742332d0f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078230"
---
# <a name="externallink-resource-type"></a><span data-ttu-id="cd29c-103">Тип ресурса externalLink</span><span class="sxs-lookup"><span data-stu-id="cd29c-103">externalLink resource type</span></span>

> <span data-ttu-id="cd29c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="cd29c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cd29c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd29c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cd29c-106">URL-адрес, который открывает страницу или записную книжку OneNote.</span><span class="sxs-lookup"><span data-stu-id="cd29c-106">A url that opens a OneNote page or notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="cd29c-107">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="cd29c-107">JSON representation</span></span>

<span data-ttu-id="cd29c-108">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="cd29c-108">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalLink"
}-->

```json
{
  "href": "string"
}

```
## <a name="properties"></a><span data-ttu-id="cd29c-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="cd29c-109">Properties</span></span>
| <span data-ttu-id="cd29c-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="cd29c-110">Property</span></span>     | <span data-ttu-id="cd29c-111">Тип</span><span class="sxs-lookup"><span data-stu-id="cd29c-111">Type</span></span>   |<span data-ttu-id="cd29c-112">Описание</span><span class="sxs-lookup"><span data-stu-id="cd29c-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cd29c-113">href</span><span class="sxs-lookup"><span data-stu-id="cd29c-113">href</span></span>|<span data-ttu-id="cd29c-114">Строка</span><span class="sxs-lookup"><span data-stu-id="cd29c-114">String</span></span>|<span data-ttu-id="cd29c-115">URL-адрес ссылки.</span><span class="sxs-lookup"><span data-stu-id="cd29c-115">The url of the link.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "externalLink resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->