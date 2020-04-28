---
title: Тип ресурса Photo
description: Ресурс photo предоставляет свойства фотографии и камеры, например метаданные EXIF, в ресурсе driveItem.
ms.date: 09/10/2017
localization_priority: Normal
author: JeremyKelley
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: bdb587e7440fd98c48f71a2611e2a34e039367dd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521885"
---
# <a name="photo-resource-type"></a><span data-ttu-id="f9937-103">Тип ресурса Photo</span><span class="sxs-lookup"><span data-stu-id="f9937-103">photo resource type</span></span>

<span data-ttu-id="f9937-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f9937-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f9937-105">Ресурс **photo** предоставляет свойства фотографии и камеры, например метаданные EXIF, в ресурсе [driveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="f9937-105">The **photo** resource provides photo and camera properties, for example, EXIF metadata, on a [driveItem](driveitem.md).</span></span>

> [!NOTE]
> <span data-ttu-id="f9937-106">В настоящее время в OneDrive для бизнеса и SharePoint доступен только **takenDateTime** .</span><span class="sxs-lookup"><span data-stu-id="f9937-106">Currently, only **takenDateTime** is available on OneDrive for Business and SharePoint.</span></span>

## <a name="properties"></a><span data-ttu-id="f9937-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f9937-107">Properties</span></span>

| <span data-ttu-id="f9937-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="f9937-108">Property</span></span>          | <span data-ttu-id="f9937-109">Тип</span><span class="sxs-lookup"><span data-stu-id="f9937-109">Type</span></span>          | <span data-ttu-id="f9937-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f9937-110">Description</span></span>                                                                |
|:------------------|:--------------|:---------------------------------------------------------------------------|
|<span data-ttu-id="f9937-111">cameraMake</span><span class="sxs-lookup"><span data-stu-id="f9937-111">cameraMake</span></span>         |<span data-ttu-id="f9937-112">Строка</span><span class="sxs-lookup"><span data-stu-id="f9937-112">String</span></span>         | <span data-ttu-id="f9937-p101">Изготовитель камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f9937-p101">Camera manufacturer. Read-only.</span></span>                                            |
|<span data-ttu-id="f9937-115">cameraModel</span><span class="sxs-lookup"><span data-stu-id="f9937-115">cameraModel</span></span>        |<span data-ttu-id="f9937-116">String</span><span class="sxs-lookup"><span data-stu-id="f9937-116">String</span></span>         | <span data-ttu-id="f9937-p102">Модель камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f9937-p102">Camera model. Read-only.</span></span>                                                   |
|<span data-ttu-id="f9937-119">exposureDenominator</span><span class="sxs-lookup"><span data-stu-id="f9937-119">exposureDenominator</span></span>|<span data-ttu-id="f9937-120">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="f9937-120">Double</span></span>         | <span data-ttu-id="f9937-p103">Знаменатель дробного значения выдержки камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f9937-p103">The denominator for the exposure time fraction from the camera. Read-only.</span></span> |
|<span data-ttu-id="f9937-123">exposureNumerator</span><span class="sxs-lookup"><span data-stu-id="f9937-123">exposureNumerator</span></span>  |<span data-ttu-id="f9937-124">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="f9937-124">Double</span></span>         | <span data-ttu-id="f9937-p104">Числитель дробного значения выдержки камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f9937-p104">The numerator for the exposure time fraction from the camera. Read-only.</span></span>   |
|<span data-ttu-id="f9937-127">fNumber</span><span class="sxs-lookup"><span data-stu-id="f9937-127">fNumber</span></span>            |<span data-ttu-id="f9937-128">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="f9937-128">Double</span></span>         | <span data-ttu-id="f9937-p105">Значение диафрагмы камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f9937-p105">The F-stop value from the camera. Read-only.</span></span>                               |
|<span data-ttu-id="f9937-131">focalLength</span><span class="sxs-lookup"><span data-stu-id="f9937-131">focalLength</span></span>        |<span data-ttu-id="f9937-132">Double</span><span class="sxs-lookup"><span data-stu-id="f9937-132">Double</span></span>         | <span data-ttu-id="f9937-p106">Фокусное расстояние камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f9937-p106">The focal length from the camera. Read-only.</span></span>                               |
|<span data-ttu-id="f9937-135">iso</span><span class="sxs-lookup"><span data-stu-id="f9937-135">iso</span></span>                |<span data-ttu-id="f9937-136">Int32</span><span class="sxs-lookup"><span data-stu-id="f9937-136">Int32</span></span>          | <span data-ttu-id="f9937-p107">Значение ISO камеры. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f9937-p107">The ISO value from the camera. Read-only.</span></span>                                  |
|<span data-ttu-id="f9937-139">orientation</span><span class="sxs-lookup"><span data-stu-id="f9937-139">orientation</span></span>        |<span data-ttu-id="f9937-140">Int16</span><span class="sxs-lookup"><span data-stu-id="f9937-140">Int16</span></span>          | <span data-ttu-id="f9937-141">Значение ориентации камеры.</span><span class="sxs-lookup"><span data-stu-id="f9937-141">The orientation value from the camera.</span></span> <span data-ttu-id="f9937-142">Возможность записи в OneDrive персональный.</span><span class="sxs-lookup"><span data-stu-id="f9937-142">Writable on OneDrive Personal.</span></span>      |
|<span data-ttu-id="f9937-143">takenDateTime</span><span class="sxs-lookup"><span data-stu-id="f9937-143">takenDateTime</span></span>      |<span data-ttu-id="f9937-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9937-144">DateTimeOffset</span></span> | <span data-ttu-id="f9937-145">Дата и время, когда фотография заняла время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="f9937-145">The date and time the photo was taken in UTC time.</span></span> <span data-ttu-id="f9937-146">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f9937-146">Read-only.</span></span>              |

## <a name="json-representation"></a><span data-ttu-id="f9937-147">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f9937-147">JSON representation</span></span>

<span data-ttu-id="f9937-148">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f9937-148">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.photo",
  "baseType": null
}-->

```json
{
  "cameraMake": "String",
  "cameraModel": "String",
  "exposureDenominator": 1000.0,
  "exposureNumerator": 1.0,
  "fNumber": 1.8,
  "focalLength": 22.5,
  "iso": 100,
  "orientation": 3,
  "takenDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The photo resource provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso, orientation",
  "section": "documentation",
  "tocPath": ""
}-->
