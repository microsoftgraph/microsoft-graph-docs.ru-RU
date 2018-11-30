---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Photo
ms.openlocfilehash: 391eafd84ab1abd4670c953720ff7097e060bfd3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027689"
---
# <a name="photo-resource-type"></a><span data-ttu-id="e88b8-102">Тип ресурса Photo</span><span class="sxs-lookup"><span data-stu-id="e88b8-102">Photo resource type</span></span>

<span data-ttu-id="e88b8-103">Ресурс **photo** предоставляет свойства фотографии и камеры, например метаданные EXIF, в ресурсе [driveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="e88b8-103">The **photo** resource provides photo and camera properties, for example, EXIF metadata, on a [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="e88b8-104">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e88b8-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="e88b8-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="e88b8-105">Properties</span></span>

| <span data-ttu-id="e88b8-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="e88b8-106">Property</span></span>                | <span data-ttu-id="e88b8-107">Тип</span><span class="sxs-lookup"><span data-stu-id="e88b8-107">Type</span></span>           | <span data-ttu-id="e88b8-108">Описание</span><span class="sxs-lookup"><span data-stu-id="e88b8-108">Description</span></span>
|:------------------------|:---------------|:----------------------------------
| <span data-ttu-id="e88b8-109">**takenDateTime**</span><span class="sxs-lookup"><span data-stu-id="e88b8-109">**takenDateTime**</span></span>       | <span data-ttu-id="e88b8-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e88b8-110">DateTimeOffset</span></span> | <span data-ttu-id="e88b8-p101">Представляет дату и время съемки. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e88b8-p101">Represents the date and time the photo was taken. Read-only.</span></span>
| <span data-ttu-id="e88b8-113">**cameraMake**</span><span class="sxs-lookup"><span data-stu-id="e88b8-113">**cameraMake**</span></span>          | <span data-ttu-id="e88b8-114">Строка</span><span class="sxs-lookup"><span data-stu-id="e88b8-114">String</span></span>         | <span data-ttu-id="e88b8-p102">Изготовитель камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e88b8-p102">Camera manufacturer. Read-only.</span></span>
| <span data-ttu-id="e88b8-117">**cameraModel**</span><span class="sxs-lookup"><span data-stu-id="e88b8-117">**cameraModel**</span></span>         | <span data-ttu-id="e88b8-118">String</span><span class="sxs-lookup"><span data-stu-id="e88b8-118">String</span></span>         | <span data-ttu-id="e88b8-p103">Модель камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e88b8-p103">Camera model. Read-only.</span></span>
| <span data-ttu-id="e88b8-121">**fNumber**</span><span class="sxs-lookup"><span data-stu-id="e88b8-121">**fNumber**</span></span>             | <span data-ttu-id="e88b8-122">Double</span><span class="sxs-lookup"><span data-stu-id="e88b8-122">Double</span></span>         | <span data-ttu-id="e88b8-p104">Значение диафрагмы камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e88b8-p104">The F-stop value from the camera. Read-only.</span></span>
| <span data-ttu-id="e88b8-125">**exposureDenominator**</span><span class="sxs-lookup"><span data-stu-id="e88b8-125">**exposureDenominator**</span></span> | <span data-ttu-id="e88b8-126">Double</span><span class="sxs-lookup"><span data-stu-id="e88b8-126">Double</span></span>         | <span data-ttu-id="e88b8-p105">Знаменатель дробного значения выдержки камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e88b8-p105">The denominator for the exposure time fraction from the camera. Read-only.</span></span>
| <span data-ttu-id="e88b8-129">**exposureNumerator**</span><span class="sxs-lookup"><span data-stu-id="e88b8-129">**exposureNumerator**</span></span>   | <span data-ttu-id="e88b8-130">Double</span><span class="sxs-lookup"><span data-stu-id="e88b8-130">Double</span></span>         | <span data-ttu-id="e88b8-p106">Числитель дробного значения выдержки камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e88b8-p106">The numerator for the exposure time fraction from the camera. Read-only.</span></span>
| <span data-ttu-id="e88b8-133">**focalLength**</span><span class="sxs-lookup"><span data-stu-id="e88b8-133">**focalLength**</span></span>         | <span data-ttu-id="e88b8-134">Double</span><span class="sxs-lookup"><span data-stu-id="e88b8-134">Double</span></span>         | <span data-ttu-id="e88b8-p107">Фокусное расстояние камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e88b8-p107">The focal length from the camera. Read-only.</span></span>
| <span data-ttu-id="e88b8-137">**iso**</span><span class="sxs-lookup"><span data-stu-id="e88b8-137">**iso**</span></span>                 | <span data-ttu-id="e88b8-138">Int32</span><span class="sxs-lookup"><span data-stu-id="e88b8-138">Int32</span></span>          | <span data-ttu-id="e88b8-p108">Значение ISO камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e88b8-p108">The ISO value from the camera. Read-only.</span></span>

## <a name="remarks"></a><span data-ttu-id="e88b8-141">Заметки</span><span class="sxs-lookup"><span data-stu-id="e88b8-141">Remarks</span></span>

<span data-ttu-id="e88b8-142">OneDrive для бизнеса и SharePoint возвращают только свойство **takenDateTime**.</span><span class="sxs-lookup"><span data-stu-id="e88b8-142">OneDrive for Business and SharePoint only return the **takenDateTime** property.</span></span>

<span data-ttu-id="e88b8-143">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="e88b8-143">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>
<!-- {
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso",
  "section": "documentation",
  "tocPath": "Facets/Photo"
} -->
