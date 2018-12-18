---
title: Тип ресурса mediaContentRatingJapan
description: Н/Д
author: tfitzmac
ms.openlocfilehash: 1913b28b3020ffdc51edea1a8d93dd726d70efdd
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27328471"
---
# <a name="mediacontentratingjapan-resource-type"></a><span data-ttu-id="c363a-103">Тип ресурса mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="c363a-103">mediaContentRatingJapan resource type</span></span>

> <span data-ttu-id="c363a-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c363a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c363a-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="c363a-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="c363a-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="c363a-106">Properties</span></span>
|<span data-ttu-id="c363a-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="c363a-107">Property</span></span>|<span data-ttu-id="c363a-108">Тип</span><span class="sxs-lookup"><span data-stu-id="c363a-108">Type</span></span>|<span data-ttu-id="c363a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c363a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c363a-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="c363a-110">movieRating</span></span>|[<span data-ttu-id="c363a-111">ratingJapanMoviesType</span><span class="sxs-lookup"><span data-stu-id="c363a-111">ratingJapanMoviesType</span></span>](../resources/intune-deviceconfig-ratingjapanmoviestype.md)|<span data-ttu-id="c363a-112">Оценка выбранных для Японии фильмы.</span><span class="sxs-lookup"><span data-stu-id="c363a-112">Movies rating selected for Japan.</span></span> <span data-ttu-id="c363a-113">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="c363a-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="c363a-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="c363a-114">tvRating</span></span>|[<span data-ttu-id="c363a-115">ratingJapanTelevisionType</span><span class="sxs-lookup"><span data-stu-id="c363a-115">ratingJapanTelevisionType</span></span>](../resources/intune-deviceconfig-ratingjapantelevisiontype.md)|<span data-ttu-id="c363a-116">Оценка TV, выбранной для Японии.</span><span class="sxs-lookup"><span data-stu-id="c363a-116">TV rating selected for Japan.</span></span> <span data-ttu-id="c363a-117">Возможные значения: `allAllowed`, `allBlocked`, `explicitAllowed`.</span><span class="sxs-lookup"><span data-stu-id="c363a-117">Possible values are: `allAllowed`, `allBlocked`, `explicitAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c363a-118">Связи</span><span class="sxs-lookup"><span data-stu-id="c363a-118">Relationships</span></span>
<span data-ttu-id="c363a-119">Нет</span><span class="sxs-lookup"><span data-stu-id="c363a-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c363a-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c363a-120">JSON Representation</span></span>
<span data-ttu-id="c363a-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c363a-121">Here is a JSON representation of the resource.</span></span>
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



