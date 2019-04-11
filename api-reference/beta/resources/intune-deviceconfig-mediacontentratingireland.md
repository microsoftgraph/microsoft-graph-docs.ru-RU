---
title: Тип ресурса mediaContentRatingIreland
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 22b0ad3bc1e83ab0a15c9e2185a5c7586fe31979
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31796033"
---
# <a name="mediacontentratingireland-resource-type"></a><span data-ttu-id="82f9d-103">Тип ресурса mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="82f9d-103">mediaContentRatingIreland resource type</span></span>

> <span data-ttu-id="82f9d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82f9d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="82f9d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="82f9d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82f9d-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="82f9d-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="82f9d-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="82f9d-107">Properties</span></span>
|<span data-ttu-id="82f9d-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="82f9d-108">Property</span></span>|<span data-ttu-id="82f9d-109">Тип</span><span class="sxs-lookup"><span data-stu-id="82f9d-109">Type</span></span>|<span data-ttu-id="82f9d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="82f9d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82f9d-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="82f9d-111">movieRating</span></span>|[<span data-ttu-id="82f9d-112">Ратингиреландмовиестипе</span><span class="sxs-lookup"><span data-stu-id="82f9d-112">ratingIrelandMoviesType</span></span>](../resources/intune-deviceconfig-ratingirelandmoviestype.md)|<span data-ttu-id="82f9d-113">Оценка фильмов выбрана для Ирландии.</span><span class="sxs-lookup"><span data-stu-id="82f9d-113">Movies rating selected for Ireland.</span></span> <span data-ttu-id="82f9d-114">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="82f9d-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="82f9d-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="82f9d-115">tvRating</span></span>|[<span data-ttu-id="82f9d-116">Ратингиреландтелевисионтипе</span><span class="sxs-lookup"><span data-stu-id="82f9d-116">ratingIrelandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingirelandtelevisiontype.md)|<span data-ttu-id="82f9d-117">Рейтинг телевизора выбран для Ирландии.</span><span class="sxs-lookup"><span data-stu-id="82f9d-117">TV rating selected for Ireland.</span></span> <span data-ttu-id="82f9d-118">Возможные значения: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span><span class="sxs-lookup"><span data-stu-id="82f9d-118">Possible values are: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="82f9d-119">Отношения</span><span class="sxs-lookup"><span data-stu-id="82f9d-119">Relationships</span></span>
<span data-ttu-id="82f9d-120">Нет</span><span class="sxs-lookup"><span data-stu-id="82f9d-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="82f9d-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="82f9d-121">JSON Representation</span></span>
<span data-ttu-id="82f9d-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="82f9d-122">Here is a JSON representation of the resource.</span></span>
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





