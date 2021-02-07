---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: GeoCoordinates
localization_priority: Normal
description: Ресурс GeoCoordinates предоставляет географические координаты и высоту расположения в соответствии с метаданными файла.
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 048fefc8938a789a0aae06f3dd6f50c25c305c31
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130510"
---
# <a name="geocoordinates-resource-type"></a><span data-ttu-id="3aa6b-103">Тип ресурса GeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="3aa6b-103">GeoCoordinates resource type</span></span>

<span data-ttu-id="3aa6b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3aa6b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3aa6b-p101">Ресурс **GeoCoordinates** предоставляет географические координаты и высоту расположения в соответствии с метаданными файла. Если у ресурса [**DriveItem**](driveitem.md) есть ненулевой аспект **location**, то этот ресурс представляет файл, с которым связано известное расположение.</span><span class="sxs-lookup"><span data-stu-id="3aa6b-p101">The **GeoCoordinates** resource provides geographic coordinates and elevation of a location based on metadata contained within the file. If a [**DriveItem**](driveitem.md) has a non-null **location** facet, the item represents a file with a known location assocaited with it.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3aa6b-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3aa6b-107">JSON representation</span></span>

<span data-ttu-id="3aa6b-108">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="3aa6b-108">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="3aa6b-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="3aa6b-109">Properties</span></span>

| <span data-ttu-id="3aa6b-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="3aa6b-110">Property</span></span>  | <span data-ttu-id="3aa6b-111">Тип</span><span class="sxs-lookup"><span data-stu-id="3aa6b-111">Type</span></span>   | <span data-ttu-id="3aa6b-112">Описание</span><span class="sxs-lookup"><span data-stu-id="3aa6b-112">Description</span></span>
|:----------|:-------|:--------------------------------------------------------
| <span data-ttu-id="3aa6b-113">altitude</span><span class="sxs-lookup"><span data-stu-id="3aa6b-113">altitude</span></span>  | <span data-ttu-id="3aa6b-114">Double</span><span class="sxs-lookup"><span data-stu-id="3aa6b-114">Double</span></span> | <span data-ttu-id="3aa6b-p102">Необязательный. Высота элемента над уровнем моря (в футах). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3aa6b-p102">Optional. The altitude (height), in feet,  above sea level for the item. Read-only.</span></span>
| <span data-ttu-id="3aa6b-118">latitude</span><span class="sxs-lookup"><span data-stu-id="3aa6b-118">latitude</span></span>  | <span data-ttu-id="3aa6b-119">Double</span><span class="sxs-lookup"><span data-stu-id="3aa6b-119">Double</span></span> | <span data-ttu-id="3aa6b-p103">Необязательный. Широта элемента (в десятичной системе). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3aa6b-p103">Optional. The latitude, in decimal, for the item. Read-only.</span></span>
| <span data-ttu-id="3aa6b-123">longitude</span><span class="sxs-lookup"><span data-stu-id="3aa6b-123">longitude</span></span> | <span data-ttu-id="3aa6b-124">Double</span><span class="sxs-lookup"><span data-stu-id="3aa6b-124">Double</span></span> | <span data-ttu-id="3aa6b-p104">Необязательный. Широта элемента (в десятичном виде). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3aa6b-p104">Optional. The longitude, in decimal, for the item. Read-only.</span></span>

## <a name="remarks"></a><span data-ttu-id="3aa6b-128">Заметки</span><span class="sxs-lookup"><span data-stu-id="3aa6b-128">Remarks</span></span>

<span data-ttu-id="3aa6b-129">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="3aa6b-129">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The location facet provides geographic location related properties for an item",
  "keywords": "location,geographic,item,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Location"
} -->

