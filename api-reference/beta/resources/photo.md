---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Photo
ms.openlocfilehash: f61d37eecccd4bf08a2f8abbf4cda15dee5eb94d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078693"
---
# <a name="photo-resource-type"></a><span data-ttu-id="473da-102">Тип ресурса Photo</span><span class="sxs-lookup"><span data-stu-id="473da-102">Photo resource type</span></span>

> <span data-ttu-id="473da-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="473da-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="473da-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="473da-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="473da-105">Ресурс **photo** предоставляет свойства фотографии и камеры, например метаданные EXIF, в ресурсе [driveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="473da-105">The **photo** resource provides photo and camera properties, for example, EXIF metadata, on a [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="473da-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="473da-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="473da-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="473da-107">Properties</span></span>

| <span data-ttu-id="473da-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="473da-108">Property</span></span>                | <span data-ttu-id="473da-109">Тип</span><span class="sxs-lookup"><span data-stu-id="473da-109">Type</span></span>           | <span data-ttu-id="473da-110">Описание</span><span class="sxs-lookup"><span data-stu-id="473da-110">Description</span></span>
|:------------------------|:---------------|:----------------------------------
| <span data-ttu-id="473da-111">**takenDateTime**</span><span class="sxs-lookup"><span data-stu-id="473da-111">**takenDateTime**</span></span>       | <span data-ttu-id="473da-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="473da-112">DateTimeOffset</span></span> | <span data-ttu-id="473da-p102">Представляет дату и время съемки. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="473da-p102">Represents the date and time the photo was taken. Read-only.</span></span>
| <span data-ttu-id="473da-115">**cameraMake**</span><span class="sxs-lookup"><span data-stu-id="473da-115">**cameraMake**</span></span>          | <span data-ttu-id="473da-116">String</span><span class="sxs-lookup"><span data-stu-id="473da-116">String</span></span>         | <span data-ttu-id="473da-p103">Изготовитель камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="473da-p103">Camera manufacturer. Read-only.</span></span>
| <span data-ttu-id="473da-119">**cameraModel**</span><span class="sxs-lookup"><span data-stu-id="473da-119">**cameraModel**</span></span>         | <span data-ttu-id="473da-120">String</span><span class="sxs-lookup"><span data-stu-id="473da-120">String</span></span>         | <span data-ttu-id="473da-p104">Модель камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="473da-p104">Camera model. Read-only.</span></span>
| <span data-ttu-id="473da-123">**fNumber**</span><span class="sxs-lookup"><span data-stu-id="473da-123">**fNumber**</span></span>             | <span data-ttu-id="473da-124">Double</span><span class="sxs-lookup"><span data-stu-id="473da-124">Double</span></span>         | <span data-ttu-id="473da-p105">Значение диафрагмы камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="473da-p105">The F-stop value from the camera. Read-only.</span></span>
| <span data-ttu-id="473da-127">**exposureDenominator**</span><span class="sxs-lookup"><span data-stu-id="473da-127">**exposureDenominator**</span></span> | <span data-ttu-id="473da-128">Double</span><span class="sxs-lookup"><span data-stu-id="473da-128">Double</span></span>         | <span data-ttu-id="473da-p106">Знаменатель дробного значения выдержки камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="473da-p106">The denominator for the exposure time fraction from the camera. Read-only.</span></span>
| <span data-ttu-id="473da-131">**exposureNumerator**</span><span class="sxs-lookup"><span data-stu-id="473da-131">**exposureNumerator**</span></span>   | <span data-ttu-id="473da-132">Double</span><span class="sxs-lookup"><span data-stu-id="473da-132">Double</span></span>         | <span data-ttu-id="473da-p107">Числитель дробного значения выдержки камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="473da-p107">The numerator for the exposure time fraction from the camera. Read-only.</span></span>
| <span data-ttu-id="473da-135">**focalLength**</span><span class="sxs-lookup"><span data-stu-id="473da-135">**focalLength**</span></span>         | <span data-ttu-id="473da-136">Double</span><span class="sxs-lookup"><span data-stu-id="473da-136">Double</span></span>         | <span data-ttu-id="473da-p108">Фокусное расстояние камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="473da-p108">The focal length from the camera. Read-only.</span></span>
| <span data-ttu-id="473da-139">**iso**</span><span class="sxs-lookup"><span data-stu-id="473da-139">**iso**</span></span>                 | <span data-ttu-id="473da-140">Int64</span><span class="sxs-lookup"><span data-stu-id="473da-140">Int64</span></span>          | <span data-ttu-id="473da-p109">Значение ISO камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="473da-p109">The ISO value from the camera. Read-only.</span></span>

## <a name="remarks"></a><span data-ttu-id="473da-143">Заметки</span><span class="sxs-lookup"><span data-stu-id="473da-143">Remarks</span></span>
<span data-ttu-id="473da-144">OneDrive для бизнеса и SharePoint возвращают только свойство **takenDateTime**.</span><span class="sxs-lookup"><span data-stu-id="473da-144">OneDrive for Business and SharePoint only return the **takenDateTime** property.</span></span>

<span data-ttu-id="473da-145">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="473da-145">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>
<!-- {
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso",
  "section": "documentation",
  "tocPath": "Facets/Photo"
} -->
