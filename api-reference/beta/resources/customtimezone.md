---
title: Тип ресурса customTimeZone
description: Представляет часовой пояс c нестандартным переходом на летнее время и обратно.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 40ab8318931f720780ef21ae6b1c455fc6125814
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507319"
---
# <a name="customtimezone-resource-type"></a><span data-ttu-id="7d596-103">Тип ресурса customTimeZone</span><span class="sxs-lookup"><span data-stu-id="7d596-103">customTimeZone resource type</span></span>

<span data-ttu-id="7d596-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7d596-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7d596-105">Представляет часовой пояс c нестандартным переходом на летнее время и обратно.</span><span class="sxs-lookup"><span data-stu-id="7d596-105">Represents a time zone where the transition from standard to daylight saving time, or vice versa is not standard.</span></span>


## <a name="properties"></a><span data-ttu-id="7d596-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="7d596-106">Properties</span></span>
| <span data-ttu-id="7d596-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="7d596-107">Property</span></span>     | <span data-ttu-id="7d596-108">Тип</span><span class="sxs-lookup"><span data-stu-id="7d596-108">Type</span></span>   |<span data-ttu-id="7d596-109">Описание</span><span class="sxs-lookup"><span data-stu-id="7d596-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7d596-110">bias</span><span class="sxs-lookup"><span data-stu-id="7d596-110">bias</span></span> | <span data-ttu-id="7d596-111">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="7d596-111">Edm.Int32</span></span> | <span data-ttu-id="7d596-112">Смещение времени часового пояса относительно времени в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="7d596-112">The time offset of the time zone from Coordinated Universal Time (UTC).</span></span> <span data-ttu-id="7d596-113">Это значение представлено в минутах.</span><span class="sxs-lookup"><span data-stu-id="7d596-113">This value is in minutes.</span></span><span data-ttu-id="7d596-114">Часовые пояса с положительным смещением от UTC опережают время UTC, а с отрицательным смещением — отстают от него.</span><span class="sxs-lookup"><span data-stu-id="7d596-114"> Time zones that are ahead of UTC have a positive offset; time zones that are behind UTC have a negative offset.</span></span>|
| <span data-ttu-id="7d596-115">daylightOffset</span><span class="sxs-lookup"><span data-stu-id="7d596-115">daylightOffset</span></span> | [<span data-ttu-id="7d596-116">daylightTimeZoneOffset</span><span class="sxs-lookup"><span data-stu-id="7d596-116">daylightTimeZoneOffset</span></span>](daylighttimezoneoffset.md) | <span data-ttu-id="7d596-117">Определяет, когда в часовом поясе осуществляется переход со стандартного времени на летнее.</span><span class="sxs-lookup"><span data-stu-id="7d596-117">Specifies when the time zone switches from standard time to daylight saving time.</span></span> |
| <span data-ttu-id="7d596-118">name</span><span class="sxs-lookup"><span data-stu-id="7d596-118">name</span></span> | <span data-ttu-id="7d596-119">string</span><span class="sxs-lookup"><span data-stu-id="7d596-119">string</span></span> | <span data-ttu-id="7d596-120">Имя настраиваемого часового пояса.</span><span class="sxs-lookup"><span data-stu-id="7d596-120">The name of the custom time zone.</span></span> |
| <span data-ttu-id="7d596-121">standardOffset</span><span class="sxs-lookup"><span data-stu-id="7d596-121">standardOffset</span></span> | [<span data-ttu-id="7d596-122">standardTimeZoneOffset</span><span class="sxs-lookup"><span data-stu-id="7d596-122">standardTimeZoneOffset</span></span>](standardtimezoneoffset.md) | <span data-ttu-id="7d596-123">Определяет, когда в часовом поясе осуществляется переход с летнего времени на стандартное.</span><span class="sxs-lookup"><span data-stu-id="7d596-123">Specifies when the time zone switches from daylight saving time to standard time.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="7d596-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7d596-124">JSON representation</span></span>

<span data-ttu-id="7d596-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7d596-125">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
