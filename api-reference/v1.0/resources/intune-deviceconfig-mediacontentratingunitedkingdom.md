---
title: Тип ресурса mediaContentRatingUnitedKingdom
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 947fd12d8219215b0828ef1c05d2d8b36f970f16
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32572306"
---
# <a name="mediacontentratingunitedkingdom-resource-type"></a><span data-ttu-id="28bf0-103">Тип ресурса mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="28bf0-103">mediaContentRatingUnitedKingdom resource type</span></span>

> <span data-ttu-id="28bf0-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="28bf0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="28bf0-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="28bf0-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="28bf0-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="28bf0-106">Properties</span></span>
|<span data-ttu-id="28bf0-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="28bf0-107">Property</span></span>|<span data-ttu-id="28bf0-108">Тип</span><span class="sxs-lookup"><span data-stu-id="28bf0-108">Type</span></span>|<span data-ttu-id="28bf0-109">Описание</span><span class="sxs-lookup"><span data-stu-id="28bf0-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28bf0-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="28bf0-110">movieRating</span></span>|[<span data-ttu-id="28bf0-111">Ратингунитедкингдоммовиестипе</span><span class="sxs-lookup"><span data-stu-id="28bf0-111">ratingUnitedKingdomMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdommoviestype.md)|<span data-ttu-id="28bf0-112">Оценка фильмов выбрана для Великобритании.</span><span class="sxs-lookup"><span data-stu-id="28bf0-112">Movies rating selected for United Kingdom.</span></span> <span data-ttu-id="28bf0-113">Возможные значения: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="28bf0-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span></span>|
|<span data-ttu-id="28bf0-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="28bf0-114">tvRating</span></span>|[<span data-ttu-id="28bf0-115">Ратингунитедкингдомтелевисионтипе</span><span class="sxs-lookup"><span data-stu-id="28bf0-115">ratingUnitedKingdomTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdomtelevisiontype.md)|<span data-ttu-id="28bf0-116">Рейтинг для телевизора выбран для Великобритании.</span><span class="sxs-lookup"><span data-stu-id="28bf0-116">TV rating selected for United Kingdom.</span></span> <span data-ttu-id="28bf0-117">Возможные значения: `allAllowed`, `allBlocked`, `caution`.</span><span class="sxs-lookup"><span data-stu-id="28bf0-117">Possible values are: `allAllowed`, `allBlocked`, `caution`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="28bf0-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="28bf0-118">Relationships</span></span>
<span data-ttu-id="28bf0-119">Нет</span><span class="sxs-lookup"><span data-stu-id="28bf0-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="28bf0-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="28bf0-120">JSON Representation</span></span>
<span data-ttu-id="28bf0-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="28bf0-121">Here is a JSON representation of the resource.</span></span>
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



