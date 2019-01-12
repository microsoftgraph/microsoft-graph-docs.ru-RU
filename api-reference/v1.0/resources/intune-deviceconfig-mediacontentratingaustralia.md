---
title: Тип ресурса mediaContentRatingAustralia
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5f3f12cc233c1accfad05ccec92d412c75426d1a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952848"
---
# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="73fe1-103">Тип ресурса mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="73fe1-103">mediaContentRatingAustralia resource type</span></span>

> <span data-ttu-id="73fe1-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="73fe1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="73fe1-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="73fe1-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="73fe1-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="73fe1-106">Properties</span></span>
|<span data-ttu-id="73fe1-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="73fe1-107">Property</span></span>|<span data-ttu-id="73fe1-108">Тип</span><span class="sxs-lookup"><span data-stu-id="73fe1-108">Type</span></span>|<span data-ttu-id="73fe1-109">Описание</span><span class="sxs-lookup"><span data-stu-id="73fe1-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73fe1-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="73fe1-110">movieRating</span></span>|[<span data-ttu-id="73fe1-111">ratingAustraliaMoviesType</span><span class="sxs-lookup"><span data-stu-id="73fe1-111">ratingAustraliaMoviesType</span></span>](../resources/intune-deviceconfig-ratingaustraliamoviestype.md)|<span data-ttu-id="73fe1-112">Оценка выбранных для Австралии фильмы.</span><span class="sxs-lookup"><span data-stu-id="73fe1-112">Movies rating selected for Australia.</span></span> <span data-ttu-id="73fe1-113">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="73fe1-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="73fe1-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="73fe1-114">tvRating</span></span>|[<span data-ttu-id="73fe1-115">ratingAustraliaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="73fe1-115">ratingAustraliaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingaustraliatelevisiontype.md)|<span data-ttu-id="73fe1-116">Оценка TV, выбранной для Австралии.</span><span class="sxs-lookup"><span data-stu-id="73fe1-116">TV rating selected for Australia.</span></span> <span data-ttu-id="73fe1-117">Возможные значения: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span><span class="sxs-lookup"><span data-stu-id="73fe1-117">Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="73fe1-118">Связи</span><span class="sxs-lookup"><span data-stu-id="73fe1-118">Relationships</span></span>
<span data-ttu-id="73fe1-119">Нет</span><span class="sxs-lookup"><span data-stu-id="73fe1-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="73fe1-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="73fe1-120">JSON Representation</span></span>
<span data-ttu-id="73fe1-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="73fe1-121">Here is a JSON representation of the resource.</span></span>
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



