---
author: MarcMroz
description: DriveItemSource содержит метаданные об источнике приложения, в которое был создан элемент диска.
title: тип ресурса driveItemSource
localization_priority: Normal
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: a403f570ac550b62f9c0e7fa0c3c2fa9758e1772
ms.sourcegitcommit: 0adbbcbc65b6acab80e9195f13321055994f56be
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2021
ms.locfileid: "53236321"
---
# <a name="driveitemsource-resource-type"></a><span data-ttu-id="c1479-103">тип ресурса driveItemSource</span><span class="sxs-lookup"><span data-stu-id="c1479-103">driveItemSource resource type</span></span>

<span data-ttu-id="c1479-104">Содержит метаданные об источнике элемента диска.</span><span class="sxs-lookup"><span data-stu-id="c1479-104">Contains metadata about the source of the drive item.</span></span>

<span data-ttu-id="c1479-105">Он доступен в свойстве источника [ресурсов driveItem.][item-resource]</span><span class="sxs-lookup"><span data-stu-id="c1479-105">It is available on the source property of [driveItem][item-resource] resources.</span></span>

## <a name="properties"></a><span data-ttu-id="c1479-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="c1479-106">Properties</span></span>

| <span data-ttu-id="c1479-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="c1479-107">Property</span></span>                 | <span data-ttu-id="c1479-108">Тип</span><span class="sxs-lookup"><span data-stu-id="c1479-108">Type</span></span>                       | <span data-ttu-id="c1479-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c1479-109">Description</span></span>                                                                                      |
| :----------------------- | :------------------------  | :----------------------------------------------------------------------------------------------- |
| <span data-ttu-id="c1479-110">**application**</span><span class="sxs-lookup"><span data-stu-id="c1479-110">**application**</span></span>          | <span data-ttu-id="c1479-111">driveItemSourceApplication</span><span class="sxs-lookup"><span data-stu-id="c1479-111">driveItemSourceApplication</span></span> | <span data-ttu-id="c1479-112">Значение переумерия, которое указывает на источник приложения, в котором был создан файл.</span><span class="sxs-lookup"><span data-stu-id="c1479-112">Enumeration value that indicates the source application where the file was created.</span></span>              |
| <span data-ttu-id="c1479-113">**externalId**</span><span class="sxs-lookup"><span data-stu-id="c1479-113">**externalId**</span></span>           | <span data-ttu-id="c1479-114">строка</span><span class="sxs-lookup"><span data-stu-id="c1479-114">string</span></span>                     | <span data-ttu-id="c1479-115">Внешний идентификатор элемента диска из источника.</span><span class="sxs-lookup"><span data-stu-id="c1479-115">The external identifier for the drive item from the source.</span></span>                                      |

### <a name="driveitemsourceapplication-values"></a><span data-ttu-id="c1479-116">значения driveItemSourceApplication</span><span class="sxs-lookup"><span data-stu-id="c1479-116">driveItemSourceApplication values</span></span>

| <span data-ttu-id="c1479-117">Значение</span><span class="sxs-lookup"><span data-stu-id="c1479-117">Value</span></span>               | <span data-ttu-id="c1479-118">Описание</span><span class="sxs-lookup"><span data-stu-id="c1479-118">Description</span></span>                                       |
|:--------------------|:--------------------------------------------------|
| <span data-ttu-id="c1479-119">teams</span><span class="sxs-lookup"><span data-stu-id="c1479-119">teams</span></span>               | <span data-ttu-id="c1479-120">Приложение Teams.</span><span class="sxs-lookup"><span data-stu-id="c1479-120">The application is Teams.</span></span>                         |
| <span data-ttu-id="c1479-121">yammer</span><span class="sxs-lookup"><span data-stu-id="c1479-121">yammer</span></span>              | <span data-ttu-id="c1479-122">Приложение Yammer.</span><span class="sxs-lookup"><span data-stu-id="c1479-122">The application is Yammer.</span></span>                        |
| <span data-ttu-id="c1479-123">sharePoint</span><span class="sxs-lookup"><span data-stu-id="c1479-123">sharePoint</span></span>          | <span data-ttu-id="c1479-124">Приложение SharePoint.</span><span class="sxs-lookup"><span data-stu-id="c1479-124">The application is SharePoint.</span></span>                    |
| <span data-ttu-id="c1479-125">oneDrive</span><span class="sxs-lookup"><span data-stu-id="c1479-125">oneDrive</span></span>            | <span data-ttu-id="c1479-126">Приложение OneDrive.</span><span class="sxs-lookup"><span data-stu-id="c1479-126">The application is OneDrive.</span></span>                      |
| <span data-ttu-id="c1479-127">stream</span><span class="sxs-lookup"><span data-stu-id="c1479-127">stream</span></span>              | <span data-ttu-id="c1479-128">Приложение — Stream.</span><span class="sxs-lookup"><span data-stu-id="c1479-128">The application is Stream.</span></span>                        |
| <span data-ttu-id="c1479-129">powerPoint</span><span class="sxs-lookup"><span data-stu-id="c1479-129">powerPoint</span></span>          | <span data-ttu-id="c1479-130">Приложение PowerPoint</span><span class="sxs-lookup"><span data-stu-id="c1479-130">The application is PowerPoint</span></span>                     |
| <span data-ttu-id="c1479-131">Office</span><span class="sxs-lookup"><span data-stu-id="c1479-131">office</span></span>              | <span data-ttu-id="c1479-132">Приложение Office</span><span class="sxs-lookup"><span data-stu-id="c1479-132">The application is Office</span></span>                         |
| <span data-ttu-id="c1479-133">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="c1479-133">unknownFutureValue</span></span>  | <span data-ttu-id="c1479-134">Значение маркера для будущей совместимости.</span><span class="sxs-lookup"><span data-stu-id="c1479-134">Marker value for future compatibility.</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="c1479-135">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c1479-135">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "application",
    "externalId",
  ],
  "@odata.type": "microsoft.graph.driveItemSource"
}-->

```json
{
  "application": "string",
  "externalId" : "string"
}
```

## <a name="see-also"></a><span data-ttu-id="c1479-136">См. также</span><span class="sxs-lookup"><span data-stu-id="c1479-136">See also</span></span>

<span data-ttu-id="c1479-137">Дополнительные сведения о гранях на driveItem см. [в сайте driveItem.](driveitem.md)</span><span class="sxs-lookup"><span data-stu-id="c1479-137">For more information about the facets on a driveItem, see [driveItem](driveitem.md).</span></span>

[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "The driveItemSource facet provides information about drive item source.",
  "keywords": "driveItemSoruce,client,media info,onedrive",
  "section": "documentation",
  "tocPath&quot;: &quot;Facets/driveItemSource"
} -->
