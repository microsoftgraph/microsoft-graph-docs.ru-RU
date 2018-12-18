---
title: Тип ресурса mediaContentRatingGermany
description: Н/Д
author: tfitzmac
ms.openlocfilehash: 8add327725e5d3886d381b63c7debc16c256d810
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27327701"
---
# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="721c1-103">Тип ресурса mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="721c1-103">mediaContentRatingGermany resource type</span></span>

> <span data-ttu-id="721c1-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="721c1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="721c1-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="721c1-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="721c1-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="721c1-106">Properties</span></span>
|<span data-ttu-id="721c1-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="721c1-107">Property</span></span>|<span data-ttu-id="721c1-108">Тип</span><span class="sxs-lookup"><span data-stu-id="721c1-108">Type</span></span>|<span data-ttu-id="721c1-109">Описание</span><span class="sxs-lookup"><span data-stu-id="721c1-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="721c1-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="721c1-110">movieRating</span></span>|[<span data-ttu-id="721c1-111">ratingGermanyMoviesType</span><span class="sxs-lookup"><span data-stu-id="721c1-111">ratingGermanyMoviesType</span></span>](../resources/intune-deviceconfig-ratinggermanymoviestype.md)|<span data-ttu-id="721c1-112">Оценка выбранных для Германии фильмы.</span><span class="sxs-lookup"><span data-stu-id="721c1-112">Movies rating selected for Germany.</span></span> <span data-ttu-id="721c1-113">Возможные значения: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="721c1-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="721c1-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="721c1-114">tvRating</span></span>|[<span data-ttu-id="721c1-115">ratingGermanyTelevisionType</span><span class="sxs-lookup"><span data-stu-id="721c1-115">ratingGermanyTelevisionType</span></span>](../resources/intune-deviceconfig-ratinggermanytelevisiontype.md)|<span data-ttu-id="721c1-116">Оценка TV, выбранной для Германии.</span><span class="sxs-lookup"><span data-stu-id="721c1-116">TV rating selected for Germany.</span></span> <span data-ttu-id="721c1-117">Возможные значения: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="721c1-117">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="721c1-118">Связи</span><span class="sxs-lookup"><span data-stu-id="721c1-118">Relationships</span></span>
<span data-ttu-id="721c1-119">Нет</span><span class="sxs-lookup"><span data-stu-id="721c1-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="721c1-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="721c1-120">JSON Representation</span></span>
<span data-ttu-id="721c1-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="721c1-121">Here is a JSON representation of the resource.</span></span>
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



