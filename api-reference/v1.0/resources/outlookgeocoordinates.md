---
title: Тип ресурса outlookGeoCoordinates
description: Географические координаты, высота и точность физического местоположения.
localization_priority: Normal
author: harini84
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: ae101814d7e32be67ae7becc6e2032ff4e2026d2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43353851"
---
# <a name="outlookgeocoordinates-resource-type"></a><span data-ttu-id="1f22a-103">Тип ресурса outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="1f22a-103">outlookGeoCoordinates resource type</span></span>

<span data-ttu-id="1f22a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f22a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1f22a-105">Географические координаты, высота и точность физического местоположения.</span><span class="sxs-lookup"><span data-stu-id="1f22a-105">The geographic coordinates, elevation, and their degree of accuracy for a physical location.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1f22a-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1f22a-106">JSON representation</span></span>

<span data-ttu-id="1f22a-107">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1f22a-107">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="1f22a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="1f22a-108">Properties</span></span>
| <span data-ttu-id="1f22a-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="1f22a-109">Property</span></span>     | <span data-ttu-id="1f22a-110">Тип</span><span class="sxs-lookup"><span data-stu-id="1f22a-110">Type</span></span>   |<span data-ttu-id="1f22a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="1f22a-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1f22a-112">accuracy</span><span class="sxs-lookup"><span data-stu-id="1f22a-112">accuracy</span></span>|<span data-ttu-id="1f22a-113">double</span><span class="sxs-lookup"><span data-stu-id="1f22a-113">double</span></span>|<span data-ttu-id="1f22a-114">Точность широты и долготы.</span><span class="sxs-lookup"><span data-stu-id="1f22a-114">The accuracy of the latitude and longitude.</span></span> <span data-ttu-id="1f22a-115">Например, точность может измеряться в метрах и составлять 50 метров.</span><span class="sxs-lookup"><span data-stu-id="1f22a-115">As an example, the accuracy can be measured in meters, such as the latitude and longitude are accurate to within 50 meters.</span></span>|
|<span data-ttu-id="1f22a-116">altitude</span><span class="sxs-lookup"><span data-stu-id="1f22a-116">altitude</span></span>|<span data-ttu-id="1f22a-117">double</span><span class="sxs-lookup"><span data-stu-id="1f22a-117">double</span></span>|<span data-ttu-id="1f22a-118">Высота местоположения.</span><span class="sxs-lookup"><span data-stu-id="1f22a-118">The altitude of the location.</span></span>|
|<span data-ttu-id="1f22a-119">altitudeAccuracy</span><span class="sxs-lookup"><span data-stu-id="1f22a-119">altitudeAccuracy</span></span>|<span data-ttu-id="1f22a-120">double</span><span class="sxs-lookup"><span data-stu-id="1f22a-120">double</span></span>|<span data-ttu-id="1f22a-121">Точность высоты.</span><span class="sxs-lookup"><span data-stu-id="1f22a-121">The accuracy of the altitude.</span></span>|
|<span data-ttu-id="1f22a-122">latitude</span><span class="sxs-lookup"><span data-stu-id="1f22a-122">latitude</span></span>|<span data-ttu-id="1f22a-123">double</span><span class="sxs-lookup"><span data-stu-id="1f22a-123">double</span></span>|<span data-ttu-id="1f22a-124">Широта местоположения.</span><span class="sxs-lookup"><span data-stu-id="1f22a-124">The latitude of the location.</span></span>|
|<span data-ttu-id="1f22a-125">longitude</span><span class="sxs-lookup"><span data-stu-id="1f22a-125">longitude</span></span>|<span data-ttu-id="1f22a-126">double</span><span class="sxs-lookup"><span data-stu-id="1f22a-126">double</span></span>|<span data-ttu-id="1f22a-127">Долгота местоположения.</span><span class="sxs-lookup"><span data-stu-id="1f22a-127">The longitude of the location.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookGeoCoordinates resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
