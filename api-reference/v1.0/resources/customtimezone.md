---
title: Тип ресурса customTimeZone
description: Представляет часовой пояс c нестандартным переходом на летнее время и обратно.
localization_priority: Normal
author: abheek-das
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: a4d05d000b2491fcc9d02b3e39bb012e6e5f023e
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130517"
---
# <a name="customtimezone-resource-type"></a><span data-ttu-id="b6068-103">Тип ресурса customTimeZone</span><span class="sxs-lookup"><span data-stu-id="b6068-103">customTimeZone resource type</span></span>

<span data-ttu-id="b6068-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b6068-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b6068-105">Представляет часовой пояс c нестандартным переходом на летнее время и обратно.</span><span class="sxs-lookup"><span data-stu-id="b6068-105">Represents a time zone where the transition from standard to daylight saving time, or vice versa is not standard.</span></span>


## <a name="properties"></a><span data-ttu-id="b6068-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="b6068-106">Properties</span></span>
| <span data-ttu-id="b6068-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="b6068-107">Property</span></span>     | <span data-ttu-id="b6068-108">Тип</span><span class="sxs-lookup"><span data-stu-id="b6068-108">Type</span></span>   |<span data-ttu-id="b6068-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b6068-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b6068-110">bias</span><span class="sxs-lookup"><span data-stu-id="b6068-110">bias</span></span> | <span data-ttu-id="b6068-111">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="b6068-111">Edm.Int32</span></span> | <span data-ttu-id="b6068-112">Смещение времени часового пояса относительно времени в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="b6068-112">The time offset of the time zone from Coordinated Universal Time (UTC).</span></span> <span data-ttu-id="b6068-113">Это значение представлено в минутах.</span><span class="sxs-lookup"><span data-stu-id="b6068-113">This value is in minutes.</span></span> <span data-ttu-id="b6068-114">Часовые пояса с положительным смещением от UTC опережают время UTC, а с отрицательным смещением — отстают от него.</span><span class="sxs-lookup"><span data-stu-id="b6068-114">Time zones that are ahead of UTC have a positive offset; time zones that are behind UTC have a negative offset.</span></span>|
| <span data-ttu-id="b6068-115">daylightOffset</span><span class="sxs-lookup"><span data-stu-id="b6068-115">daylightOffset</span></span> | [<span data-ttu-id="b6068-116">daylightTimeZoneOffset</span><span class="sxs-lookup"><span data-stu-id="b6068-116">daylightTimeZoneOffset</span></span>](daylighttimezoneoffset.md) | <span data-ttu-id="b6068-117">Определяет, когда в часовом поясе осуществляется переход со стандартного времени на летнее.</span><span class="sxs-lookup"><span data-stu-id="b6068-117">Specifies when the time zone switches from standard time to daylight saving time.</span></span> |
| <span data-ttu-id="b6068-118">name</span><span class="sxs-lookup"><span data-stu-id="b6068-118">name</span></span> | <span data-ttu-id="b6068-119">string</span><span class="sxs-lookup"><span data-stu-id="b6068-119">string</span></span> | <span data-ttu-id="b6068-120">Имя настраиваемого часового пояса.</span><span class="sxs-lookup"><span data-stu-id="b6068-120">The name of the custom time zone.</span></span> |
| <span data-ttu-id="b6068-121">standardOffset</span><span class="sxs-lookup"><span data-stu-id="b6068-121">standardOffset</span></span> | [<span data-ttu-id="b6068-122">standardTimeZoneOffset</span><span class="sxs-lookup"><span data-stu-id="b6068-122">standardTimeZoneOffset</span></span>](standardtimezoneoffset.md) | <span data-ttu-id="b6068-123">Определяет, когда в часовом поясе осуществляется переход с летнего времени на стандартное.</span><span class="sxs-lookup"><span data-stu-id="b6068-123">Specifies when the time zone switches from daylight saving time to standard time.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="b6068-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b6068-124">JSON representation</span></span>

<span data-ttu-id="b6068-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b6068-125">Here is a JSON representation of the resource.</span></span>

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

