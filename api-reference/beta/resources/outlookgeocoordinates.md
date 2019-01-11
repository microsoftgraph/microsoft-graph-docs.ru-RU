---
title: Тип ресурса outlookGeoCoordinates
description: Географические координаты, высота и точность физического местоположения.
localization_priority: Normal
ms.openlocfilehash: 2522410cd55705411084945b0519738871dedaa0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845362"
---
# <a name="outlookgeocoordinates-resource-type"></a><span data-ttu-id="b2e24-103">Тип ресурса outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="b2e24-103">outlookGeoCoordinates resource type</span></span>

> <span data-ttu-id="b2e24-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b2e24-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b2e24-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2e24-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b2e24-106">Географические координаты, высота и точность физического местоположения.</span><span class="sxs-lookup"><span data-stu-id="b2e24-106">The geographic coordinates, elevation, and their degree of accuracy for a physical location.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b2e24-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b2e24-107">JSON representation</span></span>

<span data-ttu-id="b2e24-108">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b2e24-108">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.outlookGeoCoordinates"
}-->

```json
{
  "accuracy": 1024.13,
  "altitude": 1024.13,
  "altitudeAccuracy": 1024.13,
  "latitude": 1024.13,
  "longitude": 1024.13
}

```
## <a name="properties"></a><span data-ttu-id="b2e24-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="b2e24-109">Properties</span></span>
| <span data-ttu-id="b2e24-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="b2e24-110">Property</span></span>     | <span data-ttu-id="b2e24-111">Тип</span><span class="sxs-lookup"><span data-stu-id="b2e24-111">Type</span></span>   |<span data-ttu-id="b2e24-112">Описание</span><span class="sxs-lookup"><span data-stu-id="b2e24-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b2e24-113">accuracy</span><span class="sxs-lookup"><span data-stu-id="b2e24-113">accuracy</span></span>|<span data-ttu-id="b2e24-114">double</span><span class="sxs-lookup"><span data-stu-id="b2e24-114">double</span></span>|<span data-ttu-id="b2e24-115">Точность широты и долготы.</span><span class="sxs-lookup"><span data-stu-id="b2e24-115">The accuracy of the latitude and longitude.</span></span> <span data-ttu-id="b2e24-116">Например, точность может измеряться в метрах и составлять 50 метров.</span><span class="sxs-lookup"><span data-stu-id="b2e24-116">As an example, the accuracy can be measured in meters, such as the latitude and longitude are accurate to within 50 meters.</span></span>|
|<span data-ttu-id="b2e24-117">altitude</span><span class="sxs-lookup"><span data-stu-id="b2e24-117">altitude</span></span>|<span data-ttu-id="b2e24-118">double</span><span class="sxs-lookup"><span data-stu-id="b2e24-118">double</span></span>|<span data-ttu-id="b2e24-119">Высота местоположения.</span><span class="sxs-lookup"><span data-stu-id="b2e24-119">The altitude of the location.</span></span>|
|<span data-ttu-id="b2e24-120">altitudeAccuracy</span><span class="sxs-lookup"><span data-stu-id="b2e24-120">altitudeAccuracy</span></span>|<span data-ttu-id="b2e24-121">double</span><span class="sxs-lookup"><span data-stu-id="b2e24-121">double</span></span>|<span data-ttu-id="b2e24-122">Точность высоты.</span><span class="sxs-lookup"><span data-stu-id="b2e24-122">The accuracy of the altitude.</span></span>|
|<span data-ttu-id="b2e24-123">latitude</span><span class="sxs-lookup"><span data-stu-id="b2e24-123">latitude</span></span>|<span data-ttu-id="b2e24-124">double</span><span class="sxs-lookup"><span data-stu-id="b2e24-124">double</span></span>|<span data-ttu-id="b2e24-125">Широта местоположения.</span><span class="sxs-lookup"><span data-stu-id="b2e24-125">The latitude of the location.</span></span>|
|<span data-ttu-id="b2e24-126">longitude</span><span class="sxs-lookup"><span data-stu-id="b2e24-126">longitude</span></span>|<span data-ttu-id="b2e24-127">double</span><span class="sxs-lookup"><span data-stu-id="b2e24-127">double</span></span>|<span data-ttu-id="b2e24-128">Долгота местоположения.</span><span class="sxs-lookup"><span data-stu-id="b2e24-128">The longitude of the location.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookGeoCoordinates resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
