---
title: Тип ресурса mediaContentRatingIreland
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9a36d4e56d4d101c5cdf0ba198a6b3ea17d11bd1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028072"
---
# <a name="mediacontentratingireland-resource-type"></a><span data-ttu-id="0d5a5-103">Тип ресурса mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="0d5a5-103">mediaContentRatingIreland resource type</span></span>

> <span data-ttu-id="0d5a5-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0d5a5-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0d5a5-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="0d5a5-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="0d5a5-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="0d5a5-106">Properties</span></span>
|<span data-ttu-id="0d5a5-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="0d5a5-107">Property</span></span>|<span data-ttu-id="0d5a5-108">Тип</span><span class="sxs-lookup"><span data-stu-id="0d5a5-108">Type</span></span>|<span data-ttu-id="0d5a5-109">Описание</span><span class="sxs-lookup"><span data-stu-id="0d5a5-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d5a5-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="0d5a5-110">movieRating</span></span>|[<span data-ttu-id="0d5a5-111">Ратингиреландмовиестипе</span><span class="sxs-lookup"><span data-stu-id="0d5a5-111">ratingIrelandMoviesType</span></span>](../resources/intune-deviceconfig-ratingirelandmoviestype.md)|<span data-ttu-id="0d5a5-112">Оценка фильмов выбрана для Ирландии.</span><span class="sxs-lookup"><span data-stu-id="0d5a5-112">Movies rating selected for Ireland.</span></span> <span data-ttu-id="0d5a5-113">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="0d5a5-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="0d5a5-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="0d5a5-114">tvRating</span></span>|[<span data-ttu-id="0d5a5-115">Ратингиреландтелевисионтипе</span><span class="sxs-lookup"><span data-stu-id="0d5a5-115">ratingIrelandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingirelandtelevisiontype.md)|<span data-ttu-id="0d5a5-116">Рейтинг телевизора выбран для Ирландии.</span><span class="sxs-lookup"><span data-stu-id="0d5a5-116">TV rating selected for Ireland.</span></span> <span data-ttu-id="0d5a5-117">Возможные значения: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span><span class="sxs-lookup"><span data-stu-id="0d5a5-117">Possible values are: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0d5a5-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="0d5a5-118">Relationships</span></span>
<span data-ttu-id="0d5a5-119">Нет</span><span class="sxs-lookup"><span data-stu-id="0d5a5-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0d5a5-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0d5a5-120">JSON Representation</span></span>
<span data-ttu-id="0d5a5-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0d5a5-121">Here is a JSON representation of the resource.</span></span>
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



