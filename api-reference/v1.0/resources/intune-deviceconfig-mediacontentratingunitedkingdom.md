---
title: Тип ресурса mediaContentRatingUnitedKingdom
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 947fd12d8219215b0828ef1c05d2d8b36f970f16
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30252457"
---
# <a name="mediacontentratingunitedkingdom-resource-type"></a><span data-ttu-id="9d74f-103">Тип ресурса mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="9d74f-103">mediaContentRatingUnitedKingdom resource type</span></span>

> <span data-ttu-id="9d74f-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9d74f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9d74f-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="9d74f-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="9d74f-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="9d74f-106">Properties</span></span>
|<span data-ttu-id="9d74f-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="9d74f-107">Property</span></span>|<span data-ttu-id="9d74f-108">Тип</span><span class="sxs-lookup"><span data-stu-id="9d74f-108">Type</span></span>|<span data-ttu-id="9d74f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="9d74f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d74f-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="9d74f-110">movieRating</span></span>|[<span data-ttu-id="9d74f-111">Ратингунитедкингдоммовиестипе</span><span class="sxs-lookup"><span data-stu-id="9d74f-111">ratingUnitedKingdomMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdommoviestype.md)|<span data-ttu-id="9d74f-112">Оценка фильмов выбрана для Великобритании.</span><span class="sxs-lookup"><span data-stu-id="9d74f-112">Movies rating selected for United Kingdom.</span></span> <span data-ttu-id="9d74f-113">Возможные значения: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="9d74f-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span></span>|
|<span data-ttu-id="9d74f-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="9d74f-114">tvRating</span></span>|[<span data-ttu-id="9d74f-115">Ратингунитедкингдомтелевисионтипе</span><span class="sxs-lookup"><span data-stu-id="9d74f-115">ratingUnitedKingdomTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdomtelevisiontype.md)|<span data-ttu-id="9d74f-116">Рейтинг для телевизора выбран для Великобритании.</span><span class="sxs-lookup"><span data-stu-id="9d74f-116">TV rating selected for United Kingdom.</span></span> <span data-ttu-id="9d74f-117">Возможные значения: `allAllowed`, `allBlocked`, `caution`.</span><span class="sxs-lookup"><span data-stu-id="9d74f-117">Possible values are: `allAllowed`, `allBlocked`, `caution`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9d74f-118">Связи</span><span class="sxs-lookup"><span data-stu-id="9d74f-118">Relationships</span></span>
<span data-ttu-id="9d74f-119">Нет</span><span class="sxs-lookup"><span data-stu-id="9d74f-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9d74f-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9d74f-120">JSON Representation</span></span>
<span data-ttu-id="9d74f-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9d74f-121">Here is a JSON representation of the resource.</span></span>
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



