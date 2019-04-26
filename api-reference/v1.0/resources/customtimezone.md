---
title: Тип ресурса customTimeZone
description: Представляет часовой пояс c нестандартным переходом на летнее время и обратно.
localization_priority: Normal
ms.openlocfilehash: 7d43de045b99a1163ae8fc74e40d659d10cabe63
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32574745"
---
# <a name="customtimezone-resource-type"></a><span data-ttu-id="7a001-103">Тип ресурса customTimeZone</span><span class="sxs-lookup"><span data-stu-id="7a001-103">customTimeZone resource type</span></span>

<span data-ttu-id="7a001-104">Представляет часовой пояс c нестандартным переходом на летнее время и обратно.</span><span class="sxs-lookup"><span data-stu-id="7a001-104">Represents a time zone where the transition from standard to daylight saving time, or vice versa is not standard.</span></span>


## <a name="properties"></a><span data-ttu-id="7a001-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="7a001-105">Properties</span></span>
| <span data-ttu-id="7a001-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="7a001-106">Property</span></span>     | <span data-ttu-id="7a001-107">Тип</span><span class="sxs-lookup"><span data-stu-id="7a001-107">Type</span></span>   |<span data-ttu-id="7a001-108">Описание</span><span class="sxs-lookup"><span data-stu-id="7a001-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7a001-109">bias</span><span class="sxs-lookup"><span data-stu-id="7a001-109">bias</span></span> | <span data-ttu-id="7a001-110">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="7a001-110">Edm.Int32</span></span> | <span data-ttu-id="7a001-111">Смещение времени часового пояса относительно времени в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="7a001-111">The time offset of the time zone from Coordinated Universal Time (UTC).</span></span> <span data-ttu-id="7a001-112">Это значение представлено в минутах.</span><span class="sxs-lookup"><span data-stu-id="7a001-112">This value is in minutes.</span></span><span data-ttu-id="7a001-113">Часовые пояса с положительным смещением от UTC опережают время UTC, а с отрицательным смещением — отстают от него.</span><span class="sxs-lookup"><span data-stu-id="7a001-113"> Time zones that are ahead of UTC have a positive offset; time zones that are behind UTC have a negative offset.</span></span>|
| <span data-ttu-id="7a001-114">daylightOffset</span><span class="sxs-lookup"><span data-stu-id="7a001-114">daylightOffset</span></span> | [<span data-ttu-id="7a001-115">daylightTimeZoneOffset</span><span class="sxs-lookup"><span data-stu-id="7a001-115">daylightTimeZoneOffset</span></span>](daylighttimezoneoffset.md) | <span data-ttu-id="7a001-116">Определяет, когда в часовом поясе осуществляется переход со стандартного времени на летнее.</span><span class="sxs-lookup"><span data-stu-id="7a001-116">Specifies when the time zone switches from standard time to daylight saving time.</span></span> |
| <span data-ttu-id="7a001-117">name</span><span class="sxs-lookup"><span data-stu-id="7a001-117">name</span></span> | <span data-ttu-id="7a001-118">string</span><span class="sxs-lookup"><span data-stu-id="7a001-118">string</span></span> | <span data-ttu-id="7a001-119">Имя настраиваемого часового пояса.</span><span class="sxs-lookup"><span data-stu-id="7a001-119">The name of the custom time zone.</span></span> |
| <span data-ttu-id="7a001-120">standardOffset</span><span class="sxs-lookup"><span data-stu-id="7a001-120">standardOffset</span></span> | [<span data-ttu-id="7a001-121">standardTimeZoneOffset</span><span class="sxs-lookup"><span data-stu-id="7a001-121">standardTimeZoneOffset</span></span>](standardtimezoneoffset.md) | <span data-ttu-id="7a001-122">Определяет, когда в часовом поясе осуществляется переход с летнего времени на стандартное.</span><span class="sxs-lookup"><span data-stu-id="7a001-122">Specifies when the time zone switches from daylight saving time to standard time.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="7a001-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7a001-123">JSON representation</span></span>

<span data-ttu-id="7a001-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7a001-124">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.timeZoneBase",
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
<!-- {
  "type": "#page.annotation",
  "description": "customTimeZone resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
