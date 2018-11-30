---
title: Тип ресурса mediaContentRatingUnitedKingdom
description: Н/Д
ms.openlocfilehash: 8bc3b7cf1de10a6ef5b72feb7e633018766b0397
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025547"
---
# <a name="mediacontentratingunitedkingdom-resource-type"></a><span data-ttu-id="a4bb7-103">Тип ресурса mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="a4bb7-103">mediaContentRatingUnitedKingdom resource type</span></span>

> <span data-ttu-id="a4bb7-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a4bb7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a4bb7-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="a4bb7-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="a4bb7-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="a4bb7-106">Properties</span></span>
|<span data-ttu-id="a4bb7-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="a4bb7-107">Property</span></span>|<span data-ttu-id="a4bb7-108">Тип</span><span class="sxs-lookup"><span data-stu-id="a4bb7-108">Type</span></span>|<span data-ttu-id="a4bb7-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a4bb7-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4bb7-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="a4bb7-110">movieRating</span></span>|[<span data-ttu-id="a4bb7-111">ratingUnitedKingdomMoviesType</span><span class="sxs-lookup"><span data-stu-id="a4bb7-111">ratingUnitedKingdomMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdommoviestype.md)|<span data-ttu-id="a4bb7-112">Оценка выбранных для Великобритании фильмы.</span><span class="sxs-lookup"><span data-stu-id="a4bb7-112">Movies rating selected for United Kingdom.</span></span> <span data-ttu-id="a4bb7-113">Возможные значения: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="a4bb7-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span></span>|
|<span data-ttu-id="a4bb7-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="a4bb7-114">tvRating</span></span>|[<span data-ttu-id="a4bb7-115">ratingUnitedKingdomTelevisionType</span><span class="sxs-lookup"><span data-stu-id="a4bb7-115">ratingUnitedKingdomTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdomtelevisiontype.md)|<span data-ttu-id="a4bb7-116">Оценка TV, выбранные для Великобритании.</span><span class="sxs-lookup"><span data-stu-id="a4bb7-116">TV rating selected for United Kingdom.</span></span> <span data-ttu-id="a4bb7-117">Возможные значения: `allAllowed`, `allBlocked`, `caution`.</span><span class="sxs-lookup"><span data-stu-id="a4bb7-117">Possible values are: `allAllowed`, `allBlocked`, `caution`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a4bb7-118">Связи</span><span class="sxs-lookup"><span data-stu-id="a4bb7-118">Relationships</span></span>
<span data-ttu-id="a4bb7-119">Нет</span><span class="sxs-lookup"><span data-stu-id="a4bb7-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a4bb7-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a4bb7-120">JSON Representation</span></span>
<span data-ttu-id="a4bb7-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a4bb7-121">Here is a JSON representation of the resource.</span></span>
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



