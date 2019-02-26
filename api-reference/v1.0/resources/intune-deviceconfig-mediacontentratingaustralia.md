---
title: Тип ресурса mediaContentRatingAustralia
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 37e42c3629e73d8dc629ba754583f8023c168b30
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30259117"
---
# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="7e25f-103">Тип ресурса mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="7e25f-103">mediaContentRatingAustralia resource type</span></span>

> <span data-ttu-id="7e25f-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7e25f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7e25f-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="7e25f-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="7e25f-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="7e25f-106">Properties</span></span>
|<span data-ttu-id="7e25f-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="7e25f-107">Property</span></span>|<span data-ttu-id="7e25f-108">Тип</span><span class="sxs-lookup"><span data-stu-id="7e25f-108">Type</span></span>|<span data-ttu-id="7e25f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="7e25f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e25f-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="7e25f-110">movieRating</span></span>|[<span data-ttu-id="7e25f-111">Ратингаустралиамовиестипе</span><span class="sxs-lookup"><span data-stu-id="7e25f-111">ratingAustraliaMoviesType</span></span>](../resources/intune-deviceconfig-ratingaustraliamoviestype.md)|<span data-ttu-id="7e25f-112">Оценка фильмов выбрана для Австралии.</span><span class="sxs-lookup"><span data-stu-id="7e25f-112">Movies rating selected for Australia.</span></span> <span data-ttu-id="7e25f-113">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="7e25f-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="7e25f-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="7e25f-114">tvRating</span></span>|[<span data-ttu-id="7e25f-115">Ратингаустралиателевисионтипе</span><span class="sxs-lookup"><span data-stu-id="7e25f-115">ratingAustraliaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingaustraliatelevisiontype.md)|<span data-ttu-id="7e25f-116">Рейтинг для телевизора выбран для Австралии.</span><span class="sxs-lookup"><span data-stu-id="7e25f-116">TV rating selected for Australia.</span></span> <span data-ttu-id="7e25f-117">Возможные значения: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span><span class="sxs-lookup"><span data-stu-id="7e25f-117">Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7e25f-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="7e25f-118">Relationships</span></span>
<span data-ttu-id="7e25f-119">Нет</span><span class="sxs-lookup"><span data-stu-id="7e25f-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7e25f-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7e25f-120">JSON Representation</span></span>
<span data-ttu-id="7e25f-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7e25f-121">Here is a JSON representation of the resource.</span></span>
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



