---
title: Тип ресурса freeBusyError
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
ms.openlocfilehash: f1ff7717034798830a610b35dbbff5c987cf7371
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529847"
---
# <a name="freebusyerror-resource-type"></a><span data-ttu-id="6ffd2-104">Тип ресурса freeBusyError</span><span class="sxs-lookup"><span data-stu-id="6ffd2-104">freeBusyError resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="6ffd2-105">Представляет сведения об ошибке при попытке получить доступности пользователя, ресурса или список рассылки.</span><span class="sxs-lookup"><span data-stu-id="6ffd2-105">Represents error information from attempting to get the availability of a user, distribution list, or resource.</span></span>

## <a name="properties"></a><span data-ttu-id="6ffd2-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="6ffd2-106">Properties</span></span>
| <span data-ttu-id="6ffd2-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="6ffd2-107">Property</span></span>     | <span data-ttu-id="6ffd2-108">Тип</span><span class="sxs-lookup"><span data-stu-id="6ffd2-108">Type</span></span>   |<span data-ttu-id="6ffd2-109">Описание</span><span class="sxs-lookup"><span data-stu-id="6ffd2-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6ffd2-110">message</span><span class="sxs-lookup"><span data-stu-id="6ffd2-110">message</span></span> |<span data-ttu-id="6ffd2-111">String</span><span class="sxs-lookup"><span data-stu-id="6ffd2-111">String</span></span> |<span data-ttu-id="6ffd2-112">Описание ошибки.</span><span class="sxs-lookup"><span data-stu-id="6ffd2-112">Describes the error.</span></span> |
|<span data-ttu-id="6ffd2-113">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="6ffd2-113">responseCode</span></span> |<span data-ttu-id="6ffd2-114">String</span><span class="sxs-lookup"><span data-stu-id="6ffd2-114">String</span></span> |<span data-ttu-id="6ffd2-115">Код ответа от запроса для обеспечения доступности пользователя, ресурса или список рассылки.</span><span class="sxs-lookup"><span data-stu-id="6ffd2-115">The response code from querying for the availability of the user, distribution list, or resource.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="6ffd2-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6ffd2-116">JSON representation</span></span>

<span data-ttu-id="6ffd2-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6ffd2-117">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "freeBusyError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/freebusyerror.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
