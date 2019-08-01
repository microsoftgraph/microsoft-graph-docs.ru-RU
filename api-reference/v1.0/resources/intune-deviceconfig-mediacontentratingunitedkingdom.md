---
title: Тип ресурса mediaContentRatingUnitedKingdom
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e19ac4fd5fdc63d1635b3f831ebb0f96f934038b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031369"
---
# <a name="mediacontentratingunitedkingdom-resource-type"></a><span data-ttu-id="dafb6-103">Тип ресурса mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="dafb6-103">mediaContentRatingUnitedKingdom resource type</span></span>

> <span data-ttu-id="dafb6-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dafb6-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dafb6-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="dafb6-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="dafb6-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="dafb6-106">Properties</span></span>
|<span data-ttu-id="dafb6-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="dafb6-107">Property</span></span>|<span data-ttu-id="dafb6-108">Тип</span><span class="sxs-lookup"><span data-stu-id="dafb6-108">Type</span></span>|<span data-ttu-id="dafb6-109">Описание</span><span class="sxs-lookup"><span data-stu-id="dafb6-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dafb6-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="dafb6-110">movieRating</span></span>|[<span data-ttu-id="dafb6-111">Ратингунитедкингдоммовиестипе</span><span class="sxs-lookup"><span data-stu-id="dafb6-111">ratingUnitedKingdomMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdommoviestype.md)|<span data-ttu-id="dafb6-112">Оценка фильмов выбрана для Великобритании.</span><span class="sxs-lookup"><span data-stu-id="dafb6-112">Movies rating selected for United Kingdom.</span></span> <span data-ttu-id="dafb6-113">Возможные значения: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="dafb6-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span></span>|
|<span data-ttu-id="dafb6-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="dafb6-114">tvRating</span></span>|[<span data-ttu-id="dafb6-115">Ратингунитедкингдомтелевисионтипе</span><span class="sxs-lookup"><span data-stu-id="dafb6-115">ratingUnitedKingdomTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdomtelevisiontype.md)|<span data-ttu-id="dafb6-116">Рейтинг для телевизора выбран для Великобритании.</span><span class="sxs-lookup"><span data-stu-id="dafb6-116">TV rating selected for United Kingdom.</span></span> <span data-ttu-id="dafb6-117">Возможные значения: `allAllowed`, `allBlocked`, `caution`.</span><span class="sxs-lookup"><span data-stu-id="dafb6-117">Possible values are: `allAllowed`, `allBlocked`, `caution`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dafb6-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="dafb6-118">Relationships</span></span>
<span data-ttu-id="dafb6-119">Нет</span><span class="sxs-lookup"><span data-stu-id="dafb6-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dafb6-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dafb6-120">JSON Representation</span></span>
<span data-ttu-id="dafb6-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dafb6-121">Here is a JSON representation of the resource.</span></span>
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



