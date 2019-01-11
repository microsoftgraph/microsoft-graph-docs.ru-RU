---
title: Тип ресурса freeBusyError
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
ms.openlocfilehash: 63cfc4b14ba6176d582155df57b7f7f787e63cf4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889770"
---
# <a name="freebusyerror-resource-type"></a><span data-ttu-id="73fe8-104">Тип ресурса freeBusyError</span><span class="sxs-lookup"><span data-stu-id="73fe8-104">freeBusyError resource type</span></span>

 > <span data-ttu-id="73fe8-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="73fe8-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="73fe8-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73fe8-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="73fe8-107">Представляет сведения об ошибке при попытке получить доступности пользователя, ресурса или список рассылки.</span><span class="sxs-lookup"><span data-stu-id="73fe8-107">Represents error information from attempting to get the availability of a user, distribution list, or resource.</span></span>

## <a name="properties"></a><span data-ttu-id="73fe8-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="73fe8-108">Properties</span></span>
| <span data-ttu-id="73fe8-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="73fe8-109">Property</span></span>     | <span data-ttu-id="73fe8-110">Тип</span><span class="sxs-lookup"><span data-stu-id="73fe8-110">Type</span></span>   |<span data-ttu-id="73fe8-111">Описание</span><span class="sxs-lookup"><span data-stu-id="73fe8-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="73fe8-112">message</span><span class="sxs-lookup"><span data-stu-id="73fe8-112">message</span></span> |<span data-ttu-id="73fe8-113">String</span><span class="sxs-lookup"><span data-stu-id="73fe8-113">String</span></span> |<span data-ttu-id="73fe8-114">Описание ошибки.</span><span class="sxs-lookup"><span data-stu-id="73fe8-114">Describes the error.</span></span> |
|<span data-ttu-id="73fe8-115">responseCode</span><span class="sxs-lookup"><span data-stu-id="73fe8-115">responseCode</span></span> |<span data-ttu-id="73fe8-116">Строка</span><span class="sxs-lookup"><span data-stu-id="73fe8-116">String</span></span> |<span data-ttu-id="73fe8-117">Код ответа от запроса для обеспечения доступности пользователя, ресурса или список рассылки.</span><span class="sxs-lookup"><span data-stu-id="73fe8-117">The response code from querying for the availability of the user, distribution list, or resource.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="73fe8-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="73fe8-118">JSON representation</span></span>

<span data-ttu-id="73fe8-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="73fe8-119">The following is a JSON representation of the resource.</span></span>

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
