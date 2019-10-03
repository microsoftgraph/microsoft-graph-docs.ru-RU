---
title: Тип ресурса mediaContentRatingUnitedStates
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ee961024a526300b1bbf7ebb186df69ce0337f78
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37366589"
---
# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="273e5-103">Тип ресурса mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="273e5-103">mediaContentRatingUnitedStates resource type</span></span>

> <span data-ttu-id="273e5-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="273e5-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="273e5-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="273e5-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="273e5-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="273e5-106">Properties</span></span>
|<span data-ttu-id="273e5-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="273e5-107">Property</span></span>|<span data-ttu-id="273e5-108">Тип</span><span class="sxs-lookup"><span data-stu-id="273e5-108">Type</span></span>|<span data-ttu-id="273e5-109">Описание</span><span class="sxs-lookup"><span data-stu-id="273e5-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="273e5-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="273e5-110">movieRating</span></span>|[<span data-ttu-id="273e5-111">ратингунитедстатесмовиестипе</span><span class="sxs-lookup"><span data-stu-id="273e5-111">ratingUnitedStatesMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedstatesmoviestype.md)|<span data-ttu-id="273e5-112">Оценка фильмов, выбранных для США.</span><span class="sxs-lookup"><span data-stu-id="273e5-112">Movies rating selected for United States.</span></span> <span data-ttu-id="273e5-113">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="273e5-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="273e5-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="273e5-114">tvRating</span></span>|[<span data-ttu-id="273e5-115">ратингунитедстатестелевисионтипе</span><span class="sxs-lookup"><span data-stu-id="273e5-115">ratingUnitedStatesTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedstatestelevisiontype.md)|<span data-ttu-id="273e5-116">Рейтинг для телевизора выбран для США.</span><span class="sxs-lookup"><span data-stu-id="273e5-116">TV rating selected for United States.</span></span> <span data-ttu-id="273e5-117">Возможные значения: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="273e5-117">Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="273e5-118">Связи</span><span class="sxs-lookup"><span data-stu-id="273e5-118">Relationships</span></span>
<span data-ttu-id="273e5-119">Нет</span><span class="sxs-lookup"><span data-stu-id="273e5-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="273e5-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="273e5-120">JSON Representation</span></span>
<span data-ttu-id="273e5-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="273e5-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingUnitedStates"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingUnitedStates",
  "movieRating": "String",
  "tvRating": "String"
}
```




