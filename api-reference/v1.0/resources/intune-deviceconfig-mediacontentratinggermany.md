---
title: Тип ресурса mediaContentRatingGermany
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b4f2eda6b9666d3b23ea48d96f7a7231e189b4f5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028100"
---
# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="af2a6-103">Тип ресурса mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="af2a6-103">mediaContentRatingGermany resource type</span></span>

> <span data-ttu-id="af2a6-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="af2a6-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="af2a6-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="af2a6-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="af2a6-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="af2a6-106">Properties</span></span>
|<span data-ttu-id="af2a6-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="af2a6-107">Property</span></span>|<span data-ttu-id="af2a6-108">Тип</span><span class="sxs-lookup"><span data-stu-id="af2a6-108">Type</span></span>|<span data-ttu-id="af2a6-109">Описание</span><span class="sxs-lookup"><span data-stu-id="af2a6-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af2a6-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="af2a6-110">movieRating</span></span>|[<span data-ttu-id="af2a6-111">Ратингжерманимовиестипе</span><span class="sxs-lookup"><span data-stu-id="af2a6-111">ratingGermanyMoviesType</span></span>](../resources/intune-deviceconfig-ratinggermanymoviestype.md)|<span data-ttu-id="af2a6-112">Оценка фильмов выбрана для Германии.</span><span class="sxs-lookup"><span data-stu-id="af2a6-112">Movies rating selected for Germany.</span></span> <span data-ttu-id="af2a6-113">Возможные значения: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="af2a6-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="af2a6-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="af2a6-114">tvRating</span></span>|[<span data-ttu-id="af2a6-115">Ратингжерманителевисионтипе</span><span class="sxs-lookup"><span data-stu-id="af2a6-115">ratingGermanyTelevisionType</span></span>](../resources/intune-deviceconfig-ratinggermanytelevisiontype.md)|<span data-ttu-id="af2a6-116">Рейтинг для телевизора выбран в Германии.</span><span class="sxs-lookup"><span data-stu-id="af2a6-116">TV rating selected for Germany.</span></span> <span data-ttu-id="af2a6-117">Возможные значения: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="af2a6-117">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="af2a6-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="af2a6-118">Relationships</span></span>
<span data-ttu-id="af2a6-119">Нет</span><span class="sxs-lookup"><span data-stu-id="af2a6-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="af2a6-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="af2a6-120">JSON Representation</span></span>
<span data-ttu-id="af2a6-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="af2a6-121">Here is a JSON representation of the resource.</span></span>
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



