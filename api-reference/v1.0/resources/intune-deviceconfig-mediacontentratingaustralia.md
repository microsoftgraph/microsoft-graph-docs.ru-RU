---
title: Тип ресурса mediaContentRatingAustralia
description: Н/Д
ms.openlocfilehash: f60df6c4948d0e0208b545a8a25e31ca29247879
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026207"
---
# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="c699f-103">Тип ресурса mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="c699f-103">mediaContentRatingAustralia resource type</span></span>

> <span data-ttu-id="c699f-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c699f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c699f-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="c699f-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="c699f-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="c699f-106">Properties</span></span>
|<span data-ttu-id="c699f-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="c699f-107">Property</span></span>|<span data-ttu-id="c699f-108">Тип</span><span class="sxs-lookup"><span data-stu-id="c699f-108">Type</span></span>|<span data-ttu-id="c699f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c699f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c699f-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="c699f-110">movieRating</span></span>|[<span data-ttu-id="c699f-111">ratingAustraliaMoviesType</span><span class="sxs-lookup"><span data-stu-id="c699f-111">ratingAustraliaMoviesType</span></span>](../resources/intune-deviceconfig-ratingaustraliamoviestype.md)|<span data-ttu-id="c699f-112">Оценка выбранных для Австралии фильмы.</span><span class="sxs-lookup"><span data-stu-id="c699f-112">Movies rating selected for Australia.</span></span> <span data-ttu-id="c699f-113">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="c699f-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="c699f-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="c699f-114">tvRating</span></span>|[<span data-ttu-id="c699f-115">ratingAustraliaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="c699f-115">ratingAustraliaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingaustraliatelevisiontype.md)|<span data-ttu-id="c699f-116">Оценка TV, выбранной для Австралии.</span><span class="sxs-lookup"><span data-stu-id="c699f-116">TV rating selected for Australia.</span></span> <span data-ttu-id="c699f-117">Возможные значения: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span><span class="sxs-lookup"><span data-stu-id="c699f-117">Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c699f-118">Связи</span><span class="sxs-lookup"><span data-stu-id="c699f-118">Relationships</span></span>
<span data-ttu-id="c699f-119">Нет</span><span class="sxs-lookup"><span data-stu-id="c699f-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c699f-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c699f-120">JSON Representation</span></span>
<span data-ttu-id="c699f-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c699f-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingAustralia"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingAustralia",
  "movieRating": "String",
  "tvRating": "String"
}
```



