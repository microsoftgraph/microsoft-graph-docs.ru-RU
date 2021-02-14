---
author: JeremyKelley
ms.date: 09/10/2017
title: Photo
localization_priority: Normal
description: Ресурс photo предоставляет свойства фотографии и камеры, например метаданные EXIF, в ресурсе driveItem.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: fce0ba456e07c798cfcfce534b6428720afa619e
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239529"
---
# <a name="photo-resource-type"></a><span data-ttu-id="8a35b-103">Тип ресурса Photo</span><span class="sxs-lookup"><span data-stu-id="8a35b-103">Photo resource type</span></span>

<span data-ttu-id="8a35b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a35b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8a35b-105">Ресурс **photo** предоставляет свойства фотографии и камеры, например метаданные EXIF, в ресурсе [driveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="8a35b-105">The **photo** resource provides photo and camera properties, for example, EXIF metadata, on a [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="8a35b-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8a35b-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="8a35b-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="8a35b-107">Properties</span></span>

| <span data-ttu-id="8a35b-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="8a35b-108">Property</span></span>                | <span data-ttu-id="8a35b-109">Тип</span><span class="sxs-lookup"><span data-stu-id="8a35b-109">Type</span></span>           | <span data-ttu-id="8a35b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8a35b-110">Description</span></span>
|:------------------------|:---------------|:----------------------------------
| <span data-ttu-id="8a35b-111">**takenDateTime**</span><span class="sxs-lookup"><span data-stu-id="8a35b-111">**takenDateTime**</span></span>       | <span data-ttu-id="8a35b-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8a35b-112">DateTimeOffset</span></span> | <span data-ttu-id="8a35b-p101">Представляет дату и время съемки. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8a35b-p101">Represents the date and time the photo was taken. Read-only.</span></span>
| <span data-ttu-id="8a35b-115">**cameraMake**</span><span class="sxs-lookup"><span data-stu-id="8a35b-115">**cameraMake**</span></span>          | <span data-ttu-id="8a35b-116">Строка</span><span class="sxs-lookup"><span data-stu-id="8a35b-116">String</span></span>         | <span data-ttu-id="8a35b-p102">Изготовитель камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8a35b-p102">Camera manufacturer. Read-only.</span></span>
| <span data-ttu-id="8a35b-119">**cameraModel**</span><span class="sxs-lookup"><span data-stu-id="8a35b-119">**cameraModel**</span></span>         | <span data-ttu-id="8a35b-120">String</span><span class="sxs-lookup"><span data-stu-id="8a35b-120">String</span></span>         | <span data-ttu-id="8a35b-p103">Модель камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8a35b-p103">Camera model. Read-only.</span></span>
| <span data-ttu-id="8a35b-123">**fNumber**</span><span class="sxs-lookup"><span data-stu-id="8a35b-123">**fNumber**</span></span>             | <span data-ttu-id="8a35b-124">Double</span><span class="sxs-lookup"><span data-stu-id="8a35b-124">Double</span></span>         | <span data-ttu-id="8a35b-p104">Значение диафрагмы камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8a35b-p104">The F-stop value from the camera. Read-only.</span></span>
| <span data-ttu-id="8a35b-127">**exposureDenominator**</span><span class="sxs-lookup"><span data-stu-id="8a35b-127">**exposureDenominator**</span></span> | <span data-ttu-id="8a35b-128">Double</span><span class="sxs-lookup"><span data-stu-id="8a35b-128">Double</span></span>         | <span data-ttu-id="8a35b-p105">Знаменатель дробного значения выдержки камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8a35b-p105">The denominator for the exposure time fraction from the camera. Read-only.</span></span>
| <span data-ttu-id="8a35b-131">**exposureNumerator**</span><span class="sxs-lookup"><span data-stu-id="8a35b-131">**exposureNumerator**</span></span>   | <span data-ttu-id="8a35b-132">Double</span><span class="sxs-lookup"><span data-stu-id="8a35b-132">Double</span></span>         | <span data-ttu-id="8a35b-p106">Числитель дробного значения выдержки камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8a35b-p106">The numerator for the exposure time fraction from the camera. Read-only.</span></span>
| <span data-ttu-id="8a35b-135">**focalLength**</span><span class="sxs-lookup"><span data-stu-id="8a35b-135">**focalLength**</span></span>         | <span data-ttu-id="8a35b-136">Double</span><span class="sxs-lookup"><span data-stu-id="8a35b-136">Double</span></span>         | <span data-ttu-id="8a35b-p107">Фокусное расстояние камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8a35b-p107">The focal length from the camera. Read-only.</span></span>
| <span data-ttu-id="8a35b-139">**iso**</span><span class="sxs-lookup"><span data-stu-id="8a35b-139">**iso**</span></span>                 | <span data-ttu-id="8a35b-140">Int32</span><span class="sxs-lookup"><span data-stu-id="8a35b-140">Int32</span></span>          | <span data-ttu-id="8a35b-p108">Значение ISO камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8a35b-p108">The ISO value from the camera. Read-only.</span></span>
| <span data-ttu-id="8a35b-143">**orientation**</span><span class="sxs-lookup"><span data-stu-id="8a35b-143">**orientation**</span></span>         | <span data-ttu-id="8a35b-144">Int16</span><span class="sxs-lookup"><span data-stu-id="8a35b-144">Int16</span></span>          | <span data-ttu-id="8a35b-145">Значение ориентации камеры.</span><span class="sxs-lookup"><span data-stu-id="8a35b-145">The orientation value from the camera.</span></span> <span data-ttu-id="8a35b-146">Можно перезаписать в OneDrive персональный.</span><span class="sxs-lookup"><span data-stu-id="8a35b-146">Writable on OneDrive Personal.</span></span>      |

## <a name="remarks"></a><span data-ttu-id="8a35b-147">Заметки</span><span class="sxs-lookup"><span data-stu-id="8a35b-147">Remarks</span></span>

<span data-ttu-id="8a35b-148">OneDrive для бизнеса и SharePoint возвращают только свойство **takenDateTime**.</span><span class="sxs-lookup"><span data-stu-id="8a35b-148">OneDrive for Business and SharePoint only return the **takenDateTime** property.</span></span>

<span data-ttu-id="8a35b-149">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="8a35b-149">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>
<!-- {
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso, orientation",
  "section": "documentation",
  "tocPath": "Facets/Photo"
} -->

