---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Photo
localization_priority: Normal
ms.openlocfilehash: ed891f917ba8018aac349976df0455adfd269fdb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869386"
---
# <a name="photo-resource-type"></a><span data-ttu-id="8b7ed-102">Тип ресурса Photo</span><span class="sxs-lookup"><span data-stu-id="8b7ed-102">Photo resource type</span></span>

> <span data-ttu-id="8b7ed-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8b7ed-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8b7ed-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b7ed-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8b7ed-105">Ресурс **photo** предоставляет свойства фотографии и камеры, например метаданные EXIF, в ресурсе [driveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="8b7ed-105">The **photo** resource provides photo and camera properties, for example, EXIF metadata, on a [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="8b7ed-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8b7ed-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="8b7ed-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="8b7ed-107">Properties</span></span>

| <span data-ttu-id="8b7ed-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="8b7ed-108">Property</span></span>                | <span data-ttu-id="8b7ed-109">Тип</span><span class="sxs-lookup"><span data-stu-id="8b7ed-109">Type</span></span>           | <span data-ttu-id="8b7ed-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8b7ed-110">Description</span></span>
|:------------------------|:---------------|:----------------------------------
| <span data-ttu-id="8b7ed-111">**takenDateTime**</span><span class="sxs-lookup"><span data-stu-id="8b7ed-111">**takenDateTime**</span></span>       | <span data-ttu-id="8b7ed-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8b7ed-112">DateTimeOffset</span></span> | <span data-ttu-id="8b7ed-p102">Представляет дату и время съемки. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8b7ed-p102">Represents the date and time the photo was taken. Read-only.</span></span>
| <span data-ttu-id="8b7ed-115">**cameraMake**</span><span class="sxs-lookup"><span data-stu-id="8b7ed-115">**cameraMake**</span></span>          | <span data-ttu-id="8b7ed-116">Строка</span><span class="sxs-lookup"><span data-stu-id="8b7ed-116">String</span></span>         | <span data-ttu-id="8b7ed-p103">Изготовитель камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8b7ed-p103">Camera manufacturer. Read-only.</span></span>
| <span data-ttu-id="8b7ed-119">**cameraModel**</span><span class="sxs-lookup"><span data-stu-id="8b7ed-119">**cameraModel**</span></span>         | <span data-ttu-id="8b7ed-120">String</span><span class="sxs-lookup"><span data-stu-id="8b7ed-120">String</span></span>         | <span data-ttu-id="8b7ed-p104">Модель камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8b7ed-p104">Camera model. Read-only.</span></span>
| <span data-ttu-id="8b7ed-123">**fNumber**</span><span class="sxs-lookup"><span data-stu-id="8b7ed-123">**fNumber**</span></span>             | <span data-ttu-id="8b7ed-124">Double</span><span class="sxs-lookup"><span data-stu-id="8b7ed-124">Double</span></span>         | <span data-ttu-id="8b7ed-p105">Значение диафрагмы камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8b7ed-p105">The F-stop value from the camera. Read-only.</span></span>
| <span data-ttu-id="8b7ed-127">**exposureDenominator**</span><span class="sxs-lookup"><span data-stu-id="8b7ed-127">**exposureDenominator**</span></span> | <span data-ttu-id="8b7ed-128">Double</span><span class="sxs-lookup"><span data-stu-id="8b7ed-128">Double</span></span>         | <span data-ttu-id="8b7ed-p106">Знаменатель дробного значения выдержки камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8b7ed-p106">The denominator for the exposure time fraction from the camera. Read-only.</span></span>
| <span data-ttu-id="8b7ed-131">**exposureNumerator**</span><span class="sxs-lookup"><span data-stu-id="8b7ed-131">**exposureNumerator**</span></span>   | <span data-ttu-id="8b7ed-132">Double</span><span class="sxs-lookup"><span data-stu-id="8b7ed-132">Double</span></span>         | <span data-ttu-id="8b7ed-p107">Числитель дробного значения выдержки камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8b7ed-p107">The numerator for the exposure time fraction from the camera. Read-only.</span></span>
| <span data-ttu-id="8b7ed-135">**focalLength**</span><span class="sxs-lookup"><span data-stu-id="8b7ed-135">**focalLength**</span></span>         | <span data-ttu-id="8b7ed-136">Double</span><span class="sxs-lookup"><span data-stu-id="8b7ed-136">Double</span></span>         | <span data-ttu-id="8b7ed-p108">Фокусное расстояние камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8b7ed-p108">The focal length from the camera. Read-only.</span></span>
| <span data-ttu-id="8b7ed-139">**iso**</span><span class="sxs-lookup"><span data-stu-id="8b7ed-139">**iso**</span></span>                 | <span data-ttu-id="8b7ed-140">Int64</span><span class="sxs-lookup"><span data-stu-id="8b7ed-140">Int64</span></span>          | <span data-ttu-id="8b7ed-p109">Значение ISO камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8b7ed-p109">The ISO value from the camera. Read-only.</span></span>

## <a name="remarks"></a><span data-ttu-id="8b7ed-143">Заметки</span><span class="sxs-lookup"><span data-stu-id="8b7ed-143">Remarks</span></span>
<span data-ttu-id="8b7ed-144">OneDrive для бизнеса и SharePoint возвращают только свойство **takenDateTime**.</span><span class="sxs-lookup"><span data-stu-id="8b7ed-144">OneDrive for Business and SharePoint only return the **takenDateTime** property.</span></span>

<span data-ttu-id="8b7ed-145">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="8b7ed-145">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>
<!-- {
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso",
  "section": "documentation",
  "tocPath": "Facets/Photo"
} -->
