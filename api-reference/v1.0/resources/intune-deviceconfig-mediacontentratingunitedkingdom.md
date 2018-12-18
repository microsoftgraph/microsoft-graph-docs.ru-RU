---
title: Тип ресурса mediaContentRatingUnitedKingdom
description: Н/Д
author: tfitzmac
ms.openlocfilehash: 0fcd17f27d999f933ce6824f8a49018013341c7b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27315535"
---
# <a name="mediacontentratingunitedkingdom-resource-type"></a><span data-ttu-id="80b6b-103">Тип ресурса mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="80b6b-103">mediaContentRatingUnitedKingdom resource type</span></span>

> <span data-ttu-id="80b6b-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="80b6b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="80b6b-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="80b6b-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="80b6b-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="80b6b-106">Properties</span></span>
|<span data-ttu-id="80b6b-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="80b6b-107">Property</span></span>|<span data-ttu-id="80b6b-108">Тип</span><span class="sxs-lookup"><span data-stu-id="80b6b-108">Type</span></span>|<span data-ttu-id="80b6b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="80b6b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80b6b-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="80b6b-110">movieRating</span></span>|[<span data-ttu-id="80b6b-111">ratingUnitedKingdomMoviesType</span><span class="sxs-lookup"><span data-stu-id="80b6b-111">ratingUnitedKingdomMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdommoviestype.md)|<span data-ttu-id="80b6b-112">Оценка выбранных для Великобритании фильмы.</span><span class="sxs-lookup"><span data-stu-id="80b6b-112">Movies rating selected for United Kingdom.</span></span> <span data-ttu-id="80b6b-113">Возможные значения: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="80b6b-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span></span>|
|<span data-ttu-id="80b6b-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="80b6b-114">tvRating</span></span>|[<span data-ttu-id="80b6b-115">ratingUnitedKingdomTelevisionType</span><span class="sxs-lookup"><span data-stu-id="80b6b-115">ratingUnitedKingdomTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdomtelevisiontype.md)|<span data-ttu-id="80b6b-116">Оценка TV, выбранные для Великобритании.</span><span class="sxs-lookup"><span data-stu-id="80b6b-116">TV rating selected for United Kingdom.</span></span> <span data-ttu-id="80b6b-117">Возможные значения: `allAllowed`, `allBlocked`, `caution`.</span><span class="sxs-lookup"><span data-stu-id="80b6b-117">Possible values are: `allAllowed`, `allBlocked`, `caution`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="80b6b-118">Связи</span><span class="sxs-lookup"><span data-stu-id="80b6b-118">Relationships</span></span>
<span data-ttu-id="80b6b-119">Нет</span><span class="sxs-lookup"><span data-stu-id="80b6b-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="80b6b-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="80b6b-120">JSON Representation</span></span>
<span data-ttu-id="80b6b-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="80b6b-121">Here is a JSON representation of the resource.</span></span>
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



