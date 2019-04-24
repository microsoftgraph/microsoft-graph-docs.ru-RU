---
title: Тип ресурса Митингинфо
description: Сведения о собрании, указанные для создания или присоединения к собранию.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c1126a3408b8353e927b5653fe60dd4a89125051
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457139"
---
# <a name="meetinginfo-resource-type"></a><span data-ttu-id="80151-103">Тип ресурса Митингинфо</span><span class="sxs-lookup"><span data-stu-id="80151-103">meetingInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="80151-104">Сведения о собрании, указанные для создания или присоединения к собранию.</span><span class="sxs-lookup"><span data-stu-id="80151-104">Meeting information specified to create or join a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="80151-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="80151-105">Properties</span></span>

| <span data-ttu-id="80151-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="80151-106">Property</span></span>       | <span data-ttu-id="80151-107">Тип</span><span class="sxs-lookup"><span data-stu-id="80151-107">Type</span></span>    | <span data-ttu-id="80151-108">Описание</span><span class="sxs-lookup"><span data-stu-id="80151-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="80151-109">Алловконверсатионвисаусост</span><span class="sxs-lookup"><span data-stu-id="80151-109">allowConversationWithoutHost</span></span> | <span data-ttu-id="80151-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="80151-110">Boolean</span></span> |  |

## <a name="json-representation"></a><span data-ttu-id="80151-111">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="80151-111">JSON representation</span></span>

<span data-ttu-id="80151-112">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="80151-112">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingInfo"
}-->
```json
{
  "allowConversationWithoutHost": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "meetingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/meetinginfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
