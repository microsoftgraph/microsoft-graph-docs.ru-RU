---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: GeoCoordinates
ms.openlocfilehash: f9110591ee1e3350979aa2c7785cdebb2d4a584c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078237"
---
# <a name="geocoordinates-resource-type"></a><span data-ttu-id="dbacf-102">Тип ресурса GeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="dbacf-102">GeoCoordinates resource type</span></span>

> <span data-ttu-id="dbacf-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="dbacf-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dbacf-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dbacf-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dbacf-p102">Ресурс **GeoCoordinates** предоставляет географические координаты и высоту расположения в соответствии с метаданными файла. Если у ресурса [**DriveItem**](driveitem.md) есть ненулевой аспект **location**, то этот ресурс представляет файл, с которым связано известное расположение.</span><span class="sxs-lookup"><span data-stu-id="dbacf-p102">The **GeoCoordinates** resource provides geographic coordinates and elevation of a location based on metadata contained within the file. If a [**DriveItem**](driveitem.md) has a non-null **location** facet, the item represents a file with a known location assocaited with it.</span></span>

## <a name="json-representation"></a><span data-ttu-id="dbacf-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dbacf-107">JSON representation</span></span>

<span data-ttu-id="dbacf-108">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="dbacf-108">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.geoCoordinates"
}-->

```json
{
  "altitude": 1024.13,
  "latitude": 26.13246,
  "longitude": 24.34616
}
```

## <a name="properties"></a><span data-ttu-id="dbacf-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="dbacf-109">Properties</span></span>

| <span data-ttu-id="dbacf-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="dbacf-110">Property</span></span>  | <span data-ttu-id="dbacf-111">Тип</span><span class="sxs-lookup"><span data-stu-id="dbacf-111">Type</span></span>   | <span data-ttu-id="dbacf-112">Описание</span><span class="sxs-lookup"><span data-stu-id="dbacf-112">Description</span></span>
|:----------|:-------|:--------------------------------------------------------
| <span data-ttu-id="dbacf-113">altitude</span><span class="sxs-lookup"><span data-stu-id="dbacf-113">altitude</span></span>  | <span data-ttu-id="dbacf-114">Double</span><span class="sxs-lookup"><span data-stu-id="dbacf-114">Double</span></span> | <span data-ttu-id="dbacf-p103">Необязательный. Высота элемента над уровнем моря (в футах). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="dbacf-p103">Optional. The altitude (height), in feet,  above sea level for the item. Read-only.</span></span>
| <span data-ttu-id="dbacf-118">latitude</span><span class="sxs-lookup"><span data-stu-id="dbacf-118">latitude</span></span>  | <span data-ttu-id="dbacf-119">Double</span><span class="sxs-lookup"><span data-stu-id="dbacf-119">Double</span></span> | <span data-ttu-id="dbacf-p104">Необязательный. Широта элемента (в десятичной системе). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="dbacf-p104">Optional. The latitude, in decimal, for the item. Read-only.</span></span>
| <span data-ttu-id="dbacf-123">longitude</span><span class="sxs-lookup"><span data-stu-id="dbacf-123">longitude</span></span> | <span data-ttu-id="dbacf-124">Double</span><span class="sxs-lookup"><span data-stu-id="dbacf-124">Double</span></span> | <span data-ttu-id="dbacf-p105">Необязательный. Широта элемента (в десятичном виде). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="dbacf-p105">Optional. The longitude, in decimal, for the item. Read-only.</span></span>

## <a name="remarks"></a><span data-ttu-id="dbacf-128">Заметки</span><span class="sxs-lookup"><span data-stu-id="dbacf-128">Remarks</span></span>

<span data-ttu-id="dbacf-129">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="dbacf-129">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The location facet provides geographic location related properties for an item",
  "keywords": "location,geographic,item,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Location"
} -->
