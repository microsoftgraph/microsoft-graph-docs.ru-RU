---
title: Тип ресурса outlookGeoCoordinates
description: Географические координаты, высота и точность физического местоположения.
ms.openlocfilehash: 9de60c218f6fc54ed2be12b2987126195e5eb140
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076977"
---
# <a name="outlookgeocoordinates-resource-type"></a><span data-ttu-id="2f32a-103">Тип ресурса outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="2f32a-103">outlookGeoCoordinates resource type</span></span>

> <span data-ttu-id="2f32a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2f32a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2f32a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f32a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2f32a-106">Географические координаты, высота и точность физического местоположения.</span><span class="sxs-lookup"><span data-stu-id="2f32a-106">The geographic coordinates, elevation, and their degree of accuracy for a physical location.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2f32a-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2f32a-107">JSON representation</span></span>

<span data-ttu-id="2f32a-108">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2f32a-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="2f32a-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="2f32a-109">Properties</span></span>
| <span data-ttu-id="2f32a-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="2f32a-110">Property</span></span>     | <span data-ttu-id="2f32a-111">Тип</span><span class="sxs-lookup"><span data-stu-id="2f32a-111">Type</span></span>   |<span data-ttu-id="2f32a-112">Описание</span><span class="sxs-lookup"><span data-stu-id="2f32a-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2f32a-113">accuracy</span><span class="sxs-lookup"><span data-stu-id="2f32a-113">accuracy</span></span>|<span data-ttu-id="2f32a-114">double</span><span class="sxs-lookup"><span data-stu-id="2f32a-114">double</span></span>|<span data-ttu-id="2f32a-115">Точность широты и долготы.</span><span class="sxs-lookup"><span data-stu-id="2f32a-115">The accuracy of the latitude and longitude.</span></span> <span data-ttu-id="2f32a-116">Например, точность может измеряться в метрах и составлять 50 метров.</span><span class="sxs-lookup"><span data-stu-id="2f32a-116">As an example, the accuracy can be measured in meters, such as the latitude and longitude are accurate to within 50 meters.</span></span>|
|<span data-ttu-id="2f32a-117">altitude</span><span class="sxs-lookup"><span data-stu-id="2f32a-117">altitude</span></span>|<span data-ttu-id="2f32a-118">double</span><span class="sxs-lookup"><span data-stu-id="2f32a-118">double</span></span>|<span data-ttu-id="2f32a-119">Высота местоположения.</span><span class="sxs-lookup"><span data-stu-id="2f32a-119">The altitude of the location.</span></span>|
|<span data-ttu-id="2f32a-120">altitudeAccuracy</span><span class="sxs-lookup"><span data-stu-id="2f32a-120">altitudeAccuracy</span></span>|<span data-ttu-id="2f32a-121">double</span><span class="sxs-lookup"><span data-stu-id="2f32a-121">double</span></span>|<span data-ttu-id="2f32a-122">Точность высоты.</span><span class="sxs-lookup"><span data-stu-id="2f32a-122">The accuracy of the altitude.</span></span>|
|<span data-ttu-id="2f32a-123">latitude</span><span class="sxs-lookup"><span data-stu-id="2f32a-123">latitude</span></span>|<span data-ttu-id="2f32a-124">double</span><span class="sxs-lookup"><span data-stu-id="2f32a-124">double</span></span>|<span data-ttu-id="2f32a-125">Широта местоположения.</span><span class="sxs-lookup"><span data-stu-id="2f32a-125">The latitude of the location.</span></span>|
|<span data-ttu-id="2f32a-126">longitude</span><span class="sxs-lookup"><span data-stu-id="2f32a-126">longitude</span></span>|<span data-ttu-id="2f32a-127">double</span><span class="sxs-lookup"><span data-stu-id="2f32a-127">double</span></span>|<span data-ttu-id="2f32a-128">Долгота местоположения.</span><span class="sxs-lookup"><span data-stu-id="2f32a-128">The longitude of the location.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookGeoCoordinates resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->