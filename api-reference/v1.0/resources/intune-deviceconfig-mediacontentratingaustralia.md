---
title: Тип ресурса mediaContentRatingAustralia
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 29e7c1d6668671afee5e382f6ba71e7d8f146df0
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37360036"
---
# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="a7b4d-103">Тип ресурса mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="a7b4d-103">mediaContentRatingAustralia resource type</span></span>

> <span data-ttu-id="a7b4d-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a7b4d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a7b4d-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="a7b4d-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="a7b4d-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="a7b4d-106">Properties</span></span>
|<span data-ttu-id="a7b4d-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="a7b4d-107">Property</span></span>|<span data-ttu-id="a7b4d-108">Тип</span><span class="sxs-lookup"><span data-stu-id="a7b4d-108">Type</span></span>|<span data-ttu-id="a7b4d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a7b4d-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7b4d-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="a7b4d-110">movieRating</span></span>|[<span data-ttu-id="a7b4d-111">ратингаустралиамовиестипе</span><span class="sxs-lookup"><span data-stu-id="a7b4d-111">ratingAustraliaMoviesType</span></span>](../resources/intune-deviceconfig-ratingaustraliamoviestype.md)|<span data-ttu-id="a7b4d-112">Оценка фильмов выбрана для Австралии.</span><span class="sxs-lookup"><span data-stu-id="a7b4d-112">Movies rating selected for Australia.</span></span> <span data-ttu-id="a7b4d-113">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="a7b4d-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="a7b4d-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="a7b4d-114">tvRating</span></span>|[<span data-ttu-id="a7b4d-115">ратингаустралиателевисионтипе</span><span class="sxs-lookup"><span data-stu-id="a7b4d-115">ratingAustraliaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingaustraliatelevisiontype.md)|<span data-ttu-id="a7b4d-116">Рейтинг для телевизора выбран для Австралии.</span><span class="sxs-lookup"><span data-stu-id="a7b4d-116">TV rating selected for Australia.</span></span> <span data-ttu-id="a7b4d-117">Возможные значения: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span><span class="sxs-lookup"><span data-stu-id="a7b4d-117">Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a7b4d-118">Связи</span><span class="sxs-lookup"><span data-stu-id="a7b4d-118">Relationships</span></span>
<span data-ttu-id="a7b4d-119">Нет</span><span class="sxs-lookup"><span data-stu-id="a7b4d-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a7b4d-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a7b4d-120">JSON Representation</span></span>
<span data-ttu-id="a7b4d-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a7b4d-121">Here is a JSON representation of the resource.</span></span>
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




