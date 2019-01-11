---
title: Тип ресурса mediaContentRatingGermany
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5dd25a8bd29211fd593daf3ecea20a7808384bc1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860006"
---
# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="83ccc-103">Тип ресурса mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="83ccc-103">mediaContentRatingGermany resource type</span></span>

> <span data-ttu-id="83ccc-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="83ccc-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="83ccc-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="83ccc-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="83ccc-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="83ccc-106">Properties</span></span>
|<span data-ttu-id="83ccc-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="83ccc-107">Property</span></span>|<span data-ttu-id="83ccc-108">Тип</span><span class="sxs-lookup"><span data-stu-id="83ccc-108">Type</span></span>|<span data-ttu-id="83ccc-109">Описание</span><span class="sxs-lookup"><span data-stu-id="83ccc-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83ccc-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="83ccc-110">movieRating</span></span>|[<span data-ttu-id="83ccc-111">ratingGermanyMoviesType</span><span class="sxs-lookup"><span data-stu-id="83ccc-111">ratingGermanyMoviesType</span></span>](../resources/intune-deviceconfig-ratinggermanymoviestype.md)|<span data-ttu-id="83ccc-112">Оценка выбранных для Германии фильмы.</span><span class="sxs-lookup"><span data-stu-id="83ccc-112">Movies rating selected for Germany.</span></span> <span data-ttu-id="83ccc-113">Возможные значения: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="83ccc-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="83ccc-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="83ccc-114">tvRating</span></span>|[<span data-ttu-id="83ccc-115">ratingGermanyTelevisionType</span><span class="sxs-lookup"><span data-stu-id="83ccc-115">ratingGermanyTelevisionType</span></span>](../resources/intune-deviceconfig-ratinggermanytelevisiontype.md)|<span data-ttu-id="83ccc-116">Оценка TV, выбранной для Германии.</span><span class="sxs-lookup"><span data-stu-id="83ccc-116">TV rating selected for Germany.</span></span> <span data-ttu-id="83ccc-117">Возможные значения: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="83ccc-117">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="83ccc-118">Связи</span><span class="sxs-lookup"><span data-stu-id="83ccc-118">Relationships</span></span>
<span data-ttu-id="83ccc-119">Нет</span><span class="sxs-lookup"><span data-stu-id="83ccc-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="83ccc-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="83ccc-120">JSON Representation</span></span>
<span data-ttu-id="83ccc-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="83ccc-121">Here is a JSON representation of the resource.</span></span>
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



