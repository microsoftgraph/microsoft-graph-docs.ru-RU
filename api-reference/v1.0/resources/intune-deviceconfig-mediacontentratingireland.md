---
title: Тип ресурса mediaContentRatingIreland
description: Н/Д
ms.openlocfilehash: b4348e6f73730d59e6e67b3e102b9ad9caa98add
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024726"
---
# <a name="mediacontentratingireland-resource-type"></a><span data-ttu-id="86d47-103">Тип ресурса mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="86d47-103">mediaContentRatingIreland resource type</span></span>

> <span data-ttu-id="86d47-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="86d47-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="86d47-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="86d47-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="86d47-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="86d47-106">Properties</span></span>
|<span data-ttu-id="86d47-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="86d47-107">Property</span></span>|<span data-ttu-id="86d47-108">Тип</span><span class="sxs-lookup"><span data-stu-id="86d47-108">Type</span></span>|<span data-ttu-id="86d47-109">Описание</span><span class="sxs-lookup"><span data-stu-id="86d47-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86d47-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="86d47-110">movieRating</span></span>|[<span data-ttu-id="86d47-111">ratingIrelandMoviesType</span><span class="sxs-lookup"><span data-stu-id="86d47-111">ratingIrelandMoviesType</span></span>](../resources/intune-deviceconfig-ratingirelandmoviestype.md)|<span data-ttu-id="86d47-112">Оценка выбранных для Ирландия фильмы.</span><span class="sxs-lookup"><span data-stu-id="86d47-112">Movies rating selected for Ireland.</span></span> <span data-ttu-id="86d47-113">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="86d47-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="86d47-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="86d47-114">tvRating</span></span>|[<span data-ttu-id="86d47-115">ratingIrelandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="86d47-115">ratingIrelandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingirelandtelevisiontype.md)|<span data-ttu-id="86d47-116">Оценка TV, выбранной для Ирландия.</span><span class="sxs-lookup"><span data-stu-id="86d47-116">TV rating selected for Ireland.</span></span> <span data-ttu-id="86d47-117">Возможные значения: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span><span class="sxs-lookup"><span data-stu-id="86d47-117">Possible values are: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="86d47-118">Связи</span><span class="sxs-lookup"><span data-stu-id="86d47-118">Relationships</span></span>
<span data-ttu-id="86d47-119">Нет</span><span class="sxs-lookup"><span data-stu-id="86d47-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="86d47-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="86d47-120">JSON Representation</span></span>
<span data-ttu-id="86d47-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="86d47-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingIreland"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingIreland",
  "movieRating": "String",
  "tvRating": "String"
}
```



