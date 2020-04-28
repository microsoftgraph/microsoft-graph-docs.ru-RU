---
author: JeremyKelley
description: Ресурс "геокоординаты" предоставляет географические координаты и возвышение расположения на основе метаданных, содержащихся в файле.
ms.date: 09/10/2017
title: GeoCoordinates
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 07b0a39155b8c9c4dc02d6cff1e0a93c1a9cd418
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42497638"
---
# <a name="geocoordinates-resource-type"></a><span data-ttu-id="218fe-103">Тип ресурса "геокоординаты"</span><span class="sxs-lookup"><span data-stu-id="218fe-103">geoCoordinates resource type</span></span>

<span data-ttu-id="218fe-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="218fe-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="218fe-105">Предоставляет географические координаты и расширение расположения на основе метаданных, содержащихся в файле.</span><span class="sxs-lookup"><span data-stu-id="218fe-105">Provides geographic coordinates and elevation of a location based on metadata contained within the file.</span></span>
<span data-ttu-id="218fe-106">Если [**driveItem**](driveitem.md) имеет аспект **Location** , отличный от NULL, элемент представляет файл с известным расположением связанной с ним.</span><span class="sxs-lookup"><span data-stu-id="218fe-106">If a [**driveItem**](driveitem.md) has a non-null **location** facet, the item represents a file with a known location assocaited with it.</span></span>

> [!NOTE]
> <span data-ttu-id="218fe-107">При обновлении широты и долготы фотографии необходимо указать ресурс [Photo](photo.md) (пустой или другой).</span><span class="sxs-lookup"><span data-stu-id="218fe-107">When updating the latitude and longitude of a photo, a [photo](photo.md) resource (empty or otherwise) must be provided.</span></span>

## <a name="properties"></a><span data-ttu-id="218fe-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="218fe-108">Properties</span></span>

| <span data-ttu-id="218fe-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="218fe-109">Property</span></span>  | <span data-ttu-id="218fe-110">Тип</span><span class="sxs-lookup"><span data-stu-id="218fe-110">Type</span></span>   | <span data-ttu-id="218fe-111">Описание</span><span class="sxs-lookup"><span data-stu-id="218fe-111">Description</span></span>
|:----------|:-------|:--------------------------------------------------------
| <span data-ttu-id="218fe-112">altitude</span><span class="sxs-lookup"><span data-stu-id="218fe-112">altitude</span></span>  | <span data-ttu-id="218fe-113">Double</span><span class="sxs-lookup"><span data-stu-id="218fe-113">Double</span></span> | <span data-ttu-id="218fe-p102">Необязательный. Высота элемента над уровнем моря (в футах). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="218fe-p102">Optional. The altitude (height), in feet,  above sea level for the item. Read-only.</span></span>
| <span data-ttu-id="218fe-117">latitude</span><span class="sxs-lookup"><span data-stu-id="218fe-117">latitude</span></span>  | <span data-ttu-id="218fe-118">Double</span><span class="sxs-lookup"><span data-stu-id="218fe-118">Double</span></span> | <span data-ttu-id="218fe-119">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="218fe-119">Optional.</span></span> <span data-ttu-id="218fe-120">Широта элемента (в десятичной системе).</span><span class="sxs-lookup"><span data-stu-id="218fe-120">The latitude, in decimal, for the item.</span></span> <span data-ttu-id="218fe-121">Возможность записи в OneDrive персональный.</span><span class="sxs-lookup"><span data-stu-id="218fe-121">Writable on OneDrive Personal.</span></span>
| <span data-ttu-id="218fe-122">longitude</span><span class="sxs-lookup"><span data-stu-id="218fe-122">longitude</span></span> | <span data-ttu-id="218fe-123">Double</span><span class="sxs-lookup"><span data-stu-id="218fe-123">Double</span></span> | <span data-ttu-id="218fe-124">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="218fe-124">Optional.</span></span> <span data-ttu-id="218fe-125">Широта элемента (в десятичном виде).</span><span class="sxs-lookup"><span data-stu-id="218fe-125">The longitude, in decimal, for the item.</span></span> <span data-ttu-id="218fe-126">Возможность записи в OneDrive персональный.</span><span class="sxs-lookup"><span data-stu-id="218fe-126">Writable on OneDrive Personal.</span></span>

## <a name="json-representation"></a><span data-ttu-id="218fe-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="218fe-127">JSON representation</span></span>

<span data-ttu-id="218fe-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="218fe-128">Here is a JSON representation of the resource</span></span>

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
