---
title: Тип ресурса outlookGeoCoordinates
description: Географические координаты, высота и точность физического местоположения.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 6cfa08c15318fdaa58ac71e01a940b621b207f12
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035674"
---
# <a name="outlookgeocoordinates-resource-type"></a><span data-ttu-id="1094c-103">Тип ресурса outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="1094c-103">outlookGeoCoordinates resource type</span></span>

<span data-ttu-id="1094c-104">Географические координаты, высота и точность физического местоположения.</span><span class="sxs-lookup"><span data-stu-id="1094c-104">The geographic coordinates, elevation, and their degree of accuracy for a physical location.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1094c-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1094c-105">JSON representation</span></span>

<span data-ttu-id="1094c-106">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1094c-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="1094c-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="1094c-107">Properties</span></span>
| <span data-ttu-id="1094c-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="1094c-108">Property</span></span>     | <span data-ttu-id="1094c-109">Тип</span><span class="sxs-lookup"><span data-stu-id="1094c-109">Type</span></span>   |<span data-ttu-id="1094c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1094c-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1094c-111">accuracy</span><span class="sxs-lookup"><span data-stu-id="1094c-111">accuracy</span></span>|<span data-ttu-id="1094c-112">double</span><span class="sxs-lookup"><span data-stu-id="1094c-112">double</span></span>|<span data-ttu-id="1094c-113">Точность широты и долготы.</span><span class="sxs-lookup"><span data-stu-id="1094c-113">The accuracy of the latitude and longitude.</span></span> <span data-ttu-id="1094c-114">Например, точность может измеряться в метрах и составлять 50 метров.</span><span class="sxs-lookup"><span data-stu-id="1094c-114">As an example, the accuracy can be measured in meters, such as the latitude and longitude are accurate to within 50 meters.</span></span>|
|<span data-ttu-id="1094c-115">altitude</span><span class="sxs-lookup"><span data-stu-id="1094c-115">altitude</span></span>|<span data-ttu-id="1094c-116">double</span><span class="sxs-lookup"><span data-stu-id="1094c-116">double</span></span>|<span data-ttu-id="1094c-117">Высота местоположения.</span><span class="sxs-lookup"><span data-stu-id="1094c-117">The altitude of the location.</span></span>|
|<span data-ttu-id="1094c-118">altitudeAccuracy</span><span class="sxs-lookup"><span data-stu-id="1094c-118">altitudeAccuracy</span></span>|<span data-ttu-id="1094c-119">double</span><span class="sxs-lookup"><span data-stu-id="1094c-119">double</span></span>|<span data-ttu-id="1094c-120">Точность высоты.</span><span class="sxs-lookup"><span data-stu-id="1094c-120">The accuracy of the altitude.</span></span>|
|<span data-ttu-id="1094c-121">latitude</span><span class="sxs-lookup"><span data-stu-id="1094c-121">latitude</span></span>|<span data-ttu-id="1094c-122">double</span><span class="sxs-lookup"><span data-stu-id="1094c-122">double</span></span>|<span data-ttu-id="1094c-123">Широта местоположения.</span><span class="sxs-lookup"><span data-stu-id="1094c-123">The latitude of the location.</span></span>|
|<span data-ttu-id="1094c-124">longitude</span><span class="sxs-lookup"><span data-stu-id="1094c-124">longitude</span></span>|<span data-ttu-id="1094c-125">double</span><span class="sxs-lookup"><span data-stu-id="1094c-125">double</span></span>|<span data-ttu-id="1094c-126">Долгота местоположения.</span><span class="sxs-lookup"><span data-stu-id="1094c-126">The longitude of the location.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookGeoCoordinates resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
