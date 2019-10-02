---
title: Тип ресурса mediaContentRatingGermany
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3242ffabc3f0bdac7e013ad6ffec97f6dd49d2de
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37359973"
---
# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="6157b-103">Тип ресурса mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="6157b-103">mediaContentRatingGermany resource type</span></span>

> <span data-ttu-id="6157b-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6157b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6157b-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="6157b-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="6157b-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="6157b-106">Properties</span></span>
|<span data-ttu-id="6157b-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="6157b-107">Property</span></span>|<span data-ttu-id="6157b-108">Тип</span><span class="sxs-lookup"><span data-stu-id="6157b-108">Type</span></span>|<span data-ttu-id="6157b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="6157b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6157b-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="6157b-110">movieRating</span></span>|[<span data-ttu-id="6157b-111">ратингжерманимовиестипе</span><span class="sxs-lookup"><span data-stu-id="6157b-111">ratingGermanyMoviesType</span></span>](../resources/intune-deviceconfig-ratinggermanymoviestype.md)|<span data-ttu-id="6157b-112">Оценка фильмов выбрана для Германии.</span><span class="sxs-lookup"><span data-stu-id="6157b-112">Movies rating selected for Germany.</span></span> <span data-ttu-id="6157b-113">Возможные значения: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="6157b-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="6157b-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="6157b-114">tvRating</span></span>|[<span data-ttu-id="6157b-115">ратингжерманителевисионтипе</span><span class="sxs-lookup"><span data-stu-id="6157b-115">ratingGermanyTelevisionType</span></span>](../resources/intune-deviceconfig-ratinggermanytelevisiontype.md)|<span data-ttu-id="6157b-116">Рейтинг для телевизора выбран в Германии.</span><span class="sxs-lookup"><span data-stu-id="6157b-116">TV rating selected for Germany.</span></span> <span data-ttu-id="6157b-117">Возможные значения: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="6157b-117">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6157b-118">Связи</span><span class="sxs-lookup"><span data-stu-id="6157b-118">Relationships</span></span>
<span data-ttu-id="6157b-119">Нет</span><span class="sxs-lookup"><span data-stu-id="6157b-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6157b-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6157b-120">JSON Representation</span></span>
<span data-ttu-id="6157b-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6157b-121">Here is a JSON representation of the resource.</span></span>
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




