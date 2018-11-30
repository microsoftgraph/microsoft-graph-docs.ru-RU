---
title: Тип ресурса mediaContentRatingJapan
description: Н/Д
ms.openlocfilehash: 15e905355133545db2cdf0864fcbba7e9c226183
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025783"
---
# <a name="mediacontentratingjapan-resource-type"></a><span data-ttu-id="03229-103">Тип ресурса mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="03229-103">mediaContentRatingJapan resource type</span></span>

> <span data-ttu-id="03229-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="03229-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="03229-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="03229-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="03229-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="03229-106">Properties</span></span>
|<span data-ttu-id="03229-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="03229-107">Property</span></span>|<span data-ttu-id="03229-108">Тип</span><span class="sxs-lookup"><span data-stu-id="03229-108">Type</span></span>|<span data-ttu-id="03229-109">Описание</span><span class="sxs-lookup"><span data-stu-id="03229-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03229-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="03229-110">movieRating</span></span>|[<span data-ttu-id="03229-111">ratingJapanMoviesType</span><span class="sxs-lookup"><span data-stu-id="03229-111">ratingJapanMoviesType</span></span>](../resources/intune-deviceconfig-ratingjapanmoviestype.md)|<span data-ttu-id="03229-112">Оценка выбранных для Японии фильмы.</span><span class="sxs-lookup"><span data-stu-id="03229-112">Movies rating selected for Japan.</span></span> <span data-ttu-id="03229-113">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="03229-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="03229-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="03229-114">tvRating</span></span>|[<span data-ttu-id="03229-115">ratingJapanTelevisionType</span><span class="sxs-lookup"><span data-stu-id="03229-115">ratingJapanTelevisionType</span></span>](../resources/intune-deviceconfig-ratingjapantelevisiontype.md)|<span data-ttu-id="03229-116">Оценка TV, выбранной для Японии.</span><span class="sxs-lookup"><span data-stu-id="03229-116">TV rating selected for Japan.</span></span> <span data-ttu-id="03229-117">Возможные значения: `allAllowed`, `allBlocked`, `explicitAllowed`.</span><span class="sxs-lookup"><span data-stu-id="03229-117">Possible values are: `allAllowed`, `allBlocked`, `explicitAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="03229-118">Связи</span><span class="sxs-lookup"><span data-stu-id="03229-118">Relationships</span></span>
<span data-ttu-id="03229-119">Нет</span><span class="sxs-lookup"><span data-stu-id="03229-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="03229-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="03229-120">JSON Representation</span></span>
<span data-ttu-id="03229-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="03229-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingJapan"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingJapan",
  "movieRating": "String",
  "tvRating": "String"
}
```



