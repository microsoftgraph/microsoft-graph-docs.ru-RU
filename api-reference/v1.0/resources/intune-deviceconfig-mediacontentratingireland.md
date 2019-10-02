---
title: Тип ресурса mediaContentRatingIreland
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7aa885ddf964e11cd5cd6c364b98501b5f67c1ff
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37359959"
---
# <a name="mediacontentratingireland-resource-type"></a><span data-ttu-id="1ee1f-103">Тип ресурса mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="1ee1f-103">mediaContentRatingIreland resource type</span></span>

> <span data-ttu-id="1ee1f-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1ee1f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1ee1f-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="1ee1f-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="1ee1f-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="1ee1f-106">Properties</span></span>
|<span data-ttu-id="1ee1f-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="1ee1f-107">Property</span></span>|<span data-ttu-id="1ee1f-108">Тип</span><span class="sxs-lookup"><span data-stu-id="1ee1f-108">Type</span></span>|<span data-ttu-id="1ee1f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="1ee1f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ee1f-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="1ee1f-110">movieRating</span></span>|[<span data-ttu-id="1ee1f-111">ратингиреландмовиестипе</span><span class="sxs-lookup"><span data-stu-id="1ee1f-111">ratingIrelandMoviesType</span></span>](../resources/intune-deviceconfig-ratingirelandmoviestype.md)|<span data-ttu-id="1ee1f-112">Оценка фильмов выбрана для Ирландии.</span><span class="sxs-lookup"><span data-stu-id="1ee1f-112">Movies rating selected for Ireland.</span></span> <span data-ttu-id="1ee1f-113">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="1ee1f-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="1ee1f-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="1ee1f-114">tvRating</span></span>|[<span data-ttu-id="1ee1f-115">ратингиреландтелевисионтипе</span><span class="sxs-lookup"><span data-stu-id="1ee1f-115">ratingIrelandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingirelandtelevisiontype.md)|<span data-ttu-id="1ee1f-116">Рейтинг телевизора выбран для Ирландии.</span><span class="sxs-lookup"><span data-stu-id="1ee1f-116">TV rating selected for Ireland.</span></span> <span data-ttu-id="1ee1f-117">Возможные значения: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span><span class="sxs-lookup"><span data-stu-id="1ee1f-117">Possible values are: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1ee1f-118">Связи</span><span class="sxs-lookup"><span data-stu-id="1ee1f-118">Relationships</span></span>
<span data-ttu-id="1ee1f-119">Нет</span><span class="sxs-lookup"><span data-stu-id="1ee1f-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1ee1f-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1ee1f-120">JSON Representation</span></span>
<span data-ttu-id="1ee1f-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1ee1f-121">Here is a JSON representation of the resource.</span></span>
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




