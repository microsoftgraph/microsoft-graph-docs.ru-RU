---
title: Тип ресурса outlookGeoCoordinates
description: Географические координаты, высота и точность физического местоположения.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: f51f5eeb663a1d1ce55bee083639d244905b2c37
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27973120"
---
# <a name="outlookgeocoordinates-resource-type"></a><span data-ttu-id="7b277-103">Тип ресурса outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="7b277-103">outlookGeoCoordinates resource type</span></span>

> <span data-ttu-id="7b277-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7b277-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7b277-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b277-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7b277-106">Географические координаты, высота и точность физического местоположения.</span><span class="sxs-lookup"><span data-stu-id="7b277-106">The geographic coordinates, elevation, and their degree of accuracy for a physical location.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7b277-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7b277-107">JSON representation</span></span>

<span data-ttu-id="7b277-108">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7b277-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="7b277-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="7b277-109">Properties</span></span>
| <span data-ttu-id="7b277-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="7b277-110">Property</span></span>     | <span data-ttu-id="7b277-111">Тип</span><span class="sxs-lookup"><span data-stu-id="7b277-111">Type</span></span>   |<span data-ttu-id="7b277-112">Описание</span><span class="sxs-lookup"><span data-stu-id="7b277-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7b277-113">accuracy</span><span class="sxs-lookup"><span data-stu-id="7b277-113">accuracy</span></span>|<span data-ttu-id="7b277-114">double</span><span class="sxs-lookup"><span data-stu-id="7b277-114">double</span></span>|<span data-ttu-id="7b277-115">Точность широты и долготы.</span><span class="sxs-lookup"><span data-stu-id="7b277-115">The accuracy of the latitude and longitude.</span></span> <span data-ttu-id="7b277-116">Например, точность может измеряться в метрах и составлять 50 метров.</span><span class="sxs-lookup"><span data-stu-id="7b277-116">As an example, the accuracy can be measured in meters, such as the latitude and longitude are accurate to within 50 meters.</span></span>|
|<span data-ttu-id="7b277-117">altitude</span><span class="sxs-lookup"><span data-stu-id="7b277-117">altitude</span></span>|<span data-ttu-id="7b277-118">double</span><span class="sxs-lookup"><span data-stu-id="7b277-118">double</span></span>|<span data-ttu-id="7b277-119">Высота местоположения.</span><span class="sxs-lookup"><span data-stu-id="7b277-119">The altitude of the location.</span></span>|
|<span data-ttu-id="7b277-120">altitudeAccuracy</span><span class="sxs-lookup"><span data-stu-id="7b277-120">altitudeAccuracy</span></span>|<span data-ttu-id="7b277-121">double</span><span class="sxs-lookup"><span data-stu-id="7b277-121">double</span></span>|<span data-ttu-id="7b277-122">Точность высоты.</span><span class="sxs-lookup"><span data-stu-id="7b277-122">The accuracy of the altitude.</span></span>|
|<span data-ttu-id="7b277-123">latitude</span><span class="sxs-lookup"><span data-stu-id="7b277-123">latitude</span></span>|<span data-ttu-id="7b277-124">double</span><span class="sxs-lookup"><span data-stu-id="7b277-124">double</span></span>|<span data-ttu-id="7b277-125">Широта местоположения.</span><span class="sxs-lookup"><span data-stu-id="7b277-125">The latitude of the location.</span></span>|
|<span data-ttu-id="7b277-126">longitude</span><span class="sxs-lookup"><span data-stu-id="7b277-126">longitude</span></span>|<span data-ttu-id="7b277-127">double</span><span class="sxs-lookup"><span data-stu-id="7b277-127">double</span></span>|<span data-ttu-id="7b277-128">Долгота местоположения.</span><span class="sxs-lookup"><span data-stu-id="7b277-128">The longitude of the location.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookGeoCoordinates resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
