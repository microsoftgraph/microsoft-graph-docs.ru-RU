---
title: Тип ресурса mediaContentRatingUnitedKingdom
description: Н/Д
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7d21ac4650072c4523f9e120d5d73ad393686635
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29408077"
---
# <a name="mediacontentratingunitedkingdom-resource-type"></a><span data-ttu-id="fb58e-103">Тип ресурса mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="fb58e-103">mediaContentRatingUnitedKingdom resource type</span></span>

> <span data-ttu-id="fb58e-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fb58e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fb58e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb58e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fb58e-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fb58e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fb58e-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="fb58e-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="fb58e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="fb58e-108">Properties</span></span>
|<span data-ttu-id="fb58e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="fb58e-109">Property</span></span>|<span data-ttu-id="fb58e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="fb58e-110">Type</span></span>|<span data-ttu-id="fb58e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="fb58e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb58e-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="fb58e-112">movieRating</span></span>|[<span data-ttu-id="fb58e-113">ratingUnitedKingdomMoviesType</span><span class="sxs-lookup"><span data-stu-id="fb58e-113">ratingUnitedKingdomMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdommoviestype.md)|<span data-ttu-id="fb58e-114">Оценка выбранных для Великобритании фильмы.</span><span class="sxs-lookup"><span data-stu-id="fb58e-114">Movies rating selected for United Kingdom.</span></span> <span data-ttu-id="fb58e-115">Возможные значения: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="fb58e-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span></span>|
|<span data-ttu-id="fb58e-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="fb58e-116">tvRating</span></span>|[<span data-ttu-id="fb58e-117">ratingUnitedKingdomTelevisionType</span><span class="sxs-lookup"><span data-stu-id="fb58e-117">ratingUnitedKingdomTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdomtelevisiontype.md)|<span data-ttu-id="fb58e-118">Оценка TV, выбранные для Великобритании.</span><span class="sxs-lookup"><span data-stu-id="fb58e-118">TV rating selected for United Kingdom.</span></span> <span data-ttu-id="fb58e-119">Возможные значения: `allAllowed`, `allBlocked`, `caution`.</span><span class="sxs-lookup"><span data-stu-id="fb58e-119">Possible values are: `allAllowed`, `allBlocked`, `caution`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fb58e-120">Связи</span><span class="sxs-lookup"><span data-stu-id="fb58e-120">Relationships</span></span>
<span data-ttu-id="fb58e-121">Нет</span><span class="sxs-lookup"><span data-stu-id="fb58e-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fb58e-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fb58e-122">JSON Representation</span></span>
<span data-ttu-id="fb58e-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fb58e-123">Here is a JSON representation of the resource.</span></span>
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




