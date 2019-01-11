---
title: Тип ресурса mediaContentRatingFrance
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 502abcae283b7e97e04ab2c342e6b526b41f64f4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829885"
---
# <a name="mediacontentratingfrance-resource-type"></a><span data-ttu-id="de15c-103">Тип ресурса mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="de15c-103">mediaContentRatingFrance resource type</span></span>

> <span data-ttu-id="de15c-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="de15c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="de15c-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="de15c-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="de15c-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="de15c-106">Properties</span></span>
|<span data-ttu-id="de15c-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="de15c-107">Property</span></span>|<span data-ttu-id="de15c-108">Тип</span><span class="sxs-lookup"><span data-stu-id="de15c-108">Type</span></span>|<span data-ttu-id="de15c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="de15c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de15c-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="de15c-110">movieRating</span></span>|[<span data-ttu-id="de15c-111">ratingFranceMoviesType</span><span class="sxs-lookup"><span data-stu-id="de15c-111">ratingFranceMoviesType</span></span>](../resources/intune-deviceconfig-ratingfrancemoviestype.md)|<span data-ttu-id="de15c-112">Оценка выбранных для Франции фильмы.</span><span class="sxs-lookup"><span data-stu-id="de15c-112">Movies rating selected for France.</span></span> <span data-ttu-id="de15c-113">Возможные значения: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="de15c-113">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|
|<span data-ttu-id="de15c-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="de15c-114">tvRating</span></span>|[<span data-ttu-id="de15c-115">ratingFranceTelevisionType</span><span class="sxs-lookup"><span data-stu-id="de15c-115">ratingFranceTelevisionType</span></span>](../resources/intune-deviceconfig-ratingfrancetelevisiontype.md)|<span data-ttu-id="de15c-116">Оценка TV, выбранной для Франции.</span><span class="sxs-lookup"><span data-stu-id="de15c-116">TV rating selected for France.</span></span> <span data-ttu-id="de15c-117">Возможные значения: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="de15c-117">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="de15c-118">Связи</span><span class="sxs-lookup"><span data-stu-id="de15c-118">Relationships</span></span>
<span data-ttu-id="de15c-119">Нет</span><span class="sxs-lookup"><span data-stu-id="de15c-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="de15c-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="de15c-120">JSON Representation</span></span>
<span data-ttu-id="de15c-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="de15c-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingFrance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingFrance",
  "movieRating": "String",
  "tvRating": "String"
}
```



