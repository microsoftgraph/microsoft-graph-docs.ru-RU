---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Фотография
localization_priority: Normal
ms.openlocfilehash: 688bee72464c1e518c60720a7f9ca24da1f7d149
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480980"
---
# <a name="photo-resource-type"></a><span data-ttu-id="deb1a-102">Тип ресурса Photo</span><span class="sxs-lookup"><span data-stu-id="deb1a-102">Photo resource type</span></span>

<span data-ttu-id="deb1a-103">Ресурс **photo** предоставляет свойства фотографии и камеры, например метаданные EXIF, в ресурсе [driveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="deb1a-103">The **photo** resource provides photo and camera properties, for example, EXIF metadata, on a [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="deb1a-104">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="deb1a-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="deb1a-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="deb1a-105">Properties</span></span>

| <span data-ttu-id="deb1a-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="deb1a-106">Property</span></span>                | <span data-ttu-id="deb1a-107">Тип</span><span class="sxs-lookup"><span data-stu-id="deb1a-107">Type</span></span>           | <span data-ttu-id="deb1a-108">Описание</span><span class="sxs-lookup"><span data-stu-id="deb1a-108">Description</span></span>
|:------------------------|:---------------|:----------------------------------
| <span data-ttu-id="deb1a-109">**takenDateTime**</span><span class="sxs-lookup"><span data-stu-id="deb1a-109">**takenDateTime**</span></span>       | <span data-ttu-id="deb1a-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="deb1a-110">DateTimeOffset</span></span> | <span data-ttu-id="deb1a-p101">Представляет дату и время съемки. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="deb1a-p101">Represents the date and time the photo was taken. Read-only.</span></span>
| <span data-ttu-id="deb1a-113">**cameraMake**</span><span class="sxs-lookup"><span data-stu-id="deb1a-113">**cameraMake**</span></span>          | <span data-ttu-id="deb1a-114">Строка</span><span class="sxs-lookup"><span data-stu-id="deb1a-114">String</span></span>         | <span data-ttu-id="deb1a-p102">Изготовитель камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="deb1a-p102">Camera manufacturer. Read-only.</span></span>
| <span data-ttu-id="deb1a-117">**cameraModel**</span><span class="sxs-lookup"><span data-stu-id="deb1a-117">**cameraModel**</span></span>         | <span data-ttu-id="deb1a-118">String</span><span class="sxs-lookup"><span data-stu-id="deb1a-118">String</span></span>         | <span data-ttu-id="deb1a-p103">Модель камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="deb1a-p103">Camera model. Read-only.</span></span>
| <span data-ttu-id="deb1a-121">**fNumber**</span><span class="sxs-lookup"><span data-stu-id="deb1a-121">**fNumber**</span></span>             | <span data-ttu-id="deb1a-122">Double</span><span class="sxs-lookup"><span data-stu-id="deb1a-122">Double</span></span>         | <span data-ttu-id="deb1a-p104">Значение диафрагмы камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="deb1a-p104">The F-stop value from the camera. Read-only.</span></span>
| <span data-ttu-id="deb1a-125">**exposureDenominator**</span><span class="sxs-lookup"><span data-stu-id="deb1a-125">**exposureDenominator**</span></span> | <span data-ttu-id="deb1a-126">Double</span><span class="sxs-lookup"><span data-stu-id="deb1a-126">Double</span></span>         | <span data-ttu-id="deb1a-p105">Знаменатель дробного значения выдержки камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="deb1a-p105">The denominator for the exposure time fraction from the camera. Read-only.</span></span>
| <span data-ttu-id="deb1a-129">**exposureNumerator**</span><span class="sxs-lookup"><span data-stu-id="deb1a-129">**exposureNumerator**</span></span>   | <span data-ttu-id="deb1a-130">Double</span><span class="sxs-lookup"><span data-stu-id="deb1a-130">Double</span></span>         | <span data-ttu-id="deb1a-p106">Числитель дробного значения выдержки камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="deb1a-p106">The numerator for the exposure time fraction from the camera. Read-only.</span></span>
| <span data-ttu-id="deb1a-133">**focalLength**</span><span class="sxs-lookup"><span data-stu-id="deb1a-133">**focalLength**</span></span>         | <span data-ttu-id="deb1a-134">Double</span><span class="sxs-lookup"><span data-stu-id="deb1a-134">Double</span></span>         | <span data-ttu-id="deb1a-p107">Фокусное расстояние камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="deb1a-p107">The focal length from the camera. Read-only.</span></span>
| <span data-ttu-id="deb1a-137">**iso**</span><span class="sxs-lookup"><span data-stu-id="deb1a-137">**iso**</span></span>                 | <span data-ttu-id="deb1a-138">Int32</span><span class="sxs-lookup"><span data-stu-id="deb1a-138">Int32</span></span>          | <span data-ttu-id="deb1a-p108">Значение ISO камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="deb1a-p108">The ISO value from the camera. Read-only.</span></span>

## <a name="remarks"></a><span data-ttu-id="deb1a-141">Заметки</span><span class="sxs-lookup"><span data-stu-id="deb1a-141">Remarks</span></span>

<span data-ttu-id="deb1a-142">OneDrive для бизнеса и SharePoint возвращают только свойство **takenDateTime**.</span><span class="sxs-lookup"><span data-stu-id="deb1a-142">OneDrive for Business and SharePoint only return the **takenDateTime** property.</span></span>

<span data-ttu-id="deb1a-143">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="deb1a-143">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>
<!-- {
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso",
  "section": "documentation",
  "tocPath": "Facets/Photo"
} -->
