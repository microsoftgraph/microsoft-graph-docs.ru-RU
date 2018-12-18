---
title: Тип ресурса mediaContentRatingAustralia
description: Н/Д
author: tfitzmac
ms.openlocfilehash: 01d809b43bc8ce68ffc92600d3634c8bd437a954
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27319504"
---
# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="b2474-103">Тип ресурса mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="b2474-103">mediaContentRatingAustralia resource type</span></span>

> <span data-ttu-id="b2474-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b2474-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b2474-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="b2474-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="b2474-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="b2474-106">Properties</span></span>
|<span data-ttu-id="b2474-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="b2474-107">Property</span></span>|<span data-ttu-id="b2474-108">Тип</span><span class="sxs-lookup"><span data-stu-id="b2474-108">Type</span></span>|<span data-ttu-id="b2474-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b2474-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2474-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="b2474-110">movieRating</span></span>|[<span data-ttu-id="b2474-111">ratingAustraliaMoviesType</span><span class="sxs-lookup"><span data-stu-id="b2474-111">ratingAustraliaMoviesType</span></span>](../resources/intune-deviceconfig-ratingaustraliamoviestype.md)|<span data-ttu-id="b2474-112">Оценка выбранных для Австралии фильмы.</span><span class="sxs-lookup"><span data-stu-id="b2474-112">Movies rating selected for Australia.</span></span> <span data-ttu-id="b2474-113">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="b2474-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="b2474-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="b2474-114">tvRating</span></span>|[<span data-ttu-id="b2474-115">ratingAustraliaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="b2474-115">ratingAustraliaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingaustraliatelevisiontype.md)|<span data-ttu-id="b2474-116">Оценка TV, выбранной для Австралии.</span><span class="sxs-lookup"><span data-stu-id="b2474-116">TV rating selected for Australia.</span></span> <span data-ttu-id="b2474-117">Возможные значения: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span><span class="sxs-lookup"><span data-stu-id="b2474-117">Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b2474-118">Связи</span><span class="sxs-lookup"><span data-stu-id="b2474-118">Relationships</span></span>
<span data-ttu-id="b2474-119">Нет</span><span class="sxs-lookup"><span data-stu-id="b2474-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b2474-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b2474-120">JSON Representation</span></span>
<span data-ttu-id="b2474-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b2474-121">Here is a JSON representation of the resource.</span></span>
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



