---
title: Тип ресурса mediaContentRatingIreland
description: Н/Д
author: tfitzmac
ms.openlocfilehash: 68d5e0e9454fadde550988f46c1104733a9de013
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27359474"
---
# <a name="mediacontentratingireland-resource-type"></a><span data-ttu-id="e3841-103">Тип ресурса mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="e3841-103">mediaContentRatingIreland resource type</span></span>

> <span data-ttu-id="e3841-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e3841-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e3841-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="e3841-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="e3841-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="e3841-106">Properties</span></span>
|<span data-ttu-id="e3841-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="e3841-107">Property</span></span>|<span data-ttu-id="e3841-108">Тип</span><span class="sxs-lookup"><span data-stu-id="e3841-108">Type</span></span>|<span data-ttu-id="e3841-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e3841-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3841-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="e3841-110">movieRating</span></span>|[<span data-ttu-id="e3841-111">ratingIrelandMoviesType</span><span class="sxs-lookup"><span data-stu-id="e3841-111">ratingIrelandMoviesType</span></span>](../resources/intune-deviceconfig-ratingirelandmoviestype.md)|<span data-ttu-id="e3841-112">Оценка выбранных для Ирландия фильмы.</span><span class="sxs-lookup"><span data-stu-id="e3841-112">Movies rating selected for Ireland.</span></span> <span data-ttu-id="e3841-113">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="e3841-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="e3841-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="e3841-114">tvRating</span></span>|[<span data-ttu-id="e3841-115">ratingIrelandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="e3841-115">ratingIrelandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingirelandtelevisiontype.md)|<span data-ttu-id="e3841-116">Оценка TV, выбранной для Ирландия.</span><span class="sxs-lookup"><span data-stu-id="e3841-116">TV rating selected for Ireland.</span></span> <span data-ttu-id="e3841-117">Возможные значения: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span><span class="sxs-lookup"><span data-stu-id="e3841-117">Possible values are: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e3841-118">Связи</span><span class="sxs-lookup"><span data-stu-id="e3841-118">Relationships</span></span>
<span data-ttu-id="e3841-119">Нет</span><span class="sxs-lookup"><span data-stu-id="e3841-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e3841-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e3841-120">JSON Representation</span></span>
<span data-ttu-id="e3841-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e3841-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingIreland"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingIreland",
  "movieRating": "String",
  "tvRating": "String"
}
```



