---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Фотография
localization_priority: Normal
description: Ресурс photo предоставляет свойства фотографии и камеры, например метаданные EXIF, в ресурсе driveItem.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: c86190768c10b04bb55f59104368089cf7c77b18
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035501"
---
# <a name="photo-resource-type"></a><span data-ttu-id="277fc-103">Тип ресурса Photo</span><span class="sxs-lookup"><span data-stu-id="277fc-103">Photo resource type</span></span>

<span data-ttu-id="277fc-104">Ресурс **photo** предоставляет свойства фотографии и камеры, например метаданные EXIF, в ресурсе [driveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="277fc-104">The **photo** resource provides photo and camera properties, for example, EXIF metadata, on a [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="277fc-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="277fc-105">JSON representation</span></span>

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
  "takenDateTime": "String (timestamp)"
}
```

## <a name="properties"></a><span data-ttu-id="277fc-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="277fc-106">Properties</span></span>

| <span data-ttu-id="277fc-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="277fc-107">Property</span></span>                | <span data-ttu-id="277fc-108">Тип</span><span class="sxs-lookup"><span data-stu-id="277fc-108">Type</span></span>           | <span data-ttu-id="277fc-109">Описание</span><span class="sxs-lookup"><span data-stu-id="277fc-109">Description</span></span>
|:------------------------|:---------------|:----------------------------------
| <span data-ttu-id="277fc-110">**takenDateTime**</span><span class="sxs-lookup"><span data-stu-id="277fc-110">**takenDateTime**</span></span>       | <span data-ttu-id="277fc-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="277fc-111">DateTimeOffset</span></span> | <span data-ttu-id="277fc-p101">Представляет дату и время съемки. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="277fc-p101">Represents the date and time the photo was taken. Read-only.</span></span>
| <span data-ttu-id="277fc-114">**cameraMake**</span><span class="sxs-lookup"><span data-stu-id="277fc-114">**cameraMake**</span></span>          | <span data-ttu-id="277fc-115">Строка</span><span class="sxs-lookup"><span data-stu-id="277fc-115">String</span></span>         | <span data-ttu-id="277fc-p102">Изготовитель камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="277fc-p102">Camera manufacturer. Read-only.</span></span>
| <span data-ttu-id="277fc-118">**cameraModel**</span><span class="sxs-lookup"><span data-stu-id="277fc-118">**cameraModel**</span></span>         | <span data-ttu-id="277fc-119">String</span><span class="sxs-lookup"><span data-stu-id="277fc-119">String</span></span>         | <span data-ttu-id="277fc-p103">Модель камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="277fc-p103">Camera model. Read-only.</span></span>
| <span data-ttu-id="277fc-122">**fNumber**</span><span class="sxs-lookup"><span data-stu-id="277fc-122">**fNumber**</span></span>             | <span data-ttu-id="277fc-123">Двойное</span><span class="sxs-lookup"><span data-stu-id="277fc-123">Double</span></span>         | <span data-ttu-id="277fc-p104">Значение диафрагмы камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="277fc-p104">The F-stop value from the camera. Read-only.</span></span>
| <span data-ttu-id="277fc-126">**exposureDenominator**</span><span class="sxs-lookup"><span data-stu-id="277fc-126">**exposureDenominator**</span></span> | <span data-ttu-id="277fc-127">Двойное</span><span class="sxs-lookup"><span data-stu-id="277fc-127">Double</span></span>         | <span data-ttu-id="277fc-p105">Знаменатель дробного значения выдержки камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="277fc-p105">The denominator for the exposure time fraction from the camera. Read-only.</span></span>
| <span data-ttu-id="277fc-130">**exposureNumerator**</span><span class="sxs-lookup"><span data-stu-id="277fc-130">**exposureNumerator**</span></span>   | <span data-ttu-id="277fc-131">Двойное</span><span class="sxs-lookup"><span data-stu-id="277fc-131">Double</span></span>         | <span data-ttu-id="277fc-p106">Числитель дробного значения выдержки камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="277fc-p106">The numerator for the exposure time fraction from the camera. Read-only.</span></span>
| <span data-ttu-id="277fc-134">**focalLength**</span><span class="sxs-lookup"><span data-stu-id="277fc-134">**focalLength**</span></span>         | <span data-ttu-id="277fc-135">Double</span><span class="sxs-lookup"><span data-stu-id="277fc-135">Double</span></span>         | <span data-ttu-id="277fc-p107">Фокусное расстояние камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="277fc-p107">The focal length from the camera. Read-only.</span></span>
| <span data-ttu-id="277fc-138">**iso**</span><span class="sxs-lookup"><span data-stu-id="277fc-138">**iso**</span></span>                 | <span data-ttu-id="277fc-139">Int32</span><span class="sxs-lookup"><span data-stu-id="277fc-139">Int32</span></span>          | <span data-ttu-id="277fc-p108">Значение ISO камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="277fc-p108">The ISO value from the camera. Read-only.</span></span>

## <a name="remarks"></a><span data-ttu-id="277fc-142">Заметки</span><span class="sxs-lookup"><span data-stu-id="277fc-142">Remarks</span></span>

<span data-ttu-id="277fc-143">OneDrive для бизнеса и SharePoint возвращают только свойство **takenDateTime**.</span><span class="sxs-lookup"><span data-stu-id="277fc-143">OneDrive for Business and SharePoint only return the **takenDateTime** property.</span></span>

<span data-ttu-id="277fc-144">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="277fc-144">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>
<!-- {
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso",
  "section": "documentation",
  "tocPath": "Facets/Photo"
} -->
