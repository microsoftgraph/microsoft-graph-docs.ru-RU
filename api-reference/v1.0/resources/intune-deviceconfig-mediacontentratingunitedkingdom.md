---
title: Тип ресурса mediaContentRatingUnitedKingdom
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 0a3f1caa48b7890fa25b356d6105b21638033f3f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829941"
---
# <a name="mediacontentratingunitedkingdom-resource-type"></a><span data-ttu-id="40e35-103">Тип ресурса mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="40e35-103">mediaContentRatingUnitedKingdom resource type</span></span>

> <span data-ttu-id="40e35-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="40e35-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="40e35-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="40e35-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="40e35-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="40e35-106">Properties</span></span>
|<span data-ttu-id="40e35-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="40e35-107">Property</span></span>|<span data-ttu-id="40e35-108">Тип</span><span class="sxs-lookup"><span data-stu-id="40e35-108">Type</span></span>|<span data-ttu-id="40e35-109">Описание</span><span class="sxs-lookup"><span data-stu-id="40e35-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40e35-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="40e35-110">movieRating</span></span>|[<span data-ttu-id="40e35-111">ratingUnitedKingdomMoviesType</span><span class="sxs-lookup"><span data-stu-id="40e35-111">ratingUnitedKingdomMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdommoviestype.md)|<span data-ttu-id="40e35-112">Оценка выбранных для Великобритании фильмы.</span><span class="sxs-lookup"><span data-stu-id="40e35-112">Movies rating selected for United Kingdom.</span></span> <span data-ttu-id="40e35-113">Возможные значения: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="40e35-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span></span>|
|<span data-ttu-id="40e35-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="40e35-114">tvRating</span></span>|[<span data-ttu-id="40e35-115">ratingUnitedKingdomTelevisionType</span><span class="sxs-lookup"><span data-stu-id="40e35-115">ratingUnitedKingdomTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdomtelevisiontype.md)|<span data-ttu-id="40e35-116">Оценка TV, выбранные для Великобритании.</span><span class="sxs-lookup"><span data-stu-id="40e35-116">TV rating selected for United Kingdom.</span></span> <span data-ttu-id="40e35-117">Возможные значения: `allAllowed`, `allBlocked`, `caution`.</span><span class="sxs-lookup"><span data-stu-id="40e35-117">Possible values are: `allAllowed`, `allBlocked`, `caution`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="40e35-118">Связи</span><span class="sxs-lookup"><span data-stu-id="40e35-118">Relationships</span></span>
<span data-ttu-id="40e35-119">Нет</span><span class="sxs-lookup"><span data-stu-id="40e35-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="40e35-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="40e35-120">JSON Representation</span></span>
<span data-ttu-id="40e35-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="40e35-121">Here is a JSON representation of the resource.</span></span>
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



