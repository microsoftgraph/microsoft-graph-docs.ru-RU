---
title: Тип ресурса freeBusyError
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
ms.openlocfilehash: d1bf6671d6c506d9959fcd5abc8843c1a08c924b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080874"
---
# <a name="freebusyerror-resource-type"></a><span data-ttu-id="e7571-104">Тип ресурса freeBusyError</span><span class="sxs-lookup"><span data-stu-id="e7571-104">freeBusyError resource type</span></span>

 > <span data-ttu-id="e7571-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e7571-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e7571-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7571-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="e7571-107">Представляет сведения об ошибке при попытке получить доступности пользователя, ресурса или список рассылки.</span><span class="sxs-lookup"><span data-stu-id="e7571-107">Represents error information from attempting to get the availability of a user, distribution list, or resource.</span></span>

## <a name="properties"></a><span data-ttu-id="e7571-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="e7571-108">Properties</span></span>
| <span data-ttu-id="e7571-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="e7571-109">Property</span></span>     | <span data-ttu-id="e7571-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e7571-110">Type</span></span>   |<span data-ttu-id="e7571-111">Description</span><span class="sxs-lookup"><span data-stu-id="e7571-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e7571-112">message</span><span class="sxs-lookup"><span data-stu-id="e7571-112">message</span></span> |<span data-ttu-id="e7571-113">String</span><span class="sxs-lookup"><span data-stu-id="e7571-113">String</span></span> |<span data-ttu-id="e7571-114">Описание ошибки.</span><span class="sxs-lookup"><span data-stu-id="e7571-114">Describes the error.</span></span> |
|<span data-ttu-id="e7571-115">responseCode</span><span class="sxs-lookup"><span data-stu-id="e7571-115">responseCode</span></span> |<span data-ttu-id="e7571-116">String</span><span class="sxs-lookup"><span data-stu-id="e7571-116">String</span></span> |<span data-ttu-id="e7571-117">Код ответа от запроса для обеспечения доступности пользователя, ресурса или список рассылки.</span><span class="sxs-lookup"><span data-stu-id="e7571-117">The response code from querying for the availability of the user, distribution list, or resource.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="e7571-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e7571-118">JSON representation</span></span>

<span data-ttu-id="e7571-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e7571-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.freeBusyError"
}-->

```json
{
  "message": "String",
  "responseCode": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "freeBusyError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->