---
title: Тип ресурса mediaContentRatingUnitedKingdom
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0169e26be7590031ba5e7e7f676d51f69a526452
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30160181"
---
# <a name="mediacontentratingunitedkingdom-resource-type"></a><span data-ttu-id="e5dd2-103">Тип ресурса mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="e5dd2-103">mediaContentRatingUnitedKingdom resource type</span></span>

> <span data-ttu-id="e5dd2-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5dd2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e5dd2-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e5dd2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5dd2-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="e5dd2-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="e5dd2-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="e5dd2-107">Properties</span></span>
|<span data-ttu-id="e5dd2-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="e5dd2-108">Property</span></span>|<span data-ttu-id="e5dd2-109">Тип</span><span class="sxs-lookup"><span data-stu-id="e5dd2-109">Type</span></span>|<span data-ttu-id="e5dd2-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e5dd2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5dd2-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="e5dd2-111">movieRating</span></span>|[<span data-ttu-id="e5dd2-112">Ратингунитедкингдоммовиестипе</span><span class="sxs-lookup"><span data-stu-id="e5dd2-112">ratingUnitedKingdomMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdommoviestype.md)|<span data-ttu-id="e5dd2-113">Оценка фильмов выбрана для Великобритании.</span><span class="sxs-lookup"><span data-stu-id="e5dd2-113">Movies rating selected for United Kingdom.</span></span> <span data-ttu-id="e5dd2-114">Возможные значения: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="e5dd2-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span></span>|
|<span data-ttu-id="e5dd2-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="e5dd2-115">tvRating</span></span>|[<span data-ttu-id="e5dd2-116">Ратингунитедкингдомтелевисионтипе</span><span class="sxs-lookup"><span data-stu-id="e5dd2-116">ratingUnitedKingdomTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdomtelevisiontype.md)|<span data-ttu-id="e5dd2-117">Рейтинг для телевизора выбран для Великобритании.</span><span class="sxs-lookup"><span data-stu-id="e5dd2-117">TV rating selected for United Kingdom.</span></span> <span data-ttu-id="e5dd2-118">Возможные значения: `allAllowed`, `allBlocked`, `caution`.</span><span class="sxs-lookup"><span data-stu-id="e5dd2-118">Possible values are: `allAllowed`, `allBlocked`, `caution`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e5dd2-119">Связи</span><span class="sxs-lookup"><span data-stu-id="e5dd2-119">Relationships</span></span>
<span data-ttu-id="e5dd2-120">Нет</span><span class="sxs-lookup"><span data-stu-id="e5dd2-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e5dd2-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e5dd2-121">JSON Representation</span></span>
<span data-ttu-id="e5dd2-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e5dd2-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingUnitedKingdom"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingUnitedKingdom",
  "movieRating": "String",
  "tvRating": "String"
}
```




