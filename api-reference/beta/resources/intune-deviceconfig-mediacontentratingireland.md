---
title: Тип ресурса mediaContentRatingIreland
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a17ea1ddbd4e63af846ab6343f66f4a5726e9739
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140980"
---
# <a name="mediacontentratingireland-resource-type"></a><span data-ttu-id="13ae3-103">Тип ресурса mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="13ae3-103">mediaContentRatingIreland resource type</span></span>

> <span data-ttu-id="13ae3-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13ae3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="13ae3-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="13ae3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13ae3-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="13ae3-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="13ae3-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="13ae3-107">Properties</span></span>
|<span data-ttu-id="13ae3-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="13ae3-108">Property</span></span>|<span data-ttu-id="13ae3-109">Тип</span><span class="sxs-lookup"><span data-stu-id="13ae3-109">Type</span></span>|<span data-ttu-id="13ae3-110">Описание</span><span class="sxs-lookup"><span data-stu-id="13ae3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13ae3-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="13ae3-111">movieRating</span></span>|[<span data-ttu-id="13ae3-112">Ратингиреландмовиестипе</span><span class="sxs-lookup"><span data-stu-id="13ae3-112">ratingIrelandMoviesType</span></span>](../resources/intune-deviceconfig-ratingirelandmoviestype.md)|<span data-ttu-id="13ae3-113">Оценка фильмов выбрана для Ирландии.</span><span class="sxs-lookup"><span data-stu-id="13ae3-113">Movies rating selected for Ireland.</span></span> <span data-ttu-id="13ae3-114">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="13ae3-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="13ae3-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="13ae3-115">tvRating</span></span>|[<span data-ttu-id="13ae3-116">Ратингиреландтелевисионтипе</span><span class="sxs-lookup"><span data-stu-id="13ae3-116">ratingIrelandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingirelandtelevisiontype.md)|<span data-ttu-id="13ae3-117">Рейтинг телевизора выбран для Ирландии.</span><span class="sxs-lookup"><span data-stu-id="13ae3-117">TV rating selected for Ireland.</span></span> <span data-ttu-id="13ae3-118">Возможные значения: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span><span class="sxs-lookup"><span data-stu-id="13ae3-118">Possible values are: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="13ae3-119">Связи</span><span class="sxs-lookup"><span data-stu-id="13ae3-119">Relationships</span></span>
<span data-ttu-id="13ae3-120">Нет</span><span class="sxs-lookup"><span data-stu-id="13ae3-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="13ae3-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="13ae3-121">JSON Representation</span></span>
<span data-ttu-id="13ae3-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="13ae3-122">Here is a JSON representation of the resource.</span></span>
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




