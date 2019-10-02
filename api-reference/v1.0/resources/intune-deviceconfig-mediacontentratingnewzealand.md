---
title: Тип ресурса mediaContentRatingNewZealand
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b6b90142c50237706ac7e9c887d3a848224c1ec9
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356669"
---
# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="5359f-103">Тип ресурса mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="5359f-103">mediaContentRatingNewZealand resource type</span></span>

> <span data-ttu-id="5359f-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5359f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5359f-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="5359f-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="5359f-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="5359f-106">Properties</span></span>
|<span data-ttu-id="5359f-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="5359f-107">Property</span></span>|<span data-ttu-id="5359f-108">Тип</span><span class="sxs-lookup"><span data-stu-id="5359f-108">Type</span></span>|<span data-ttu-id="5359f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="5359f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5359f-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="5359f-110">movieRating</span></span>|[<span data-ttu-id="5359f-111">ратингневзеаландмовиестипе</span><span class="sxs-lookup"><span data-stu-id="5359f-111">ratingNewZealandMoviesType</span></span>](../resources/intune-deviceconfig-ratingnewzealandmoviestype.md)|<span data-ttu-id="5359f-112">Рейтинг фильмов, выбранный для Новой Зеландии.</span><span class="sxs-lookup"><span data-stu-id="5359f-112">Movies rating selected for New Zealand.</span></span> <span data-ttu-id="5359f-113">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span><span class="sxs-lookup"><span data-stu-id="5359f-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="5359f-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="5359f-114">tvRating</span></span>|[<span data-ttu-id="5359f-115">ратингневзеаландтелевисионтипе</span><span class="sxs-lookup"><span data-stu-id="5359f-115">ratingNewZealandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingnewzealandtelevisiontype.md)|<span data-ttu-id="5359f-116">Рейтинг для телевизора, выбранный для Новой Зеландии.</span><span class="sxs-lookup"><span data-stu-id="5359f-116">TV rating selected for New Zealand.</span></span> <span data-ttu-id="5359f-117">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="5359f-117">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5359f-118">Связи</span><span class="sxs-lookup"><span data-stu-id="5359f-118">Relationships</span></span>
<span data-ttu-id="5359f-119">Нет</span><span class="sxs-lookup"><span data-stu-id="5359f-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5359f-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5359f-120">JSON Representation</span></span>
<span data-ttu-id="5359f-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5359f-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingNewZealand"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingNewZealand",
  "movieRating": "String",
  "tvRating": "String"
}
```




