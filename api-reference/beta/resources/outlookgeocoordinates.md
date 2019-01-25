---
title: Тип ресурса outlookGeoCoordinates
description: Географические координаты, высота и точность физического местоположения.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 7ca63aa3df6a597aaacb81fbeacf275ac87064f1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511837"
---
# <a name="outlookgeocoordinates-resource-type"></a><span data-ttu-id="d0489-103">Тип ресурса outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="d0489-103">outlookGeoCoordinates resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0489-104">Географические координаты, высота и точность физического местоположения.</span><span class="sxs-lookup"><span data-stu-id="d0489-104">The geographic coordinates, elevation, and their degree of accuracy for a physical location.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d0489-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d0489-105">JSON representation</span></span>

<span data-ttu-id="d0489-106">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d0489-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="d0489-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="d0489-107">Properties</span></span>
| <span data-ttu-id="d0489-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="d0489-108">Property</span></span>     | <span data-ttu-id="d0489-109">Тип</span><span class="sxs-lookup"><span data-stu-id="d0489-109">Type</span></span>   |<span data-ttu-id="d0489-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d0489-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d0489-111">accuracy</span><span class="sxs-lookup"><span data-stu-id="d0489-111">accuracy</span></span>|<span data-ttu-id="d0489-112">double</span><span class="sxs-lookup"><span data-stu-id="d0489-112">double</span></span>|<span data-ttu-id="d0489-113">Точность широты и долготы.</span><span class="sxs-lookup"><span data-stu-id="d0489-113">The accuracy of the latitude and longitude.</span></span> <span data-ttu-id="d0489-114">Например, точность может измеряться в метрах и составлять 50 метров.</span><span class="sxs-lookup"><span data-stu-id="d0489-114">As an example, the accuracy can be measured in meters, such as the latitude and longitude are accurate to within 50 meters.</span></span>|
|<span data-ttu-id="d0489-115">altitude</span><span class="sxs-lookup"><span data-stu-id="d0489-115">altitude</span></span>|<span data-ttu-id="d0489-116">double</span><span class="sxs-lookup"><span data-stu-id="d0489-116">double</span></span>|<span data-ttu-id="d0489-117">Высота местоположения.</span><span class="sxs-lookup"><span data-stu-id="d0489-117">The altitude of the location.</span></span>|
|<span data-ttu-id="d0489-118">altitudeAccuracy</span><span class="sxs-lookup"><span data-stu-id="d0489-118">altitudeAccuracy</span></span>|<span data-ttu-id="d0489-119">double</span><span class="sxs-lookup"><span data-stu-id="d0489-119">double</span></span>|<span data-ttu-id="d0489-120">Точность высоты.</span><span class="sxs-lookup"><span data-stu-id="d0489-120">The accuracy of the altitude.</span></span>|
|<span data-ttu-id="d0489-121">latitude</span><span class="sxs-lookup"><span data-stu-id="d0489-121">latitude</span></span>|<span data-ttu-id="d0489-122">double</span><span class="sxs-lookup"><span data-stu-id="d0489-122">double</span></span>|<span data-ttu-id="d0489-123">Широта местоположения.</span><span class="sxs-lookup"><span data-stu-id="d0489-123">The latitude of the location.</span></span>|
|<span data-ttu-id="d0489-124">longitude</span><span class="sxs-lookup"><span data-stu-id="d0489-124">longitude</span></span>|<span data-ttu-id="d0489-125">double</span><span class="sxs-lookup"><span data-stu-id="d0489-125">double</span></span>|<span data-ttu-id="d0489-126">Долгота местоположения.</span><span class="sxs-lookup"><span data-stu-id="d0489-126">The longitude of the location.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "outlookGeoCoordinates resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/outlookgeocoordinates.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
