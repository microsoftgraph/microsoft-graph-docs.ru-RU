---
title: Тип ресурса mediaContentRatingFrance
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 40f4650a99c9914257e868ac7d84f34ed1369276
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37360001"
---
# <a name="mediacontentratingfrance-resource-type"></a><span data-ttu-id="97fe5-103">Тип ресурса mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="97fe5-103">mediaContentRatingFrance resource type</span></span>

> <span data-ttu-id="97fe5-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="97fe5-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="97fe5-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="97fe5-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="97fe5-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="97fe5-106">Properties</span></span>
|<span data-ttu-id="97fe5-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="97fe5-107">Property</span></span>|<span data-ttu-id="97fe5-108">Тип</span><span class="sxs-lookup"><span data-stu-id="97fe5-108">Type</span></span>|<span data-ttu-id="97fe5-109">Описание</span><span class="sxs-lookup"><span data-stu-id="97fe5-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97fe5-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="97fe5-110">movieRating</span></span>|[<span data-ttu-id="97fe5-111">ратингфранцемовиестипе</span><span class="sxs-lookup"><span data-stu-id="97fe5-111">ratingFranceMoviesType</span></span>](../resources/intune-deviceconfig-ratingfrancemoviestype.md)|<span data-ttu-id="97fe5-112">Оценка фильмов выбрана для Франции.</span><span class="sxs-lookup"><span data-stu-id="97fe5-112">Movies rating selected for France.</span></span> <span data-ttu-id="97fe5-113">Возможные значения: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="97fe5-113">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|
|<span data-ttu-id="97fe5-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="97fe5-114">tvRating</span></span>|[<span data-ttu-id="97fe5-115">ратингфранцетелевисионтипе</span><span class="sxs-lookup"><span data-stu-id="97fe5-115">ratingFranceTelevisionType</span></span>](../resources/intune-deviceconfig-ratingfrancetelevisiontype.md)|<span data-ttu-id="97fe5-116">Рейтинг телевизора выбран для Франции.</span><span class="sxs-lookup"><span data-stu-id="97fe5-116">TV rating selected for France.</span></span> <span data-ttu-id="97fe5-117">Возможные значения: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="97fe5-117">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="97fe5-118">Связи</span><span class="sxs-lookup"><span data-stu-id="97fe5-118">Relationships</span></span>
<span data-ttu-id="97fe5-119">Нет</span><span class="sxs-lookup"><span data-stu-id="97fe5-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="97fe5-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="97fe5-120">JSON Representation</span></span>
<span data-ttu-id="97fe5-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="97fe5-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingFrance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingFrance",
  "movieRating": "String",
  "tvRating": "String"
}
```




