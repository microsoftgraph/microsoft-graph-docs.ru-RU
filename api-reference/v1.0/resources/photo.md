---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Photo
localization_priority: Normal
description: Ресурс photo предоставляет свойства фотографии и камеры, например метаданные EXIF, в ресурсе driveItem.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: a62a138cbd48645b6b296abcde72af0cef19e259
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863735"
---
# <a name="photo-resource-type"></a><span data-ttu-id="0bbec-103">Тип ресурса Photo</span><span class="sxs-lookup"><span data-stu-id="0bbec-103">Photo resource type</span></span>

<span data-ttu-id="0bbec-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0bbec-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0bbec-105">Ресурс **photo** предоставляет свойства фотографии и камеры, например метаданные EXIF, в ресурсе [driveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="0bbec-105">The **photo** resource provides photo and camera properties, for example, EXIF metadata, on a [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="0bbec-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0bbec-106">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.photo"
}-->

```json
{
  "cameraMake": "string",
  "cameraModel": "string",
  "exposureDenominator": 1000.0,
  "exposureNumerator": 1.0,
  "fNumber": 1.8,
  "focalLength": 22.5,
  "iso": 100,
  "orientation": 3,
  "takenDateTime": "String (timestamp)"
}
```

## <a name="properties"></a><span data-ttu-id="0bbec-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="0bbec-107">Properties</span></span>

| <span data-ttu-id="0bbec-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="0bbec-108">Property</span></span>                | <span data-ttu-id="0bbec-109">Тип</span><span class="sxs-lookup"><span data-stu-id="0bbec-109">Type</span></span>           | <span data-ttu-id="0bbec-110">Описание</span><span class="sxs-lookup"><span data-stu-id="0bbec-110">Description</span></span>
|:------------------------|:---------------|:----------------------------------
| <span data-ttu-id="0bbec-111">**takenDateTime**</span><span class="sxs-lookup"><span data-stu-id="0bbec-111">**takenDateTime**</span></span>       | <span data-ttu-id="0bbec-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0bbec-112">DateTimeOffset</span></span> | <span data-ttu-id="0bbec-113">Represents the date and time the photo was taken.</span><span class="sxs-lookup"><span data-stu-id="0bbec-113">Represents the date and time the photo was taken.</span></span> <span data-ttu-id="0bbec-114">Read-only.</span><span class="sxs-lookup"><span data-stu-id="0bbec-114">Read-only.</span></span>
| <span data-ttu-id="0bbec-115">**cameraMake**</span><span class="sxs-lookup"><span data-stu-id="0bbec-115">**cameraMake**</span></span>          | <span data-ttu-id="0bbec-116">Строка</span><span class="sxs-lookup"><span data-stu-id="0bbec-116">String</span></span>         | <span data-ttu-id="0bbec-117">Camera manufacturer.</span><span class="sxs-lookup"><span data-stu-id="0bbec-117">Camera manufacturer.</span></span> <span data-ttu-id="0bbec-118">Read-only.</span><span class="sxs-lookup"><span data-stu-id="0bbec-118">Read-only.</span></span>
| <span data-ttu-id="0bbec-119">**cameraModel**</span><span class="sxs-lookup"><span data-stu-id="0bbec-119">**cameraModel**</span></span>         | <span data-ttu-id="0bbec-120">String</span><span class="sxs-lookup"><span data-stu-id="0bbec-120">String</span></span>         | <span data-ttu-id="0bbec-121">Camera model.</span><span class="sxs-lookup"><span data-stu-id="0bbec-121">Camera model.</span></span> <span data-ttu-id="0bbec-122">Read-only.</span><span class="sxs-lookup"><span data-stu-id="0bbec-122">Read-only.</span></span>
| <span data-ttu-id="0bbec-123">**fNumber**</span><span class="sxs-lookup"><span data-stu-id="0bbec-123">**fNumber**</span></span>             | <span data-ttu-id="0bbec-124">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="0bbec-124">Double</span></span>         | <span data-ttu-id="0bbec-125">The F-stop value from the camera.</span><span class="sxs-lookup"><span data-stu-id="0bbec-125">The F-stop value from the camera.</span></span> <span data-ttu-id="0bbec-126">Read-only.</span><span class="sxs-lookup"><span data-stu-id="0bbec-126">Read-only.</span></span>
| <span data-ttu-id="0bbec-127">**exposureDenominator**</span><span class="sxs-lookup"><span data-stu-id="0bbec-127">**exposureDenominator**</span></span> | <span data-ttu-id="0bbec-128">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="0bbec-128">Double</span></span>         | <span data-ttu-id="0bbec-129">The denominator for the exposure time fraction from the camera.</span><span class="sxs-lookup"><span data-stu-id="0bbec-129">The denominator for the exposure time fraction from the camera.</span></span> <span data-ttu-id="0bbec-130">Read-only.</span><span class="sxs-lookup"><span data-stu-id="0bbec-130">Read-only.</span></span>
| <span data-ttu-id="0bbec-131">**exposureNumerator**</span><span class="sxs-lookup"><span data-stu-id="0bbec-131">**exposureNumerator**</span></span>   | <span data-ttu-id="0bbec-132">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="0bbec-132">Double</span></span>         | <span data-ttu-id="0bbec-133">The numerator for the exposure time fraction from the camera.</span><span class="sxs-lookup"><span data-stu-id="0bbec-133">The numerator for the exposure time fraction from the camera.</span></span> <span data-ttu-id="0bbec-134">Read-only.</span><span class="sxs-lookup"><span data-stu-id="0bbec-134">Read-only.</span></span>
| <span data-ttu-id="0bbec-135">**focalLength**</span><span class="sxs-lookup"><span data-stu-id="0bbec-135">**focalLength**</span></span>         | <span data-ttu-id="0bbec-136">Double</span><span class="sxs-lookup"><span data-stu-id="0bbec-136">Double</span></span>         | <span data-ttu-id="0bbec-137">The focal length from the camera.</span><span class="sxs-lookup"><span data-stu-id="0bbec-137">The focal length from the camera.</span></span> <span data-ttu-id="0bbec-138">Read-only.</span><span class="sxs-lookup"><span data-stu-id="0bbec-138">Read-only.</span></span>
| <span data-ttu-id="0bbec-139">**iso**</span><span class="sxs-lookup"><span data-stu-id="0bbec-139">**iso**</span></span>                 | <span data-ttu-id="0bbec-140">Int32</span><span class="sxs-lookup"><span data-stu-id="0bbec-140">Int32</span></span>          | <span data-ttu-id="0bbec-141">The ISO value from the camera.</span><span class="sxs-lookup"><span data-stu-id="0bbec-141">The ISO value from the camera.</span></span> <span data-ttu-id="0bbec-142">Read-only.</span><span class="sxs-lookup"><span data-stu-id="0bbec-142">Read-only.</span></span>
| <span data-ttu-id="0bbec-143">**orientation**</span><span class="sxs-lookup"><span data-stu-id="0bbec-143">**orientation**</span></span>         | <span data-ttu-id="0bbec-144">Int16</span><span class="sxs-lookup"><span data-stu-id="0bbec-144">Int16</span></span>          | <span data-ttu-id="0bbec-145">Значение ориентации камеры.</span><span class="sxs-lookup"><span data-stu-id="0bbec-145">The orientation value from the camera.</span></span> <span data-ttu-id="0bbec-146">Возможность записи в OneDrive персональный.</span><span class="sxs-lookup"><span data-stu-id="0bbec-146">Writable on OneDrive Personal.</span></span>      |

## <a name="remarks"></a><span data-ttu-id="0bbec-147">Заметки</span><span class="sxs-lookup"><span data-stu-id="0bbec-147">Remarks</span></span>

<span data-ttu-id="0bbec-148">OneDrive для бизнеса и SharePoint возвращают только свойство **takenDateTime**.</span><span class="sxs-lookup"><span data-stu-id="0bbec-148">OneDrive for Business and SharePoint only return the **takenDateTime** property.</span></span>

<span data-ttu-id="0bbec-149">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="0bbec-149">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>
<!-- {
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso, orientation",
  "section": "documentation",
  "tocPath": "Facets/Photo"
} -->
