---
author: JeremyKelley
description: Ресурс "геокоординаты" предоставляет географические координаты и возвышение расположения на основе метаданных, содержащихся в файле.
ms.date: 09/10/2017
title: GeoCoordinates
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 86de97358591df8dc446b91d0be7a8192c7346f8
ms.sourcegitcommit: 2fb178ae78b5ecc47207d2b19d0c5a46e07e0960
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2019
ms.locfileid: "37333257"
---
# <a name="geocoordinates-resource-type"></a><span data-ttu-id="03efa-103">Тип ресурса "геокоординаты"</span><span class="sxs-lookup"><span data-stu-id="03efa-103">geoCoordinates resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="03efa-104">Предоставляет географические координаты и расширение расположения на основе метаданных, содержащихся в файле.</span><span class="sxs-lookup"><span data-stu-id="03efa-104">Provides geographic coordinates and elevation of a location based on metadata contained within the file.</span></span>
<span data-ttu-id="03efa-105">Если [**driveItem**](driveitem.md) имеет аспект **Location** , отличный от NULL, элемент представляет файл с известным расположением связанной с ним.</span><span class="sxs-lookup"><span data-stu-id="03efa-105">If a [**driveItem**](driveitem.md) has a non-null **location** facet, the item represents a file with a known location assocaited with it.</span></span>

> [!NOTE]
> <span data-ttu-id="03efa-106">При обновлении широты и долготы фотографии необходимо указать ресурс [Photo](photo.md) (пустой или другой).</span><span class="sxs-lookup"><span data-stu-id="03efa-106">When updating the latitude and longitude of a photo, a [photo](photo.md) resource (empty or otherwise) must be provided.</span></span>

## <a name="properties"></a><span data-ttu-id="03efa-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="03efa-107">Properties</span></span>

| <span data-ttu-id="03efa-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="03efa-108">Property</span></span>  | <span data-ttu-id="03efa-109">Тип</span><span class="sxs-lookup"><span data-stu-id="03efa-109">Type</span></span>   | <span data-ttu-id="03efa-110">Описание</span><span class="sxs-lookup"><span data-stu-id="03efa-110">Description</span></span>
|:----------|:-------|:--------------------------------------------------------
| <span data-ttu-id="03efa-111">altitude</span><span class="sxs-lookup"><span data-stu-id="03efa-111">altitude</span></span>  | <span data-ttu-id="03efa-112">Double</span><span class="sxs-lookup"><span data-stu-id="03efa-112">Double</span></span> | <span data-ttu-id="03efa-p102">Необязательный. Высота элемента над уровнем моря (в футах). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="03efa-p102">Optional. The altitude (height), in feet,  above sea level for the item. Read-only.</span></span>
| <span data-ttu-id="03efa-116">latitude</span><span class="sxs-lookup"><span data-stu-id="03efa-116">latitude</span></span>  | <span data-ttu-id="03efa-117">Double</span><span class="sxs-lookup"><span data-stu-id="03efa-117">Double</span></span> | <span data-ttu-id="03efa-118">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="03efa-118">Optional.</span></span> <span data-ttu-id="03efa-119">Широта элемента (в десятичной системе).</span><span class="sxs-lookup"><span data-stu-id="03efa-119">The latitude, in decimal, for the item.</span></span> <span data-ttu-id="03efa-120">Возможность записи в OneDrive персональный.</span><span class="sxs-lookup"><span data-stu-id="03efa-120">Writable on OneDrive Personal.</span></span>
| <span data-ttu-id="03efa-121">longitude</span><span class="sxs-lookup"><span data-stu-id="03efa-121">longitude</span></span> | <span data-ttu-id="03efa-122">Double</span><span class="sxs-lookup"><span data-stu-id="03efa-122">Double</span></span> | <span data-ttu-id="03efa-123">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="03efa-123">Optional.</span></span> <span data-ttu-id="03efa-124">Широта элемента (в десятичном виде).</span><span class="sxs-lookup"><span data-stu-id="03efa-124">The longitude, in decimal, for the item.</span></span> <span data-ttu-id="03efa-125">Возможность записи в OneDrive персональный.</span><span class="sxs-lookup"><span data-stu-id="03efa-125">Writable on OneDrive Personal.</span></span>

## <a name="json-representation"></a><span data-ttu-id="03efa-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="03efa-126">JSON representation</span></span>

<span data-ttu-id="03efa-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="03efa-127">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.geoCoordinates"
}-->

```json
{
  "altitude": 1024.13,
  "latitude": 26.13246,
  "longitude": 24.34616
}
```

<!--
{
  "type": "#page.annotation",
  "description": "The location facet provides geographic location related properties for an item",
  "keywords": "location,geographic,item,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Location",
  "suppressions": []
}
-->
