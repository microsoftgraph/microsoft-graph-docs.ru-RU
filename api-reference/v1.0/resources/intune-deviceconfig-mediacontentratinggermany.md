---
title: Тип ресурса mediaContentRatingGermany
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7e3c59bf110c55492db49a81a557cef0b421e328
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260356"
---
# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="506fb-103">Тип ресурса mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="506fb-103">mediaContentRatingGermany resource type</span></span>

> <span data-ttu-id="506fb-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="506fb-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="506fb-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="506fb-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="506fb-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="506fb-106">Properties</span></span>
|<span data-ttu-id="506fb-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="506fb-107">Property</span></span>|<span data-ttu-id="506fb-108">Тип</span><span class="sxs-lookup"><span data-stu-id="506fb-108">Type</span></span>|<span data-ttu-id="506fb-109">Описание</span><span class="sxs-lookup"><span data-stu-id="506fb-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="506fb-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="506fb-110">movieRating</span></span>|[<span data-ttu-id="506fb-111">Ратингжерманимовиестипе</span><span class="sxs-lookup"><span data-stu-id="506fb-111">ratingGermanyMoviesType</span></span>](../resources/intune-deviceconfig-ratinggermanymoviestype.md)|<span data-ttu-id="506fb-112">Оценка фильмов выбрана для Германии.</span><span class="sxs-lookup"><span data-stu-id="506fb-112">Movies rating selected for Germany.</span></span> <span data-ttu-id="506fb-113">Возможные значения: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="506fb-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="506fb-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="506fb-114">tvRating</span></span>|[<span data-ttu-id="506fb-115">Ратингжерманителевисионтипе</span><span class="sxs-lookup"><span data-stu-id="506fb-115">ratingGermanyTelevisionType</span></span>](../resources/intune-deviceconfig-ratinggermanytelevisiontype.md)|<span data-ttu-id="506fb-116">Рейтинг для телевизора выбран в Германии.</span><span class="sxs-lookup"><span data-stu-id="506fb-116">TV rating selected for Germany.</span></span> <span data-ttu-id="506fb-117">Возможные значения: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="506fb-117">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="506fb-118">Связи</span><span class="sxs-lookup"><span data-stu-id="506fb-118">Relationships</span></span>
<span data-ttu-id="506fb-119">Нет</span><span class="sxs-lookup"><span data-stu-id="506fb-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="506fb-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="506fb-120">JSON Representation</span></span>
<span data-ttu-id="506fb-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="506fb-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingGermany"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingGermany",
  "movieRating": "String",
  "tvRating": "String"
}
```



