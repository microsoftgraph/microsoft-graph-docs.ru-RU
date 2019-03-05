---
title: Тип ресурса mediaContentRatingUnitedStates
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: baa5d98f0fcb1d267221c95c0b27be988d3a197f
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254732"
---
# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="68980-103">Тип ресурса mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="68980-103">mediaContentRatingUnitedStates resource type</span></span>

> <span data-ttu-id="68980-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="68980-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="68980-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="68980-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="68980-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="68980-106">Properties</span></span>
|<span data-ttu-id="68980-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="68980-107">Property</span></span>|<span data-ttu-id="68980-108">Тип</span><span class="sxs-lookup"><span data-stu-id="68980-108">Type</span></span>|<span data-ttu-id="68980-109">Описание</span><span class="sxs-lookup"><span data-stu-id="68980-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68980-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="68980-110">movieRating</span></span>|[<span data-ttu-id="68980-111">Ратингунитедстатесмовиестипе</span><span class="sxs-lookup"><span data-stu-id="68980-111">ratingUnitedStatesMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedstatesmoviestype.md)|<span data-ttu-id="68980-112">Оценка фильмов, выбранных для США.</span><span class="sxs-lookup"><span data-stu-id="68980-112">Movies rating selected for United States.</span></span> <span data-ttu-id="68980-113">Возможные значения: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="68980-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="68980-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="68980-114">tvRating</span></span>|[<span data-ttu-id="68980-115">Ратингунитедстатестелевисионтипе</span><span class="sxs-lookup"><span data-stu-id="68980-115">ratingUnitedStatesTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedstatestelevisiontype.md)|<span data-ttu-id="68980-116">Рейтинг для телевизора выбран для США.</span><span class="sxs-lookup"><span data-stu-id="68980-116">TV rating selected for United States.</span></span> <span data-ttu-id="68980-117">Возможные значения: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="68980-117">Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="68980-118">Связи</span><span class="sxs-lookup"><span data-stu-id="68980-118">Relationships</span></span>
<span data-ttu-id="68980-119">Нет</span><span class="sxs-lookup"><span data-stu-id="68980-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="68980-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="68980-120">JSON Representation</span></span>
<span data-ttu-id="68980-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="68980-121">Here is a JSON representation of the resource.</span></span>
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



