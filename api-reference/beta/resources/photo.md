---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Фотография
localization_priority: Normal
ms.openlocfilehash: d14777b0f39983d6ccf83ae387896c6587635e66
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32573762"
---
# <a name="photo-resource-type"></a><span data-ttu-id="8dd8c-102">Тип ресурса Photo</span><span class="sxs-lookup"><span data-stu-id="8dd8c-102">Photo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8dd8c-103">Ресурс **photo** предоставляет свойства фотографии и камеры, например метаданные EXIF, в ресурсе [driveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="8dd8c-103">The **photo** resource provides photo and camera properties, for example, EXIF metadata, on a [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="8dd8c-104">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8dd8c-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="8dd8c-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="8dd8c-105">Properties</span></span>

| <span data-ttu-id="8dd8c-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="8dd8c-106">Property</span></span>                | <span data-ttu-id="8dd8c-107">Тип</span><span class="sxs-lookup"><span data-stu-id="8dd8c-107">Type</span></span>           | <span data-ttu-id="8dd8c-108">Описание</span><span class="sxs-lookup"><span data-stu-id="8dd8c-108">Description</span></span>
|:------------------------|:---------------|:----------------------------------
| <span data-ttu-id="8dd8c-109">**takenDateTime**</span><span class="sxs-lookup"><span data-stu-id="8dd8c-109">**takenDateTime**</span></span>       | <span data-ttu-id="8dd8c-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8dd8c-110">DateTimeOffset</span></span> | <span data-ttu-id="8dd8c-p101">Представляет дату и время съемки. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8dd8c-p101">Represents the date and time the photo was taken. Read-only.</span></span>
| <span data-ttu-id="8dd8c-113">**cameraMake**</span><span class="sxs-lookup"><span data-stu-id="8dd8c-113">**cameraMake**</span></span>          | <span data-ttu-id="8dd8c-114">Строка</span><span class="sxs-lookup"><span data-stu-id="8dd8c-114">String</span></span>         | <span data-ttu-id="8dd8c-p102">Изготовитель камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8dd8c-p102">Camera manufacturer. Read-only.</span></span>
| <span data-ttu-id="8dd8c-117">**cameraModel**</span><span class="sxs-lookup"><span data-stu-id="8dd8c-117">**cameraModel**</span></span>         | <span data-ttu-id="8dd8c-118">String</span><span class="sxs-lookup"><span data-stu-id="8dd8c-118">String</span></span>         | <span data-ttu-id="8dd8c-p103">Модель камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8dd8c-p103">Camera model. Read-only.</span></span>
| <span data-ttu-id="8dd8c-121">**fNumber**</span><span class="sxs-lookup"><span data-stu-id="8dd8c-121">**fNumber**</span></span>             | <span data-ttu-id="8dd8c-122">Двойное</span><span class="sxs-lookup"><span data-stu-id="8dd8c-122">Double</span></span>         | <span data-ttu-id="8dd8c-p104">Значение диафрагмы камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8dd8c-p104">The F-stop value from the camera. Read-only.</span></span>
| <span data-ttu-id="8dd8c-125">**exposureDenominator**</span><span class="sxs-lookup"><span data-stu-id="8dd8c-125">**exposureDenominator**</span></span> | <span data-ttu-id="8dd8c-126">Двойное</span><span class="sxs-lookup"><span data-stu-id="8dd8c-126">Double</span></span>         | <span data-ttu-id="8dd8c-p105">Знаменатель дробного значения выдержки камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8dd8c-p105">The denominator for the exposure time fraction from the camera. Read-only.</span></span>
| <span data-ttu-id="8dd8c-129">**exposureNumerator**</span><span class="sxs-lookup"><span data-stu-id="8dd8c-129">**exposureNumerator**</span></span>   | <span data-ttu-id="8dd8c-130">Двойное</span><span class="sxs-lookup"><span data-stu-id="8dd8c-130">Double</span></span>         | <span data-ttu-id="8dd8c-p106">Числитель дробного значения выдержки камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8dd8c-p106">The numerator for the exposure time fraction from the camera. Read-only.</span></span>
| <span data-ttu-id="8dd8c-133">**focalLength**</span><span class="sxs-lookup"><span data-stu-id="8dd8c-133">**focalLength**</span></span>         | <span data-ttu-id="8dd8c-134">Double</span><span class="sxs-lookup"><span data-stu-id="8dd8c-134">Double</span></span>         | <span data-ttu-id="8dd8c-p107">Фокусное расстояние камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8dd8c-p107">The focal length from the camera. Read-only.</span></span>
| <span data-ttu-id="8dd8c-137">**iso**</span><span class="sxs-lookup"><span data-stu-id="8dd8c-137">**iso**</span></span>                 | <span data-ttu-id="8dd8c-138">Int64</span><span class="sxs-lookup"><span data-stu-id="8dd8c-138">Int64</span></span>          | <span data-ttu-id="8dd8c-p108">Значение ISO камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8dd8c-p108">The ISO value from the camera. Read-only.</span></span>

## <a name="remarks"></a><span data-ttu-id="8dd8c-141">Заметки</span><span class="sxs-lookup"><span data-stu-id="8dd8c-141">Remarks</span></span>
<span data-ttu-id="8dd8c-142">OneDrive для бизнеса и SharePoint возвращают только свойство **takenDateTime**.</span><span class="sxs-lookup"><span data-stu-id="8dd8c-142">OneDrive for Business and SharePoint only return the **takenDateTime** property.</span></span>

<span data-ttu-id="8dd8c-143">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="8dd8c-143">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>
<!--
{
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso",
  "section": "documentation",
  "tocPath": "Facets/Photo",
  "suppressions": [
    "Error: /api-reference/beta/resources/photo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
