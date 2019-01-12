---
title: Тип ресурса mediaContentRatingUnitedKingdom
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8bdcd67bbc81cb5436c6be22c395a6c9804b0637
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951595"
---
# <a name="mediacontentratingunitedkingdom-resource-type"></a><span data-ttu-id="a1703-103">Тип ресурса mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="a1703-103">mediaContentRatingUnitedKingdom resource type</span></span>

> <span data-ttu-id="a1703-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a1703-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a1703-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="a1703-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="a1703-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="a1703-106">Properties</span></span>
|<span data-ttu-id="a1703-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="a1703-107">Property</span></span>|<span data-ttu-id="a1703-108">Тип</span><span class="sxs-lookup"><span data-stu-id="a1703-108">Type</span></span>|<span data-ttu-id="a1703-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a1703-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1703-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="a1703-110">movieRating</span></span>|[<span data-ttu-id="a1703-111">ratingUnitedKingdomMoviesType</span><span class="sxs-lookup"><span data-stu-id="a1703-111">ratingUnitedKingdomMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdommoviestype.md)|<span data-ttu-id="a1703-112">Оценка выбранных для Великобритании фильмы.</span><span class="sxs-lookup"><span data-stu-id="a1703-112">Movies rating selected for United Kingdom.</span></span> <span data-ttu-id="a1703-113">Возможные значения: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="a1703-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span></span>|
|<span data-ttu-id="a1703-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="a1703-114">tvRating</span></span>|[<span data-ttu-id="a1703-115">ratingUnitedKingdomTelevisionType</span><span class="sxs-lookup"><span data-stu-id="a1703-115">ratingUnitedKingdomTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdomtelevisiontype.md)|<span data-ttu-id="a1703-116">Оценка TV, выбранные для Великобритании.</span><span class="sxs-lookup"><span data-stu-id="a1703-116">TV rating selected for United Kingdom.</span></span> <span data-ttu-id="a1703-117">Возможные значения: `allAllowed`, `allBlocked`, `caution`.</span><span class="sxs-lookup"><span data-stu-id="a1703-117">Possible values are: `allAllowed`, `allBlocked`, `caution`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a1703-118">Связи</span><span class="sxs-lookup"><span data-stu-id="a1703-118">Relationships</span></span>
<span data-ttu-id="a1703-119">Нет</span><span class="sxs-lookup"><span data-stu-id="a1703-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a1703-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a1703-120">JSON Representation</span></span>
<span data-ttu-id="a1703-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a1703-121">Here is a JSON representation of the resource.</span></span>
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



