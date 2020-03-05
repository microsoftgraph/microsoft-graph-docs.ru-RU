---
title: Тип ресурса outlookGeoCoordinates
description: Географические координаты, высота и точность физического местоположения.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 2fba6b6d811a10f06338e8e13e5c8dc487e31813
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522188"
---
# <a name="outlookgeocoordinates-resource-type"></a><span data-ttu-id="26863-103">Тип ресурса outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="26863-103">outlookGeoCoordinates resource type</span></span>

<span data-ttu-id="26863-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="26863-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26863-105">Географические координаты, высота и точность физического местоположения.</span><span class="sxs-lookup"><span data-stu-id="26863-105">The geographic coordinates, elevation, and their degree of accuracy for a physical location.</span></span>

## <a name="json-representation"></a><span data-ttu-id="26863-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="26863-106">JSON representation</span></span>

<span data-ttu-id="26863-107">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="26863-107">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="26863-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="26863-108">Properties</span></span>
| <span data-ttu-id="26863-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="26863-109">Property</span></span>     | <span data-ttu-id="26863-110">Тип</span><span class="sxs-lookup"><span data-stu-id="26863-110">Type</span></span>   |<span data-ttu-id="26863-111">Описание</span><span class="sxs-lookup"><span data-stu-id="26863-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="26863-112">accuracy</span><span class="sxs-lookup"><span data-stu-id="26863-112">accuracy</span></span>|<span data-ttu-id="26863-113">double</span><span class="sxs-lookup"><span data-stu-id="26863-113">double</span></span>|<span data-ttu-id="26863-114">Точность широты и долготы.</span><span class="sxs-lookup"><span data-stu-id="26863-114">The accuracy of the latitude and longitude.</span></span> <span data-ttu-id="26863-115">Например, точность может измеряться в метрах и составлять 50 метров.</span><span class="sxs-lookup"><span data-stu-id="26863-115">As an example, the accuracy can be measured in meters, such as the latitude and longitude are accurate to within 50 meters.</span></span>|
|<span data-ttu-id="26863-116">altitude</span><span class="sxs-lookup"><span data-stu-id="26863-116">altitude</span></span>|<span data-ttu-id="26863-117">double</span><span class="sxs-lookup"><span data-stu-id="26863-117">double</span></span>|<span data-ttu-id="26863-118">Высота местоположения.</span><span class="sxs-lookup"><span data-stu-id="26863-118">The altitude of the location.</span></span>|
|<span data-ttu-id="26863-119">altitudeAccuracy</span><span class="sxs-lookup"><span data-stu-id="26863-119">altitudeAccuracy</span></span>|<span data-ttu-id="26863-120">double</span><span class="sxs-lookup"><span data-stu-id="26863-120">double</span></span>|<span data-ttu-id="26863-121">Точность высоты.</span><span class="sxs-lookup"><span data-stu-id="26863-121">The accuracy of the altitude.</span></span>|
|<span data-ttu-id="26863-122">latitude</span><span class="sxs-lookup"><span data-stu-id="26863-122">latitude</span></span>|<span data-ttu-id="26863-123">double</span><span class="sxs-lookup"><span data-stu-id="26863-123">double</span></span>|<span data-ttu-id="26863-124">Широта местоположения.</span><span class="sxs-lookup"><span data-stu-id="26863-124">The latitude of the location.</span></span>|
|<span data-ttu-id="26863-125">longitude</span><span class="sxs-lookup"><span data-stu-id="26863-125">longitude</span></span>|<span data-ttu-id="26863-126">double</span><span class="sxs-lookup"><span data-stu-id="26863-126">double</span></span>|<span data-ttu-id="26863-127">Долгота местоположения.</span><span class="sxs-lookup"><span data-stu-id="26863-127">The longitude of the location.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "outlookGeoCoordinates resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
