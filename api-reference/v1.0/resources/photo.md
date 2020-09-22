---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Photo
localization_priority: Normal
description: Ресурс photo предоставляет свойства фотографии и камеры, например метаданные EXIF, в ресурсе driveItem.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 362d4f76f56fa5824985a3580d6008d8c5081a7c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48072853"
---
# <a name="photo-resource-type"></a><span data-ttu-id="3c139-103">Тип ресурса Photo</span><span class="sxs-lookup"><span data-stu-id="3c139-103">Photo resource type</span></span>

<span data-ttu-id="3c139-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c139-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3c139-105">Ресурс **photo** предоставляет свойства фотографии и камеры, например метаданные EXIF, в ресурсе [driveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="3c139-105">The **photo** resource provides photo and camera properties, for example, EXIF metadata, on a [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="3c139-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3c139-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="3c139-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="3c139-107">Properties</span></span>

| <span data-ttu-id="3c139-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="3c139-108">Property</span></span>                | <span data-ttu-id="3c139-109">Тип</span><span class="sxs-lookup"><span data-stu-id="3c139-109">Type</span></span>           | <span data-ttu-id="3c139-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3c139-110">Description</span></span>
|:------------------------|:---------------|:----------------------------------
| <span data-ttu-id="3c139-111">**takenDateTime**</span><span class="sxs-lookup"><span data-stu-id="3c139-111">**takenDateTime**</span></span>       | <span data-ttu-id="3c139-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c139-112">DateTimeOffset</span></span> | <span data-ttu-id="3c139-p101">Представляет дату и время съемки. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3c139-p101">Represents the date and time the photo was taken. Read-only.</span></span>
| <span data-ttu-id="3c139-115">**cameraMake**</span><span class="sxs-lookup"><span data-stu-id="3c139-115">**cameraMake**</span></span>          | <span data-ttu-id="3c139-116">Строка</span><span class="sxs-lookup"><span data-stu-id="3c139-116">String</span></span>         | <span data-ttu-id="3c139-p102">Изготовитель камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3c139-p102">Camera manufacturer. Read-only.</span></span>
| <span data-ttu-id="3c139-119">**cameraModel**</span><span class="sxs-lookup"><span data-stu-id="3c139-119">**cameraModel**</span></span>         | <span data-ttu-id="3c139-120">String</span><span class="sxs-lookup"><span data-stu-id="3c139-120">String</span></span>         | <span data-ttu-id="3c139-p103">Модель камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3c139-p103">Camera model. Read-only.</span></span>
| <span data-ttu-id="3c139-123">**fNumber**</span><span class="sxs-lookup"><span data-stu-id="3c139-123">**fNumber**</span></span>             | <span data-ttu-id="3c139-124">Double</span><span class="sxs-lookup"><span data-stu-id="3c139-124">Double</span></span>         | <span data-ttu-id="3c139-p104">Значение диафрагмы камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3c139-p104">The F-stop value from the camera. Read-only.</span></span>
| <span data-ttu-id="3c139-127">**exposureDenominator**</span><span class="sxs-lookup"><span data-stu-id="3c139-127">**exposureDenominator**</span></span> | <span data-ttu-id="3c139-128">Double</span><span class="sxs-lookup"><span data-stu-id="3c139-128">Double</span></span>         | <span data-ttu-id="3c139-p105">Знаменатель дробного значения выдержки камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3c139-p105">The denominator for the exposure time fraction from the camera. Read-only.</span></span>
| <span data-ttu-id="3c139-131">**exposureNumerator**</span><span class="sxs-lookup"><span data-stu-id="3c139-131">**exposureNumerator**</span></span>   | <span data-ttu-id="3c139-132">Double</span><span class="sxs-lookup"><span data-stu-id="3c139-132">Double</span></span>         | <span data-ttu-id="3c139-p106">Числитель дробного значения выдержки камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3c139-p106">The numerator for the exposure time fraction from the camera. Read-only.</span></span>
| <span data-ttu-id="3c139-135">**focalLength**</span><span class="sxs-lookup"><span data-stu-id="3c139-135">**focalLength**</span></span>         | <span data-ttu-id="3c139-136">Double</span><span class="sxs-lookup"><span data-stu-id="3c139-136">Double</span></span>         | <span data-ttu-id="3c139-p107">Фокусное расстояние камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3c139-p107">The focal length from the camera. Read-only.</span></span>
| <span data-ttu-id="3c139-139">**iso**</span><span class="sxs-lookup"><span data-stu-id="3c139-139">**iso**</span></span>                 | <span data-ttu-id="3c139-140">Int32</span><span class="sxs-lookup"><span data-stu-id="3c139-140">Int32</span></span>          | <span data-ttu-id="3c139-p108">Значение ISO камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3c139-p108">The ISO value from the camera. Read-only.</span></span>
| <span data-ttu-id="3c139-143">**orientation**</span><span class="sxs-lookup"><span data-stu-id="3c139-143">**orientation**</span></span>         | <span data-ttu-id="3c139-144">Int16</span><span class="sxs-lookup"><span data-stu-id="3c139-144">Int16</span></span>          | <span data-ttu-id="3c139-145">Значение ориентации камеры.</span><span class="sxs-lookup"><span data-stu-id="3c139-145">The orientation value from the camera.</span></span> <span data-ttu-id="3c139-146">Возможность записи в OneDrive персональный.</span><span class="sxs-lookup"><span data-stu-id="3c139-146">Writable on OneDrive Personal.</span></span>      |

## <a name="remarks"></a><span data-ttu-id="3c139-147">Заметки</span><span class="sxs-lookup"><span data-stu-id="3c139-147">Remarks</span></span>

<span data-ttu-id="3c139-148">OneDrive для бизнеса и SharePoint возвращают только свойство **takenDateTime**.</span><span class="sxs-lookup"><span data-stu-id="3c139-148">OneDrive for Business and SharePoint only return the **takenDateTime** property.</span></span>

<span data-ttu-id="3c139-149">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="3c139-149">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>
<!-- {
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso, orientation",
  "section": "documentation",
  "tocPath": "Facets/Photo"
} -->

