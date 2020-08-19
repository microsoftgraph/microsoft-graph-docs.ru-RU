---
title: Тип ресурса customTimeZone
description: Представляет часовой пояс c нестандартным переходом на летнее время и обратно.
localization_priority: Normal
author: svpsiva
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 8e82524b107cb787905b87e564347148415724f8
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812325"
---
# <a name="customtimezone-resource-type"></a><span data-ttu-id="15ad2-103">Тип ресурса customTimeZone</span><span class="sxs-lookup"><span data-stu-id="15ad2-103">customTimeZone resource type</span></span>

<span data-ttu-id="15ad2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="15ad2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="15ad2-105">Представляет часовой пояс c нестандартным переходом на летнее время и обратно.</span><span class="sxs-lookup"><span data-stu-id="15ad2-105">Represents a time zone where the transition from standard to daylight saving time, or vice versa is not standard.</span></span>


## <a name="properties"></a><span data-ttu-id="15ad2-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="15ad2-106">Properties</span></span>
| <span data-ttu-id="15ad2-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="15ad2-107">Property</span></span>     | <span data-ttu-id="15ad2-108">Тип</span><span class="sxs-lookup"><span data-stu-id="15ad2-108">Type</span></span>   |<span data-ttu-id="15ad2-109">Описание</span><span class="sxs-lookup"><span data-stu-id="15ad2-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="15ad2-110">bias</span><span class="sxs-lookup"><span data-stu-id="15ad2-110">bias</span></span> | <span data-ttu-id="15ad2-111">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="15ad2-111">Edm.Int32</span></span> | <span data-ttu-id="15ad2-112">Смещение времени часового пояса относительно времени в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="15ad2-112">The time offset of the time zone from Coordinated Universal Time (UTC).</span></span> <span data-ttu-id="15ad2-113">Это значение представлено в минутах.</span><span class="sxs-lookup"><span data-stu-id="15ad2-113">This value is in minutes.</span></span><span data-ttu-id="15ad2-114">Часовые пояса с положительным смещением от UTC опережают время UTC, а с отрицательным смещением — отстают от него.</span><span class="sxs-lookup"><span data-stu-id="15ad2-114"> Time zones that are ahead of UTC have a positive offset; time zones that are behind UTC have a negative offset.</span></span>|
| <span data-ttu-id="15ad2-115">daylightOffset</span><span class="sxs-lookup"><span data-stu-id="15ad2-115">daylightOffset</span></span> | [<span data-ttu-id="15ad2-116">daylightTimeZoneOffset</span><span class="sxs-lookup"><span data-stu-id="15ad2-116">daylightTimeZoneOffset</span></span>](daylighttimezoneoffset.md) | <span data-ttu-id="15ad2-117">Определяет, когда в часовом поясе осуществляется переход со стандартного времени на летнее.</span><span class="sxs-lookup"><span data-stu-id="15ad2-117">Specifies when the time zone switches from standard time to daylight saving time.</span></span> |
| <span data-ttu-id="15ad2-118">name</span><span class="sxs-lookup"><span data-stu-id="15ad2-118">name</span></span> | <span data-ttu-id="15ad2-119">string</span><span class="sxs-lookup"><span data-stu-id="15ad2-119">string</span></span> | <span data-ttu-id="15ad2-120">Имя настраиваемого часового пояса.</span><span class="sxs-lookup"><span data-stu-id="15ad2-120">The name of the custom time zone.</span></span> |
| <span data-ttu-id="15ad2-121">standardOffset</span><span class="sxs-lookup"><span data-stu-id="15ad2-121">standardOffset</span></span> | [<span data-ttu-id="15ad2-122">standardTimeZoneOffset</span><span class="sxs-lookup"><span data-stu-id="15ad2-122">standardTimeZoneOffset</span></span>](standardtimezoneoffset.md) | <span data-ttu-id="15ad2-123">Определяет, когда в часовом поясе осуществляется переход с летнего времени на стандартное.</span><span class="sxs-lookup"><span data-stu-id="15ad2-123">Specifies when the time zone switches from daylight saving time to standard time.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="15ad2-124">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="15ad2-124">JSON representation</span></span>

<span data-ttu-id="15ad2-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="15ad2-125">Here is a JSON representation of the resource.</span></span>

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
