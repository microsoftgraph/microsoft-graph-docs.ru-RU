---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Фотография
localization_priority: Normal
description: Ресурс photo предоставляет свойства фотографии и камеры, например метаданные EXIF, в ресурсе driveItem.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 4e3f167384112c3c3354cdff88b41632f92e2637
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42534052"
---
# <a name="photo-resource-type"></a><span data-ttu-id="2824d-103">Тип ресурса Photo</span><span class="sxs-lookup"><span data-stu-id="2824d-103">Photo resource type</span></span>

<span data-ttu-id="2824d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2824d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2824d-105">Ресурс **photo** предоставляет свойства фотографии и камеры, например метаданные EXIF, в ресурсе [driveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="2824d-105">The **photo** resource provides photo and camera properties, for example, EXIF metadata, on a [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="2824d-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2824d-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="2824d-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="2824d-107">Properties</span></span>

| <span data-ttu-id="2824d-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="2824d-108">Property</span></span>                | <span data-ttu-id="2824d-109">Тип</span><span class="sxs-lookup"><span data-stu-id="2824d-109">Type</span></span>           | <span data-ttu-id="2824d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2824d-110">Description</span></span>
|:------------------------|:---------------|:----------------------------------
| <span data-ttu-id="2824d-111">**takenDateTime**</span><span class="sxs-lookup"><span data-stu-id="2824d-111">**takenDateTime**</span></span>       | <span data-ttu-id="2824d-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2824d-112">DateTimeOffset</span></span> | <span data-ttu-id="2824d-p101">Представляет дату и время съемки. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2824d-p101">Represents the date and time the photo was taken. Read-only.</span></span>
| <span data-ttu-id="2824d-115">**cameraMake**</span><span class="sxs-lookup"><span data-stu-id="2824d-115">**cameraMake**</span></span>          | <span data-ttu-id="2824d-116">Строка</span><span class="sxs-lookup"><span data-stu-id="2824d-116">String</span></span>         | <span data-ttu-id="2824d-p102">Изготовитель камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2824d-p102">Camera manufacturer. Read-only.</span></span>
| <span data-ttu-id="2824d-119">**cameraModel**</span><span class="sxs-lookup"><span data-stu-id="2824d-119">**cameraModel**</span></span>         | <span data-ttu-id="2824d-120">String</span><span class="sxs-lookup"><span data-stu-id="2824d-120">String</span></span>         | <span data-ttu-id="2824d-p103">Модель камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2824d-p103">Camera model. Read-only.</span></span>
| <span data-ttu-id="2824d-123">**fNumber**</span><span class="sxs-lookup"><span data-stu-id="2824d-123">**fNumber**</span></span>             | <span data-ttu-id="2824d-124">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="2824d-124">Double</span></span>         | <span data-ttu-id="2824d-p104">Значение диафрагмы камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2824d-p104">The F-stop value from the camera. Read-only.</span></span>
| <span data-ttu-id="2824d-127">**exposureDenominator**</span><span class="sxs-lookup"><span data-stu-id="2824d-127">**exposureDenominator**</span></span> | <span data-ttu-id="2824d-128">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="2824d-128">Double</span></span>         | <span data-ttu-id="2824d-p105">Знаменатель дробного значения выдержки камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2824d-p105">The denominator for the exposure time fraction from the camera. Read-only.</span></span>
| <span data-ttu-id="2824d-131">**exposureNumerator**</span><span class="sxs-lookup"><span data-stu-id="2824d-131">**exposureNumerator**</span></span>   | <span data-ttu-id="2824d-132">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="2824d-132">Double</span></span>         | <span data-ttu-id="2824d-p106">Числитель дробного значения выдержки камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2824d-p106">The numerator for the exposure time fraction from the camera. Read-only.</span></span>
| <span data-ttu-id="2824d-135">**focalLength**</span><span class="sxs-lookup"><span data-stu-id="2824d-135">**focalLength**</span></span>         | <span data-ttu-id="2824d-136">Double</span><span class="sxs-lookup"><span data-stu-id="2824d-136">Double</span></span>         | <span data-ttu-id="2824d-p107">Фокусное расстояние камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2824d-p107">The focal length from the camera. Read-only.</span></span>
| <span data-ttu-id="2824d-139">**iso**</span><span class="sxs-lookup"><span data-stu-id="2824d-139">**iso**</span></span>                 | <span data-ttu-id="2824d-140">Int32</span><span class="sxs-lookup"><span data-stu-id="2824d-140">Int32</span></span>          | <span data-ttu-id="2824d-p108">Значение ISO камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2824d-p108">The ISO value from the camera. Read-only.</span></span>

## <a name="remarks"></a><span data-ttu-id="2824d-143">Заметки</span><span class="sxs-lookup"><span data-stu-id="2824d-143">Remarks</span></span>

<span data-ttu-id="2824d-144">OneDrive для бизнеса и SharePoint возвращают только свойство **takenDateTime**.</span><span class="sxs-lookup"><span data-stu-id="2824d-144">OneDrive for Business and SharePoint only return the **takenDateTime** property.</span></span>

<span data-ttu-id="2824d-145">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="2824d-145">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>
<!-- {
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso",
  "section": "documentation",
  "tocPath": "Facets/Photo"
} -->
