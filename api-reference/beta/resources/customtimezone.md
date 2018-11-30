---
title: Тип ресурса customTimeZone
description: Представляет часовой пояс c нестандартным переходом на летнее время и обратно.
ms.openlocfilehash: 83375c96e4247cb0ddf2d17b1bede2c295f0b27f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074918"
---
# <a name="customtimezone-resource-type"></a><span data-ttu-id="8b053-103">Тип ресурса customTimeZone</span><span class="sxs-lookup"><span data-stu-id="8b053-103">customTimeZone resource type</span></span>

> <span data-ttu-id="8b053-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8b053-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8b053-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b053-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8b053-106">Представляет часовой пояс c нестандартным переходом на летнее время и обратно.</span><span class="sxs-lookup"><span data-stu-id="8b053-106">Represents a time zone where the transition from standard to daylight saving time, or vice versa is not standard.</span></span>


## <a name="properties"></a><span data-ttu-id="8b053-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="8b053-107">Properties</span></span>
| <span data-ttu-id="8b053-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="8b053-108">Property</span></span>     | <span data-ttu-id="8b053-109">Тип</span><span class="sxs-lookup"><span data-stu-id="8b053-109">Type</span></span>   |<span data-ttu-id="8b053-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8b053-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8b053-111">bias</span><span class="sxs-lookup"><span data-stu-id="8b053-111">bias</span></span> | <span data-ttu-id="8b053-112">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="8b053-112">Edm.Int32</span></span> | <span data-ttu-id="8b053-113">Смещение времени часового пояса относительно времени в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="8b053-113">The time offset of the time zone from Coordinated Universal Time (UTC).</span></span> <span data-ttu-id="8b053-114">Это значение представлено в минутах.</span><span class="sxs-lookup"><span data-stu-id="8b053-114">This value is in minutes.</span></span><span data-ttu-id="8b053-115">Часовые пояса с положительным смещением от UTC опережают время UTC, а с отрицательным смещением — отстают от него.</span><span class="sxs-lookup"><span data-stu-id="8b053-115"> Time zones that are ahead of UTC have a positive offset; time zones that are behind UTC have a negative offset.</span></span>|
| <span data-ttu-id="8b053-116">daylightOffset</span><span class="sxs-lookup"><span data-stu-id="8b053-116">daylightOffset</span></span> | [<span data-ttu-id="8b053-117">daylightTimeZoneOffset</span><span class="sxs-lookup"><span data-stu-id="8b053-117">daylightTimeZoneOffset</span></span>](daylighttimezoneoffset.md) | <span data-ttu-id="8b053-118">Определяет, когда в часовом поясе осуществляется переход со стандартного времени на летнее.</span><span class="sxs-lookup"><span data-stu-id="8b053-118">Specifies when the time zone switches from standard time to daylight saving time.</span></span> |
| <span data-ttu-id="8b053-119">name</span><span class="sxs-lookup"><span data-stu-id="8b053-119">name</span></span> | <span data-ttu-id="8b053-120">строка</span><span class="sxs-lookup"><span data-stu-id="8b053-120">string</span></span> | <span data-ttu-id="8b053-121">Имя настраиваемого часового пояса.</span><span class="sxs-lookup"><span data-stu-id="8b053-121">The name of the custom time zone.</span></span> |
| <span data-ttu-id="8b053-122">standardOffset</span><span class="sxs-lookup"><span data-stu-id="8b053-122">standardOffset</span></span> | [<span data-ttu-id="8b053-123">standardTimeZoneOffset</span><span class="sxs-lookup"><span data-stu-id="8b053-123">standardTimeZoneOffset</span></span>](standardtimezoneoffset.md) | <span data-ttu-id="8b053-124">Определяет, когда в часовом поясе осуществляется переход с летнего времени на стандартное.</span><span class="sxs-lookup"><span data-stu-id="8b053-124">Specifies when the time zone switches from daylight saving time to standard time.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="8b053-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8b053-125">JSON representation</span></span>

<span data-ttu-id="8b053-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8b053-126">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "customTimeZone resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->