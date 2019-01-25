---
title: Тип ресурса customTimeZone
description: Представляет часовой пояс c нестандартным переходом на летнее время и обратно.
localization_priority: Normal
ms.openlocfilehash: 0bb961e213956ef3142df1f3d55a83918a14fa78
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515253"
---
# <a name="customtimezone-resource-type"></a><span data-ttu-id="41a34-103">Тип ресурса customTimeZone</span><span class="sxs-lookup"><span data-stu-id="41a34-103">customTimeZone resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="41a34-104">Представляет часовой пояс c нестандартным переходом на летнее время и обратно.</span><span class="sxs-lookup"><span data-stu-id="41a34-104">Represents a time zone where the transition from standard to daylight saving time, or vice versa is not standard.</span></span>


## <a name="properties"></a><span data-ttu-id="41a34-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="41a34-105">Properties</span></span>
| <span data-ttu-id="41a34-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="41a34-106">Property</span></span>     | <span data-ttu-id="41a34-107">Тип</span><span class="sxs-lookup"><span data-stu-id="41a34-107">Type</span></span>   |<span data-ttu-id="41a34-108">Описание</span><span class="sxs-lookup"><span data-stu-id="41a34-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="41a34-109">bias</span><span class="sxs-lookup"><span data-stu-id="41a34-109">bias</span></span> | <span data-ttu-id="41a34-110">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="41a34-110">Edm.Int32</span></span> | <span data-ttu-id="41a34-111">Смещение времени часового пояса относительно времени в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="41a34-111">The time offset of the time zone from Coordinated Universal Time (UTC).</span></span> <span data-ttu-id="41a34-112">Это значение представлено в минутах.</span><span class="sxs-lookup"><span data-stu-id="41a34-112">This value is in minutes.</span></span><span data-ttu-id="41a34-113">Часовые пояса с положительным смещением от UTC опережают время UTC, а с отрицательным смещением — отстают от него.</span><span class="sxs-lookup"><span data-stu-id="41a34-113"> Time zones that are ahead of UTC have a positive offset; time zones that are behind UTC have a negative offset.</span></span>|
| <span data-ttu-id="41a34-114">daylightOffset</span><span class="sxs-lookup"><span data-stu-id="41a34-114">daylightOffset</span></span> | [<span data-ttu-id="41a34-115">daylightTimeZoneOffset</span><span class="sxs-lookup"><span data-stu-id="41a34-115">daylightTimeZoneOffset</span></span>](daylighttimezoneoffset.md) | <span data-ttu-id="41a34-116">Определяет, когда в часовом поясе осуществляется переход со стандартного времени на летнее.</span><span class="sxs-lookup"><span data-stu-id="41a34-116">Specifies when the time zone switches from standard time to daylight saving time.</span></span> |
| <span data-ttu-id="41a34-117">name</span><span class="sxs-lookup"><span data-stu-id="41a34-117">name</span></span> | <span data-ttu-id="41a34-118">строка</span><span class="sxs-lookup"><span data-stu-id="41a34-118">string</span></span> | <span data-ttu-id="41a34-119">Имя настраиваемого часового пояса.</span><span class="sxs-lookup"><span data-stu-id="41a34-119">The name of the custom time zone.</span></span> |
| <span data-ttu-id="41a34-120">standardOffset</span><span class="sxs-lookup"><span data-stu-id="41a34-120">standardOffset</span></span> | [<span data-ttu-id="41a34-121">standardTimeZoneOffset</span><span class="sxs-lookup"><span data-stu-id="41a34-121">standardTimeZoneOffset</span></span>](standardtimezoneoffset.md) | <span data-ttu-id="41a34-122">Определяет, когда в часовом поясе осуществляется переход с летнего времени на стандартное.</span><span class="sxs-lookup"><span data-stu-id="41a34-122">Specifies when the time zone switches from daylight saving time to standard time.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="41a34-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="41a34-123">JSON representation</span></span>

<span data-ttu-id="41a34-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="41a34-124">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.customTimeZone"
}-->

```json
{
  "bias": "Int32",
  "daylightOffset": {"@odata.type": "microsoft.graph.daylightTimeZoneOffset"},
  "name": "string",
  "standardOffset": {"@odata.type": "microsoft.graph.standardTimeZoneOffset"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "customTimeZone resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/customtimezone.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
