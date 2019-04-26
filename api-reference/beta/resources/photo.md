---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Фотография
localization_priority: Normal
ms.openlocfilehash: f55236489d71c88f8d000b3462e64e82b8c08e56
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344917"
---
# <a name="photo-resource-type"></a><span data-ttu-id="b4176-102">Тип ресурса Photo</span><span class="sxs-lookup"><span data-stu-id="b4176-102">Photo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b4176-103">Ресурс **photo** предоставляет свойства фотографии и камеры, например метаданные EXIF, в ресурсе [driveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="b4176-103">The **photo** resource provides photo and camera properties, for example, EXIF metadata, on a [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="b4176-104">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b4176-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="b4176-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="b4176-105">Properties</span></span>

| <span data-ttu-id="b4176-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="b4176-106">Property</span></span>                | <span data-ttu-id="b4176-107">Тип</span><span class="sxs-lookup"><span data-stu-id="b4176-107">Type</span></span>           | <span data-ttu-id="b4176-108">Описание</span><span class="sxs-lookup"><span data-stu-id="b4176-108">Description</span></span>
|:------------------------|:---------------|:----------------------------------
| <span data-ttu-id="b4176-109">**takenDateTime**</span><span class="sxs-lookup"><span data-stu-id="b4176-109">**takenDateTime**</span></span>       | <span data-ttu-id="b4176-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4176-110">DateTimeOffset</span></span> | <span data-ttu-id="b4176-p101">Представляет дату и время съемки. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b4176-p101">Represents the date and time the photo was taken. Read-only.</span></span>
| <span data-ttu-id="b4176-113">**cameraMake**</span><span class="sxs-lookup"><span data-stu-id="b4176-113">**cameraMake**</span></span>          | <span data-ttu-id="b4176-114">Строка</span><span class="sxs-lookup"><span data-stu-id="b4176-114">String</span></span>         | <span data-ttu-id="b4176-p102">Изготовитель камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b4176-p102">Camera manufacturer. Read-only.</span></span>
| <span data-ttu-id="b4176-117">**cameraModel**</span><span class="sxs-lookup"><span data-stu-id="b4176-117">**cameraModel**</span></span>         | <span data-ttu-id="b4176-118">String</span><span class="sxs-lookup"><span data-stu-id="b4176-118">String</span></span>         | <span data-ttu-id="b4176-p103">Модель камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b4176-p103">Camera model. Read-only.</span></span>
| <span data-ttu-id="b4176-121">**fNumber**</span><span class="sxs-lookup"><span data-stu-id="b4176-121">**fNumber**</span></span>             | <span data-ttu-id="b4176-122">Двойное</span><span class="sxs-lookup"><span data-stu-id="b4176-122">Double</span></span>         | <span data-ttu-id="b4176-p104">Значение диафрагмы камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b4176-p104">The F-stop value from the camera. Read-only.</span></span>
| <span data-ttu-id="b4176-125">**exposureDenominator**</span><span class="sxs-lookup"><span data-stu-id="b4176-125">**exposureDenominator**</span></span> | <span data-ttu-id="b4176-126">Двойное</span><span class="sxs-lookup"><span data-stu-id="b4176-126">Double</span></span>         | <span data-ttu-id="b4176-p105">Знаменатель дробного значения выдержки камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b4176-p105">The denominator for the exposure time fraction from the camera. Read-only.</span></span>
| <span data-ttu-id="b4176-129">**exposureNumerator**</span><span class="sxs-lookup"><span data-stu-id="b4176-129">**exposureNumerator**</span></span>   | <span data-ttu-id="b4176-130">Двойное</span><span class="sxs-lookup"><span data-stu-id="b4176-130">Double</span></span>         | <span data-ttu-id="b4176-p106">Числитель дробного значения выдержки камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b4176-p106">The numerator for the exposure time fraction from the camera. Read-only.</span></span>
| <span data-ttu-id="b4176-133">**focalLength**</span><span class="sxs-lookup"><span data-stu-id="b4176-133">**focalLength**</span></span>         | <span data-ttu-id="b4176-134">Double</span><span class="sxs-lookup"><span data-stu-id="b4176-134">Double</span></span>         | <span data-ttu-id="b4176-p107">Фокусное расстояние камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b4176-p107">The focal length from the camera. Read-only.</span></span>
| <span data-ttu-id="b4176-137">**iso**</span><span class="sxs-lookup"><span data-stu-id="b4176-137">**iso**</span></span>                 | <span data-ttu-id="b4176-138">Int64</span><span class="sxs-lookup"><span data-stu-id="b4176-138">Int64</span></span>          | <span data-ttu-id="b4176-p108">Значение ISO камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b4176-p108">The ISO value from the camera. Read-only.</span></span>

## <a name="remarks"></a><span data-ttu-id="b4176-141">Заметки</span><span class="sxs-lookup"><span data-stu-id="b4176-141">Remarks</span></span>
<span data-ttu-id="b4176-142">OneDrive для бизнеса и SharePoint возвращают только свойство **takenDateTime**.</span><span class="sxs-lookup"><span data-stu-id="b4176-142">OneDrive for Business and SharePoint only return the **takenDateTime** property.</span></span>

<span data-ttu-id="b4176-143">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="b4176-143">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>
<!--
{
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso",
  "section": "documentation",
  "tocPath": "Facets/Photo",
  "suppressions": []
}
-->
