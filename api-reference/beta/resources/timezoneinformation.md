---
title: Тип ресурса timeZoneInformation
description: Представляет часовой пояс. Поддерживаемые формата является Windows и Internet Assigned Numbers Authority (IANA) часовой пояс (также известной как Олсон часовой пояс)
localization_priority: Normal
ms.openlocfilehash: a63721de7ed4e8c3f3b74ce5954a88ee71a95414
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526776"
---
# <a name="timezoneinformation-resource-type"></a><span data-ttu-id="e767e-104">Тип ресурса timeZoneInformation</span><span class="sxs-lookup"><span data-stu-id="e767e-104">timeZoneInformation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e767e-105">Представляет часовой пояс.</span><span class="sxs-lookup"><span data-stu-id="e767e-105">Represents a time zone.</span></span> <span data-ttu-id="e767e-106">Поддерживаются формат Windows и формат [часового пояса IANA](https://www.iana.org/time-zones), также известного как часовой пояс Олсона (после устранения известной проблемы).</span><span class="sxs-lookup"><span data-stu-id="e767e-106">The supported format is Windows, and [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format as well when the current known problem is fixed.</span></span>

## <a name="properties"></a><span data-ttu-id="e767e-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="e767e-107">Properties</span></span>
| <span data-ttu-id="e767e-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="e767e-108">Property</span></span>     | <span data-ttu-id="e767e-109">Тип</span><span class="sxs-lookup"><span data-stu-id="e767e-109">Type</span></span>   |<span data-ttu-id="e767e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e767e-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e767e-111">alias</span><span class="sxs-lookup"><span data-stu-id="e767e-111">alias</span></span>|<span data-ttu-id="e767e-112">string</span><span class="sxs-lookup"><span data-stu-id="e767e-112">string</span></span>|<span data-ttu-id="e767e-113">Идентификатор часового пояса.</span><span class="sxs-lookup"><span data-stu-id="e767e-113">An identifier for the time zone.</span></span>|
|<span data-ttu-id="e767e-114">displayName</span><span class="sxs-lookup"><span data-stu-id="e767e-114">displayName</span></span>|<span data-ttu-id="e767e-115">строка</span><span class="sxs-lookup"><span data-stu-id="e767e-115">string</span></span>|<span data-ttu-id="e767e-116">Отображаемое имя часового пояса.</span><span class="sxs-lookup"><span data-stu-id="e767e-116">A display string that represents the time zone.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e767e-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e767e-117">JSON representation</span></span>

<span data-ttu-id="e767e-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e767e-118">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeZoneInformation"
}-->

```json
{
  "alias": "string",
  "displayName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeZoneInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/timezoneinformation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
