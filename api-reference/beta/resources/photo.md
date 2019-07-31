---
author: JeremyKelley
description: Ресурс photo предоставляет свойства фотографии и камеры, например метаданные EXIF, в ресурсе driveItem.
ms.date: 09/10/2017
title: Фотография
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 6713e66b5ca14cfa6605b9e67d4bec152a321f33
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009225"
---
# <a name="photo-resource-type"></a><span data-ttu-id="cb2aa-103">Тип ресурса Photo</span><span class="sxs-lookup"><span data-stu-id="cb2aa-103">Photo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cb2aa-104">Ресурс **photo** предоставляет свойства фотографии и камеры, например метаданные EXIF, в ресурсе [driveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="cb2aa-104">The **photo** resource provides photo and camera properties, for example, EXIF metadata, on a [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="cb2aa-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cb2aa-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="cb2aa-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="cb2aa-106">Properties</span></span>

| <span data-ttu-id="cb2aa-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="cb2aa-107">Property</span></span>                | <span data-ttu-id="cb2aa-108">Тип</span><span class="sxs-lookup"><span data-stu-id="cb2aa-108">Type</span></span>           | <span data-ttu-id="cb2aa-109">Описание</span><span class="sxs-lookup"><span data-stu-id="cb2aa-109">Description</span></span>
|:------------------------|:---------------|:----------------------------------
| <span data-ttu-id="cb2aa-110">**takenDateTime**</span><span class="sxs-lookup"><span data-stu-id="cb2aa-110">**takenDateTime**</span></span>       | <span data-ttu-id="cb2aa-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb2aa-111">DateTimeOffset</span></span> | <span data-ttu-id="cb2aa-p101">Представляет дату и время съемки. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cb2aa-p101">Represents the date and time the photo was taken. Read-only.</span></span>
| <span data-ttu-id="cb2aa-114">**cameraMake**</span><span class="sxs-lookup"><span data-stu-id="cb2aa-114">**cameraMake**</span></span>          | <span data-ttu-id="cb2aa-115">Строка</span><span class="sxs-lookup"><span data-stu-id="cb2aa-115">String</span></span>         | <span data-ttu-id="cb2aa-p102">Изготовитель камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cb2aa-p102">Camera manufacturer. Read-only.</span></span>
| <span data-ttu-id="cb2aa-118">**cameraModel**</span><span class="sxs-lookup"><span data-stu-id="cb2aa-118">**cameraModel**</span></span>         | <span data-ttu-id="cb2aa-119">String</span><span class="sxs-lookup"><span data-stu-id="cb2aa-119">String</span></span>         | <span data-ttu-id="cb2aa-p103">Модель камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cb2aa-p103">Camera model. Read-only.</span></span>
| <span data-ttu-id="cb2aa-122">**fNumber**</span><span class="sxs-lookup"><span data-stu-id="cb2aa-122">**fNumber**</span></span>             | <span data-ttu-id="cb2aa-123">Двойное</span><span class="sxs-lookup"><span data-stu-id="cb2aa-123">Double</span></span>         | <span data-ttu-id="cb2aa-p104">Значение диафрагмы камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cb2aa-p104">The F-stop value from the camera. Read-only.</span></span>
| <span data-ttu-id="cb2aa-126">**exposureDenominator**</span><span class="sxs-lookup"><span data-stu-id="cb2aa-126">**exposureDenominator**</span></span> | <span data-ttu-id="cb2aa-127">Двойное</span><span class="sxs-lookup"><span data-stu-id="cb2aa-127">Double</span></span>         | <span data-ttu-id="cb2aa-p105">Знаменатель дробного значения выдержки камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cb2aa-p105">The denominator for the exposure time fraction from the camera. Read-only.</span></span>
| <span data-ttu-id="cb2aa-130">**exposureNumerator**</span><span class="sxs-lookup"><span data-stu-id="cb2aa-130">**exposureNumerator**</span></span>   | <span data-ttu-id="cb2aa-131">Двойное</span><span class="sxs-lookup"><span data-stu-id="cb2aa-131">Double</span></span>         | <span data-ttu-id="cb2aa-p106">Числитель дробного значения выдержки камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cb2aa-p106">The numerator for the exposure time fraction from the camera. Read-only.</span></span>
| <span data-ttu-id="cb2aa-134">**focalLength**</span><span class="sxs-lookup"><span data-stu-id="cb2aa-134">**focalLength**</span></span>         | <span data-ttu-id="cb2aa-135">Double</span><span class="sxs-lookup"><span data-stu-id="cb2aa-135">Double</span></span>         | <span data-ttu-id="cb2aa-p107">Фокусное расстояние камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cb2aa-p107">The focal length from the camera. Read-only.</span></span>
| <span data-ttu-id="cb2aa-138">**iso**</span><span class="sxs-lookup"><span data-stu-id="cb2aa-138">**iso**</span></span>                 | <span data-ttu-id="cb2aa-139">Int64</span><span class="sxs-lookup"><span data-stu-id="cb2aa-139">Int64</span></span>          | <span data-ttu-id="cb2aa-p108">Значение ISO камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cb2aa-p108">The ISO value from the camera. Read-only.</span></span>

## <a name="remarks"></a><span data-ttu-id="cb2aa-142">Заметки</span><span class="sxs-lookup"><span data-stu-id="cb2aa-142">Remarks</span></span>
<span data-ttu-id="cb2aa-143">OneDrive для бизнеса и SharePoint возвращают только свойство **takenDateTime**.</span><span class="sxs-lookup"><span data-stu-id="cb2aa-143">OneDrive for Business and SharePoint only return the **takenDateTime** property.</span></span>

<span data-ttu-id="cb2aa-144">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="cb2aa-144">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>
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
